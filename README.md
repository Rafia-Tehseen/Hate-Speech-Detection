# Hate Speech and Cyberbullying Detection

### 📌 Project Overview
This project focuses on the automated identification and classification of hate speech, aggression, and cyberbullying in social media text. By leveraging a multi-source dataset and advanced Deep Learning architectures, the project distinguishes between various forms of toxic content, including racism, sexism, and general aggression.

### 📂 Dataset Information
The project utilizes a comprehensive **Cyberbullying Dataset** that aggregates data from Twitter, YouTube, and Wikipedia.
*   **Total Initial Samples:** 420,528
*   **Unique Samples (After De-duplication):** 225,349
*   **Class Distribution:** 
    *   **none:** 200,577 samples
    *   **aggression:** 14,764 samples
    *   **sexism:** 3,377 samples
    *   **hate:** 3,194 samples
    *   **racism:** 1,970 samples
    *   **toxic:** 1,464 samples

### ⚙️ Methodology & Preprocessing
A robust Natural Language Processing (NLP) pipeline was established to clean and prepare the raw social media text:
*   **Text Cleaning:** Removal of URLs, mentions (@), hashtags (#), numbers, and special punctuation.
*   **NLP Techniques:** Lowercase conversion, tokenization, stop-word removal, and lemmatization using NLTK.
*   **Feature Engineering:** Extraction of metadata such as word count, character count, average word length, sentence count, and part-of-speech (POS) tags.
*   **Vectorization:** Conversion of text into numerical format using **TF-IDF (Term Frequency-Inverse Document Frequency)** and **Word2Vec** embeddings.

### 🤖 Model Performance & Results
The project compared traditional machine learning classifiers with deep learning models to find the most effective solution.

#### 1. Random Forest Classifier
*   **Weighted Average Accuracy:** 85%
*   **Weighted F1-Score:** 0.82
*   **Key Finding:** Strong performance on neutral content but struggled with minority toxic classes due to significant dataset imbalance.

#### 2. Deep Learning (Sequential Neural Network)
A multi-layer architecture was trained for 10 epochs:
*   **Training Accuracy:** 89.10%
*   **Validation Accuracy:** 88.96%
*   **Test Accuracy:** **88.97%**
*   **Micro F1-Score:** 0.8897
*   **Hamming Loss:** 0.0315

### 📊 Key Visualizations
To provide a complete overview of the findings, the following visualizations are included in the analysis:
*   **Number of Annotations in Each Category:** A bar chart illustrating the class distribution.
*   **WordCloud:** A visual summary of the most frequent terms in the dataset.
*   **Top 20 Most Common Words:** Identifying frequent terms like 'article', 'page', and 'wikipedia'.
*   **Top 10 Common Hashtags & Mentions:** Specifically categorized for general, sexist, and racist content.
*   **TF-IDF Feature Heatmap:** A visual representation of word importance and feature extraction.
*   **Confusion Matrix:** Evaluating the precision of model predictions across different categories.

### 🛠️ Technologies Used
*   **Language:** Python
*   **Deep Learning:** TensorFlow, Keras
*   **NLP Libraries:** NLTK, TextBlob, WordCloud, Gensim (Word2Vec)
*   **Machine Learning:** Scikit-learn, LazyPredict
*   **Data Analysis:** Pandas, NumPy
*   **Visualization:** Matplotlib, Seaborn, Plotly

### 👨‍💻 Author
**Rafia Tehseen**
