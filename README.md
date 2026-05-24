# CodTech Machine Learning Internship

## Intern Details

| Field | Details |
|-------|---------|
| **Name** |  Uppara Sravani |
| **Company** | CodTech IT Solutions |
| **Domain** | Machine Learning |
| **Duration** | 8 Weeks |

---

## Repository Structure

```
CodTech-ML-Internship/
│
├── Task1_Decision_Tree/
│   └── decision_tree_task1.py
│
├── Task2_Sentiment_Analysis/
│   └── sentiment_analysis_task2.py
│
├── Task3_Image_Classification/
│   └── image_classification_task3.py
│
├── Task4_Recommendation_System/
│   └── recommendation_system_task4.py
│
└── README.md
```

---

## Task Overview

---

### Task 1 - Decision Tree Implementation

**Objective:** Build and visualize a Decision Tree model to classify or predict outcomes on a dataset.

**Dataset:** Iris Dataset (built-in from sklearn)

**Libraries Used:**
`scikit-learn` `matplotlib` `seaborn` `pandas` `numpy`

**What was done:**
- Loaded and explored the Iris dataset
- Performed EDA with pairplot and correlation heatmap
- Built a DecisionTreeClassifier with Gini criterion
- Evaluated using accuracy, confusion matrix, classification report
- Visualized the full decision tree diagram
- Plotted feature importance chart
- Checked overfitting using train vs test accuracy across different depths

**Result:** Achieved high classification accuracy on the test set

---

### Task 2 - Sentiment Analysis with NLP

**Objective:** Perform sentiment analysis on customer reviews using TF-IDF Vectorization and Logistic Regression.

**Dataset:** Custom customer reviews dataset (40 reviews — 20 positive, 20 negative)

**Libraries Used:**
`scikit-learn` `nltk` `matplotlib` `seaborn` `pandas` `numpy`

**What was done:**
- Created and cleaned a customer reviews dataset
- Text preprocessing — lowercase, punctuation removal, stopword removal
- Converted text to numerical features using TF-IDF Vectorizer
- Trained Logistic Regression classifier
- Evaluated using accuracy, confusion matrix, classification report
- Visualized top positive and negative sentiment words
- Built a function to predict sentiment of any new review

**Result:** Successfully classified reviews as Positive or Negative

---

### Task 3 - Image Classification Model (CNN)

**Objective:** Build a Convolutional Neural Network (CNN) for image classification using TensorFlow/Keras.

**Dataset:** CIFAR-10 (60,000 images across 10 classes — built-in Keras dataset)

**Libraries Used:**
`tensorflow` `keras` `matplotlib` `seaborn` `numpy` `scikit-learn`

**CNN Architecture:**
```
Input (32x32x3)
    -> Conv2D(32) + BN + Conv2D(32) + MaxPool + Dropout
    -> Conv2D(64) + BN + Conv2D(64) + MaxPool + Dropout
    -> Conv2D(128) + BN + MaxPool + Dropout
    -> Flatten -> Dense(256) + BN + Dropout
    -> Output Dense(10) Softmax
```

**What was done:**
- Loaded and normalized CIFAR-10 dataset
- Applied data augmentation (flip, shift, zoom)
- Built a 3-block CNN with BatchNormalization and Dropout
- Trained with EarlyStopping callback
- Plotted accuracy and loss curves
- Evaluated with confusion matrix and per-class accuracy
- Visualized predictions with correct/wrong color coding

**Result:** Functional CNN model with good performance on test data

---

### Task 4 - Recommendation System

**Objective:** Build a recommendation system using Collaborative Filtering and Matrix Factorization techniques.

**Dataset:** Custom movie ratings dataset (10 users, 10 movies)

**Libraries Used:**
`scikit-surprise` `matplotlib` `seaborn` `pandas` `numpy`

**Techniques Used:**

| Technique | Method | Library |
|-----------|--------|---------|
| Collaborative Filtering | KNN (User-Based, Cosine Similarity) | Surprise |
| Matrix Factorization | SVD (Singular Value Decomposition) | Surprise |

**What was done:**
- Created a user-movie ratings matrix
- Visualized rating distribution and average rating per movie
- Plotted user-movie heatmap
- Implemented KNN-based collaborative filtering
- Implemented SVD-based matrix factorization
- Compared both methods using RMSE and MAE
- Performed 5-fold cross validation
- Built Top-N recommendation function
- Generated top 5 movie recommendations for multiple users

**Result:** SVD outperformed KNN with lower RMSE and MAE

---

## Libraries and Installation

Most libraries come pre-installed in Google Colab. For any missing ones:

```python
# Task 1, 2, 3
!pip install scikit-learn matplotlib seaborn pandas numpy nltk tensorflow

# Task 4 only
!pip install scikit-surprise
```

---

## Results Summary

| Task | Method | Metric | Score |
|------|--------|--------|-------|
| Task 1 | Decision Tree | Accuracy | ~95%+ |
| Task 2 | Logistic Regression + TF-IDF | Accuracy | ~90%+ |
| Task 3 | CNN (3-block) | Test Accuracy | ~70-75% |
| Task 4 | SVD | RMSE | Low error |

---

## References

- [Scikit-learn Documentation](https://scikit-learn.org/)
- [TensorFlow / Keras Documentation](https://www.tensorflow.org/)
- [Surprise Library Documentation](https://surpriselib.com/)
- [CIFAR-10 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html)
- [NLTK Documentation](https://www.nltk.org/)

---

## Certificate

Completion certificate will be issued at the end of the internship program  by **CodTech IT Solutions**.

---

*Submitted as part of the CodTech Machine Learning Internship Program.*
