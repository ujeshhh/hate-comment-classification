# **Hate Comment Detection and Classification Using NLP**

This project is focused on creating a machine learning model that can automatically detect and classify harmful or hateful comments online. Using a dataset that contains user comments labeled with categories such as toxic, obscene, threat, insult, and identity_hate, the system analyzes text to flag inappropriate content. The goal is to create a safer and more respectful online environment by identifying these harmful comments early.

### **Objective:**
- **Detect** harmful or hateful comments in any given dataset.
- **Classify** these comments into specific hate categories, like toxic, obscene, or threat.
- **Evaluate** the model’s performance through key metrics: accuracy, recall, precision, and F1 score.
- **Visualize** the hateful and non-hateful words with word clouds to better understand the patterns.

### **Project Workflow:**

#### 1. **Data Preprocessing:**
   - Load and clean the dataset to prepare it for analysis.
   - Tokenize the text and remove unnecessary words (stopwords) to optimize processing.
   - Use TfidfVectorizer to transform text into numerical features that a machine learning model can use.

#### 2. **Model Training:**
   - Train separate classifiers for each hate category (e.g., toxic, severe_toxic, threat) using logistic regression.
   - Apply a OneVsRestClassifier approach to handle multilabel classification, so each comment can belong to multiple categories.

#### 3. **Evaluation:**
   - Assess each classifier’s performance using:
     - Accuracy
     - Recall
     - Precision
     - F1 Score
   - Print the metrics for each hate category to understand how well the model is performing.

#### 4. **Hate Detection:**
   - Allow users to input a new comment and predict whether it’s harmful or not, offering real-time feedback.

#### 5. **Visualization:**
   - Generate word clouds that show the most common words in both hateful and non-hateful comments, providing a visual understanding of harmful language.

### **Key Features:**
- **Binary and Multilabel Classification:** Each comment can be classified into one or more hate categories.
- **Real-Time Detection:** Users can input a comment to instantly check whether it’s harmful.
- **Performance Metrics:** The model's performance is carefully evaluated using multiple metrics to ensure accuracy and reliability.
- **Visualization:** Word clouds illustrate common words in harmful and non-harmful comments, making it easier to identify patterns.

### **Tools & Libraries Used:**
- **Python** for the programming language.
- **pandas & numpy** for managing and manipulating data.
- **scikit-learn** for vectorization, model training, and evaluation.
- **matplotlib & wordcloud** for creating visualizations.
- **nltk** for text preprocessing (like tokenization and removing stopwords).

### **Applications:**
- **Social Media Platforms:** Automate the moderation of harmful comments, ensuring a safe online community.
- **Online Forums and Communities:** Prevent the spread of offensive language and hateful content.
- **Content Monitoring:** Help businesses and organizations keep their platforms clean from abusive or harmful posts.

### **Potential Enhancements:**
- Integrate deep learning models like BERT or LSTM for even better accuracy in identifying complex hate speech.
- Expand the classification to cover more detailed categories of hate speech.
- Deploy the model as a web application for practical, real-world use.

