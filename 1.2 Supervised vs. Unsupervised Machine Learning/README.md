# Supervised vs. Unsupervised Machine Learning

## 1. Machine Learning

"Field of study that gives computers the ability to learn without being explicitly programmed." — Arthur Samuel, 1959

Machine learning algorithms learn patterns from data and use those patterns to make predictions, identify structures, or support decisions.

### Machine Learning Algorithms

Machine learning includes several major types:

- **Supervised Learning**
  - Learns from labeled data containing inputs and their corresponding correct outputs.
  - Used in many real-world applications and has seen rapid advancements and innovation.

- **Unsupervised Learning**
  - Learns from unlabeled data to discover patterns, structures, or relationships.

- **Recommender Systems**
  - Use machine learning techniques to suggest relevant items, products, movies, or other content to users.

- **Reinforcement Learning**
  - Learns by interacting with an environment and receiving rewards or penalties based on its actions.

Supervised and unsupervised learning are two major types of machine learning.

## 2. Supervised Learning

Supervised learning refers to algorithms that learn `x-to-y`, or input-to-output, mappings.

- `x` represents the input data or features.
- `y` represents the desired output or label.

### Key Characteristics

- The learning algorithm is provided with examples that include the correct answers.
- The correct answer is the label `y` corresponding to a given input `x`.
- By learning from these input-output pairs, the algorithm identifies patterns and relationships between inputs and their corresponding outputs.
- After training, the algorithm can take new inputs without known output labels and make predictions.

### How Supervised Learning Works

1. **Training Data:** Provide the algorithm with examples containing inputs (`X`) and their corresponding correct outputs (`Y`).
2. **Learning:** The algorithm learns patterns and relationships between the inputs and outputs.
3. **Prediction:** After training, the algorithm uses what it has learned to predict outputs for new, unseen inputs.

These examples are called **labeled training data** because each input has a corresponding correct output.

**Example: Housing Price Prediction**

- A model is trained using housing data containing features such as location, size, and number of bedrooms, along with the actual selling prices.
- The model learns the relationship between these features and house prices.
- After training, it can predict the price of a new house using its available features.

### Two Major Types of Supervised Learning

#### 2.1 Regression

- A type of supervised learning algorithm.
- Predicts a numerical value from infinitely many possible numerical values.
- Used when the output is a numerical quantity.

**Example: Housing Price Prediction**

- Given information about a house, such as its size, location, and number of bedrooms, a regression model predicts its price.
- The predicted price can be any numerical value within the range of possible prices.

#### 2.2 Classification

- The second major type of supervised learning.
- Predicts a category or class from a small, finite set of possible output categories.
- Unlike regression, classification does not predict any arbitrary numerical value.
- Categories can be numeric or non-numeric.
- Output classes and output categories are interchangeable terms.

**Example: Breast Cancer Detection**

- A classification model can use medical data to classify a tumor as:
  - **Benign (0):** Non-cancerous.
  - **Malignant (1):** Cancerous.

### Types of Classification

- **Binary Classification**
  - Predicts one of two possible categories.
  - Example: Classifying a tumor as benign or malignant.

- **Multiclass Classification**
  - Predicts one category from more than two possible categories.
  - Example: Classifying a tumor into multiple possible cancer types.

Classification can also predict non-numeric categories, such as identifying whether an image contains a cat or a dog.

### Multiple Input Features in Classification

- A classification model can use more than one input feature to predict an output.
- For example, a breast cancer detection model can use a patient's age and tumor size.
- More advanced models can use additional features, such as tumor thickness and cell size and shape characteristics.

**Decision Boundary**

- A decision boundary is a line or boundary that separates different predicted categories.
- A classification algorithm can learn a decision boundary that distinguishes between different classes based on the input features.

### Regression vs. Classification

| Feature              | Regression                                | Classification                                   |
| -------------------- | ----------------------------------------- | ------------------------------------------------ |
| **Purpose**          | Predicts a numerical value                | Predicts a category or class                     |
| **Output**           | Numerical value                           | One of a limited set of categories               |
| **Possible Results** | Infinitely many possible numerical values | A finite set of possible categories              |
| **Example**          | Predicting house prices                   | Detecting whether a tumor is benign or malignant |

## 3. Unsupervised Learning

Unsupervised learning refers to algorithms that learn from data without being provided with corresponding output labels.

- The data contains inputs (`X`) but no output labels (`Y`).
- The algorithm is not given the correct answers for individual examples.
- Instead, it tries to discover patterns, structures, relationships, or interesting information within the data.
- The algorithm identifies these patterns on its own without being explicitly told what to look for.

### How Unsupervised Learning Works

1. **Input Data:** Provide the algorithm with data containing input features (`X`) but no corresponding output labels (`Y`).
2. **Pattern Discovery:** The algorithm examines the data to identify similarities, relationships, or structures.
3. **Results:** The algorithm discovers patterns or structures, such as groups of similar data points or unusual observations.

### Important Types of Unsupervised Learning

#### 3.1 Clustering

- A type of unsupervised learning algorithm.
- Takes unlabeled data and automatically groups similar data points into clusters.
- Each cluster contains data points that share similar characteristics or patterns.
- The algorithm discovers the groups without being given predefined categories.

**Examples:**

- **News Article Grouping**
  - Groups related news articles based on similarities in their content.
  - For example, articles about the same event or topic can be grouped together.

- **DNA Data Analysis**
  - Groups individuals based on similarities in their genetic activity.

- **Customer Segmentation**
  - Groups customers based on similar characteristics, interests, or purchasing behavior.
  - Helps businesses better understand and serve different customer groups.

#### 3.2 Anomaly Detection

- Used to identify unusual events or data points that differ from expected patterns.
- Helps detect observations that do not follow normal behavior.

**Examples:**

- Detecting unusual banking transactions that may indicate financial fraud.
- Identifying suspicious network activity.
- Detecting unusual equipment behavior.

#### 3.3 Dimensionality Reduction

- Takes a large dataset and compresses it into a much smaller dataset while losing as little information as possible.
- Reduces the number of features or variables in a dataset while preserving as much important information as possible.
- Helps simplify datasets containing many features, making them easier to analyze and visualize.

## 4. Supervised vs. Unsupervised Learning

| Feature              | Supervised Learning                                     | Unsupervised Learning                                       |
| -------------------- | ------------------------------------------------------- | ----------------------------------------------------------- |
| **Training Data**    | Labeled data                                            | Unlabeled data                                              |
| **Input and Output** | Uses inputs (`X`) and corresponding output labels (`Y`) | Uses inputs (`X`) without corresponding output labels (`Y`) |
| **Learning Goal**    | Learns input-to-output mappings                         | Discovers patterns and structures in data                   |
| **Expected Result**  | Predicts outputs for new inputs                         | Identifies patterns, groups, or unusual data points         |
| **Main Techniques**  | Regression and Classification                           | Clustering, Anomaly Detection, and Dimensionality Reduction |
| **Examples**         | Housing price prediction and breast cancer detection    | Customer segmentation and news article grouping             |

## 5. Key Takeaways

- Machine learning enables computers to learn from data without being explicitly programmed.
- Supervised learning uses labeled data to learn input-to-output mappings.
- Regression predicts numerical values, while classification predicts categories or classes.
- Classification can predict two categories (binary classification) or more than two categories (multiclass classification).
- Classification models can use multiple input features and learn decision boundaries to distinguish between categories.
- Unsupervised learning uses unlabeled data to discover patterns and structures.
- Clustering groups similar data points into clusters.
- Anomaly detection identifies unusual events or data points.
- Dimensionality reduction compresses large datasets into smaller representations while preserving as much information as possible.
- Machine learning also includes recommender systems and reinforcement learning.
