# Multiple Features

Linear regression can be extended to use multiple input features instead of just one. This makes the model more powerful because it can use additional information to make better predictions.

## 1. From One Feature to Multiple Features

In the original version of linear regression, the model used a single feature $x$ (for example, the size of a house) to predict the target $y$ (the price of the house):

$$
f_{w,b}(x) = wx + b
$$

With multiple features available (such as size, number of bedrooms, number of floors, and age of the house), the model can make use of all of this information.

## 2. Notation for Multiple Features

The features are represented as:

$$
x_1, x_2, x_3, \dots, x_n
$$

- $x_j$ refers to the $j$-th feature.
- $n$ is the total number of features.

The $i$-th training example is written as $x^{(i)}$. When there are multiple features, $x^{(i)}$ is a list (vector) that contains all the feature values for that example.

A specific feature in a specific training example is written as:

$$
x^{(i)}_j
$$

This is the value of feature $j$ in training example $i$.

## 3. The Model with Multiple Features

With $n$ features, the linear regression model becomes:

$$
f_{\mathbf{w},b}(\mathbf{x}) = w_1 x_1 + w_2 x_2 + w_3 x_3 + \dots + w_n x_n + b
$$

Each feature $x_j$ has its own parameter $w_j$. The parameter $b$ remains a single number (the bias or intercept term).

**Example interpretation** (housing price prediction):

- $w_1 = 0.1$ → each additional square foot increases the predicted price by $100$ (when prices are in thousands of dollars)
- $w_2 = 4$ → each additional bedroom increases the predicted price by $4{,}000$
- $w_3 = 10$ → each additional floor increases the predicted price by $10{,}000$
- $w_4 = -2$ → each additional year of age decreases the predicted price by $2{,}000$
- $b = 80$ → base price of $80{,}000$

## 4. Vector Notation

The parameters $w_1, w_2, \dots, w_n$ can be grouped into a single vector:

$$
\mathbf{w} = [w_1, w_2, \dots, w_n]
$$

The features of an example can also be written as a vector:

$$
\mathbf{x} = [x_1, x_2, \dots, x_n]
$$

Using this notation, the model can be written more compactly with the **dot product**:

$$
f_{\mathbf{w},b}(\mathbf{x}) = \mathbf{w} \cdot \mathbf{x} + b
$$

The dot product $\mathbf{w} \cdot \mathbf{x}$ is defined as:

$$
\mathbf{w} \cdot \mathbf{x} = w_1 x_1 + w_2 x_2 + \dots + w_n x_n
$$

This is exactly the same expression as the expanded form shown earlier.

## 5. Multiple Linear Regression

The version of linear regression that uses multiple input features is called **multiple linear regression**.

This is different from univariate linear regression, which uses only a single feature.

## 6. Key Takeaways

- Multiple features allow the model to use more information when making predictions.
- The model with $n$ features is:

$$
f_{\mathbf{w},b}(\mathbf{x}) = w_1 x_1 + w_2 x_2 + \dots + w_n x_n + b
$$

- This can be written more compactly using vectors and the dot product:

$$
f_{\mathbf{w},b}(\mathbf{x}) = \mathbf{w} \cdot \mathbf{x} + b
$$

- $n$ is the number of features, $x^{(i)}$ is the feature vector of the $i$-th training example, and $x^{(i)}_j$ is the $j$-th feature of that example.
- This form of the algorithm is called **multiple linear regression**.
