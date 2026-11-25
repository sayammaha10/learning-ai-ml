# Vectorization

Vectorization is a technique that makes code shorter and significantly more efficient when implementing learning algorithms. It allows the use of modern numerical linear algebra libraries and can take advantage of specialized hardware such as GPUs (Graphics Processing Units).

## 1. Example Setup

Consider parameters $\mathbf{w}$ and $b$, where $\mathbf{w}$ is a vector containing three numbers, and a feature vector $\mathbf{x}$ that also contains three numbers. In this example, $n = 3$.

In linear algebra, indexing usually starts from 1, so the values are written as $w_1, w_2, w_3$ and $x_1, x_2, x_3$.

In Python (using the NumPy library), arrays are indexed starting from 0. The values are therefore accessed as:

- $w[0]$, $w[1]$, $w[2]$
- $x[0]$, $x[1]$, $x[2]$

## 2. Implementation Without Vectorization

### Explicit Calculation

One way to compute the prediction is to multiply each parameter by its corresponding feature and add them together, then add $b$.

This approach becomes impractical and inefficient when $n$ is large (for example, $n = 100$ or $n = 100{,}000$).

### Using a For Loop

A better non-vectorized approach uses a loop:

$$
f = \sum_{j=1}^{n} w_j x_j + b
$$

In code, this can be implemented by initializing $f$ to 0, then looping over the indices and accumulating the products $w_j x_j$, and finally adding $b$ outside the loop.

In Python, `range(n)` makes the index go from 0 to $n-1$.

While this version is more general than writing out every term, it still does not use vectorization and is not computationally efficient.

## 3. Vectorized Implementation

The model can be written using the dot product:

$$
f_{\mathbf{w},b}(\mathbf{x}) = \mathbf{w} \cdot \mathbf{x} + b
$$

This can be computed with a single line of code using NumPy:

    f = np.dot(w, x) + b

The `np.dot` function computes the mathematical dot product between the two vectors. Especially when $n$ is large, this runs much faster than the previous non-vectorized implementations.

## 4. Benefits of Vectorization

Vectorization provides two main advantages:

1. **Shorter code** — The calculation is reduced to a single, readable line.
2. **Faster execution** — Behind the scenes, functions such as `np.dot` can use parallel hardware (on both regular CPUs and GPUs). This makes the computation much more efficient than sequential for-loops or explicitly written sums.
