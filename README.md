# 🚨 Emergency Message Prioritizer

An NLP and Machine Learning project that automatically classifies emergency-related messages into different categories. The system can help organize large volumes of emergency information and identify the type of emergency message.

## 📌 Project Overview

During emergency and disaster situations, a large number of messages can be generated within a short period of time. Manually analyzing and categorizing these messages can be time-consuming.

This project uses **Natural Language Processing (NLP)** and **Machine Learning** to automatically classify emergency-related messages into predefined categories.

## 🎯 Objective

The main objective of this project is to:

* Process emergency-related text messages
* Convert text into numerical features
* Train a machine learning classification model
* Automatically predict the category of a new emergency message
* Evaluate the performance of the trained model

## 📊 Dataset

The project uses the **HumAID dataset**.

* Training samples: **53,531**
* Validation samples: **7,793**
* Test samples: **15,160**
* Number of categories: **10**

The dataset contains emergency-related messages associated with different types of information during disaster situations.

## 🧹 Text Preprocessing

Before training the model, the text data is cleaned using basic text preprocessing techniques.

The preprocessing step helps remove unnecessary elements from the messages and prepares the text for feature extraction.

## 🔢 Feature Extraction — TF-IDF

The cleaned text is converted into numerical features using **TF-IDF (Term Frequency-Inverse Document Frequency)**.

The project uses:

* **Unigrams** — individual words
* **Bigrams** — pairs of consecutive words

This allows the model to consider both individual terms and short combinations of words.

## 🤖 Machine Learning Model

The classification model used in this project is:

**Linear Support Vector Machine (LinearSVC)**

The model learns patterns from the TF-IDF features and their corresponding emergency categories.

## 📈 Model Evaluation

The model is evaluated using standard classification metrics including:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

These metrics help evaluate how accurately the model classifies emergency-related messages.

## 🧪 Example Prediction

### Input

> Several peoples were injured after the earthquake and need medical assistance

### Predicted Category

`requests_or_urgent_needs`

The trained model identifies the message as a request or urgent need because it describes injured people requiring medical assistance.

## 🛠️ Technologies Used

* Python
* Pandas
* Scikit-learn
* Matplotlib
* Seaborn
* Hugging Face Datasets
* TF-IDF
* LinearSVC
* Joblib
* Google Colab / Jupyter Notebook

## 📁 Project Files

```text
Emergency-Message-Prioritizer/
│
├── Emergency_Message_Prioritizer.ipynb
├── emergency_message_prioritizer.pkl
└── README.md
```

## ▶️ How to Run

1. Download or clone this repository.
2. Open `Emergency_Message_Prioritizer.ipynb` in Google Colab or Jupyter Notebook.
3. Install the required Python libraries.
4. Run the notebook cells in sequence.
5. The trained model can be used to classify new emergency messages.

## 🔮 Future Improvements

Possible future improvements include:

* Adding a web-based user interface
* Real-time emergency message classification
* Improving model performance
* Adding multilingual emergency message support
* Integrating the model with real-time emergency data sources

## 👩‍💻 Project

**Emergency Message Prioritizer**

Built using Machine Learning and Natural Language Processing to support faster organization and classification of emergency-related information.

