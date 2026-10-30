# Supervised vs. Unsupervised Machine Learning

## 1. Machine Learning

"Field of study that gives computers the ability to learn without being explicitly programmed." — Arthur Samuel, 1959

Machine learning algorithms learn patterns from data and use those patterns to make predictions, identify structures, or support decisions.

### Machine Learning Algorithms

- Two main types of machine learning are supervised learning and unsupervised learning.
- **Supervised Learning**
  - Used in most real-world applications.
  - Has seen the most rapid advancements and innovation.
- **Unsupervised Learning**
- **Recommender Systems**
  - Use machine learning techniques to suggest relevant items, products, movies, or other content to users.
- **Reinforcement Learning**
  - Learns by interacting with an environment and receiving rewards or penalties based on its actions.

Supervised and unsupervised learning are two major categories of machine learning.

## 2. Supervised Learning

- Supervised machine learning, or more commonly, supervised learning, refers to algorithms that learn `x-to-y` or input-to-output mappings.
  - `x` represents the input data or features.
  - `y` represents the desired output or label.

- **Key characteristic:**
  - We give the learning algorithm examples to learn from that include the correct answers.
  - The correct answer is the correct label `y` for a given input `x`.
  - By seeing correct pairs of input `x` and desired output label `y`, the learning algorithm eventually learns to take just the input alone, without the output label, and give a reasonably accurate prediction or guess of the output.

### How Supervised Learning Works

- The algorithm is trained using examples that contain both inputs and their corresponding correct outputs.
- These examples are called **labeled training data**.
- The algorithm identifies patterns and relationships between the inputs and their corresponding outputs.
- After training, the algorithm can take new inputs without known outputs and predict the likely results.

**Example: Housing Price Prediction**

- A model can be trained using housing data containing information such as location, size, and number of bedrooms, along with the actual selling prices.
- After learning from these examples, the model can predict the price of a house based on its features.

### Two Major Types of Supervised Learning

#### 2.1 Regression

- A type of supervised learning algorithm.
- Predicts a number from infinitely many possible numerical values.
- Used when the output is a numerical quantity.
- **Example: Housing Price Prediction**
  - Given information about a house, such as its size, location, and number of bedrooms, a regression model predicts its price.

#### 2.2 Classification

- The second major type of supervised learning problem.
- Different from regression because it tries to predict only a small number of possible outputs or categories.
- Classification predicts a small, finite, and limited set of possible output categories.
- Categories do not have to be numbers.
- **Example: Breast Cancer Detection**
  - A classification model can analyze medical data and classify a tumor as benign or malignant.

### Regression vs. Classification

| Feature              | Regression                     | Classification                                   |
| -------------------- | ------------------------------ | ------------------------------------------------ |
| **Purpose**          | Predicts a numerical value     | Predicts a category or class                     |
| **Output**           | Continuous numerical value     | One of a limited set of categories               |
| **Possible Results** | Many possible numerical values | A finite set of possible classes                 |
| **Example**          | Predicting house prices        | Detecting whether a tumor is benign or malignant |

## 3. Unsupervised Learning

- We are given data that isn't associated with any output labels.
- The data only comes with inputs `x`, but not output labels `y`.
- The goal is to find some structure, pattern, or something interesting in the data.
- It is called unsupervised because we are not trying to supervise the algorithm by giving it the correct answer for every input.
- Instead, we ask the algorithm to figure out by itself what is interesting or what patterns and structures might exist in the data.

### How Unsupervised Learning Works

- The algorithm examines the available data without being provided with correct output labels.
- It tries to discover patterns, relationships, or structures within the data.
- Unlike supervised learning, there are no predefined correct answers for each input.
- The algorithm identifies interesting patterns based on the characteristics of the data.

### Important Types of Unsupervised Learning

#### 3.1 Clustering

- A type of unsupervised learning algorithm.
- Takes data without labels and tries to automatically group the data into clusters.
- Unlabeled data is placed into different clusters based on similarities or patterns.
- Each cluster contains data points that are relatively similar to one another.

**Examples:**

- **Google News**
  - Groups related news articles into different clusters based on their topics.
- **Grouping Customers**
  - Groups customers based on similar characteristics, interests, or purchasing behavior.

#### 3.2 Anomaly Detection

- Used to detect unusual events or data points that differ significantly from normal patterns.
- Helps identify observations that do not follow expected behavior.

**Examples:**

- Detecting unusual banking transactions.
- Identifying suspicious network activity.
- Detecting unusual equipment behavior.

#### 3.3 Dimensionality Reduction

- Takes a big dataset and compresses it into a much smaller dataset while losing as little information as possible.
- Reduces the number of features or variables in a dataset while preserving as much important information as possible.
- Helps simplify datasets containing many features, making them easier to analyze and visualize.

## 4. Supervised vs. Unsupervised Learning

| Feature              | Supervised Learning                                  | Unsupervised Learning                                       |
| -------------------- | ---------------------------------------------------- | ----------------------------------------------------------- |
| **Training Data**    | Labeled data                                         | Unlabeled data                                              |
| **Input and Output** | Uses input `x` and its corresponding output `y`      | Uses input `x` without corresponding output labels `y`      |
| **Learning Goal**    | Learns input-to-output mappings                      | Discovers patterns and structures in data                   |
| **Expected Result**  | Predicts outputs for new inputs                      | Identifies patterns, groups, or unusual data points         |
| **Main Techniques**  | Regression and Classification                        | Clustering, Anomaly Detection, and Dimensionality Reduction |
| **Example**          | Housing price prediction and breast cancer detection | Customer grouping and news article clustering               |

## 5. Key Takeaways

- Machine Learning gives computers the ability to learn from data without being explicitly programmed.
- Supervised learning uses labeled data to learn input-to-output mappings.
- Regression predicts numerical values, while classification predicts categories or classes.
- Unsupervised learning uses unlabeled data to discover patterns and structures.
- Clustering groups similar data points into clusters.
- Anomaly detection identifies unusual events or data points.
- Dimensionality reduction compresses large datasets into smaller representations while preserving important information.
- Machine learning also includes reinforcement learning and applications such as recommender systems.
