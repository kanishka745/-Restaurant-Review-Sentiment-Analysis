# 🍽️ Restaurant Review Sentiment Analysis

A Machine Learning project for analyzing restaurant customer reviews and classifying them into **Positive** and **Negative** sentiments.

The project uses **Natural Language Processing (NLP)** techniques to convert text reviews into numerical features and applies a **K-Nearest Neighbors (KNN)** classifier for sentiment classification.

---

## 📌 Project Overview

Customer reviews contain valuable information about their experiences with food, service, staff, ambience, and overall restaurant quality.

This project analyzes restaurant reviews to:

* Classify reviews as **Positive** or **Negative**
* Convert text data into numerical features using **CountVectorizer**
* Train a **K-Nearest Neighbors (KNN)** classification model
* Evaluate the model's performance
* Predict the sentiment of new customer reviews
* Identify common positive and negative words
* Analyze customer complaints
* Suggest possible areas for restaurant improvement

---

## 🎯 Objectives

The main objectives of this project are:

1. Analyze restaurant customer reviews.
2. Perform basic text preprocessing and exploration.
3. Convert textual reviews into numerical features.
4. Train a machine learning model for sentiment classification.
5. Evaluate the classification performance.
6. Predict sentiment for new/unseen reviews.
7. Understand customer feedback and complaints.
8. Identify possible areas for improvement.

---

## 🗂️ Project Structure

```text
Restaurant-Review-Sentiment-Analysis/
│
├── Restaurant Review Sentiment Analysis (3)(1).ipynb
├── restaurant_reviews_250.csv
└── README.md
```

---

## 📊 Dataset

The project uses a restaurant review dataset containing customer reviews and their corresponding sentiment labels.

The sentiment categories are:

* **Positive**
* **Negative**

For machine learning, these labels are converted into numerical values:

```text
Positive → 1
Negative → 0
```

---

## 🛠️ Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Scikit-learn
* Natural Language Processing (NLP)
* CountVectorizer
* K-Nearest Neighbors (KNN)
* Matplotlib / visualization tools used in the notebook

---

## 🔄 Project Workflow

```text
Restaurant Reviews
        ↓
Data Loading
        ↓
Data Exploration
        ↓
Sentiment Label Conversion
        ↓
Text Vectorization
        ↓
Train-Test Split
        ↓
KNN Model Training
        ↓
Model Evaluation
        ↓
New Review Prediction
        ↓
Customer Feedback Analysis
```

---

## 🔍 Methodology

### 1. Data Loading

The restaurant review dataset is loaded into a Pandas DataFrame for further analysis.

### 2. Data Exploration

The dataset is explored to understand:

* Number of reviews
* Review text
* Sentiment labels
* Distribution of positive and negative reviews

### 3. Sentiment Encoding

The categorical sentiment labels are converted into numerical values:

```python
Positive → 1
Negative → 0
```

This allows the data to be used with the machine learning classifier.

### 4. Text Vectorization

Since machine learning models cannot directly process raw text, **CountVectorizer** is used.

CountVectorizer converts the reviews into numerical feature vectors based on word occurrences.

Example:

```text
"I love the food"
```

is transformed into numerical features representing the words present in the review.

### 5. Train-Test Split

The dataset is divided into training and testing data.

The training data is used to train the KNN classifier, while the testing data is used to evaluate its performance on unseen reviews.

### 6. K-Nearest Neighbors

The project uses the **K-Nearest Neighbors (KNN)** algorithm for sentiment classification.

The model predicts the sentiment of a review based on the nearest examples in the feature space.

### 7. Model Evaluation

The trained model is evaluated using the testing data.

The notebook calculates the model's classification performance using accuracy.

> The exact accuracy should be taken from the notebook output after running the complete notebook.

---

## 🤖 Sentiment Prediction

After training the model, it can be used to predict the sentiment of new restaurant reviews.

Example:

```text
Input:
"The food was delicious and the service was excellent."

Prediction:
Positive
```

Another example:

```text
Input:
"The food was cold and the service was very slow."

Prediction:
Negative
```

The trained vectorizer transforms the new review into numerical features before passing it to the KNN classifier.

---

## 📈 Customer Feedback Analysis

Apart from sentiment classification, the project also examines customer feedback to understand what customers liked and disliked.

### Positive Feedback

Positive reviews can help identify aspects of the restaurant that customers appreciate, such as:

* Food quality
* Service
* Overall experience
* Staff behavior
* Restaurant experience

### Customer Complaints

Negative reviews can highlight areas where customers experienced problems.

These complaints can be used to identify issues related to:

* Food quality
* Service delays
* Customer experience
* Staff/service
* Other negative aspects mentioned in reviews

---

## 💡 Possible Improvements

The sentiment analysis results can help restaurants understand customer expectations and improve their services.

Possible improvement areas include:

* Improving food quality and consistency
* Reducing service delays
* Improving customer service
* Addressing frequently mentioned complaints
* Maintaining a better overall dining experience

---

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/restaurant-review-sentiment-analysis.git
```

### 2. Navigate to the Project Directory

```bash
cd restaurant-review-sentiment-analysis
```

### 3. Install Required Libraries

```bash
pip install pandas numpy scikit-learn matplotlib jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open the Notebook

Open:

```text
Restaurant Review Sentiment Analysis (3)(1).ipynb
```

Make sure the dataset file:

```text
restaurant_reviews_250.csv
```

is available in the appropriate project directory.

### 6. Run the Cells

Run the notebook cells sequentially to:

1. Load the dataset
2. Explore the data
3. Prepare sentiment labels
4. Vectorize the reviews
5. Split the data
6. Train the KNN model
7. Evaluate the model
8. Predict new reviews
9. Analyze customer feedback

---

## 📁 Files Description

| File                                                | Description                                                                          |
| --------------------------------------------------- | ------------------------------------------------------------------------------------ |
| `Restaurant Review Sentiment Analysis (3)(1).ipynb` | Main Jupyter Notebook containing the complete analysis and machine learning workflow |
| `restaurant_reviews_250.csv`                        | Restaurant review dataset                                                            |
| `README.md`                                         | Project documentation                                                                |

---

## 🔮 Future Improvements

The project can be further improved by:

* Trying different machine learning algorithms
* Comparing KNN with other classifiers
* Improving text preprocessing
* Using TF-IDF instead of only word-count features
* Hyperparameter tuning
* Using confusion matrix and additional evaluation metrics
* Applying advanced NLP techniques
* Increasing the size and diversity of the dataset

---

## 📌 Conclusion

This project demonstrates how **Natural Language Processing and Machine Learning** can be used to analyze restaurant customer reviews.

Using **CountVectorizer** and a **K-Nearest Neighbors classifier**, textual restaurant reviews can be transformed into machine-readable features and classified into positive or negative sentiments.

The analysis can also provide useful insights into customer complaints and potential areas where restaurants can improve their services.

---

## 👨‍💻 Author

**Kanishka**

If you found this project useful, feel free to ⭐ the repository.
