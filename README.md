<h1>Phishing Email Classification System</h1>

<h2>Overview</h2>
<p>This project focuses on detecting phishing emails using Natural Language Processing (NLP) and Machine Learning techniques.
The goal is to classify email content as either <b>Phishing</b> or <b>Legitimate</b>.</p>
<p>The model analyzes textual patterns and learns distinguishing features that help identify malicious or deceptive emails.</p>

<h2>Objective</h2>
<ul>
  <li>Classify emails into Phishing or Legitimate categories</li>
  <li>Build a complete NLP pipeline for text classification</li>
  <li>Understand feature extraction using TF-IDF</li>
  <li>Evaluate model performance using standard metrics</li>
</ul>

<h2>Dataset</h2>
<p>The dataset used contains email messages labeled as phishing or legitimate.</p>
<p>Each record includes:</p>
<ul>
  <li>Email text</li>
  <li>Label (1 = Phishing, 0 = Legitimate)</li>
</ul>

<p>Dataset Link: 
<a href="https://www.kaggle.com/datasets/kuladeep19/phishing-and-legitimate-emails-dataset" target="_blank">
https://www.kaggle.com/datasets/kuladeep19/phishing-and-legitimate-emails-dataset
</a></p>

<h2>Tech Stack</h2>
<ul>
  <li>Python</li>
  <li>Pandas, NumPy</li>
  <li>Matplotlib</li>
  <li>Scikit-learn</li>
  <li>Natural Language Processing (NLP)</li>
</ul>

<h2>Data Preprocessing</h2>
<p>Text data was cleaned and standardized before training the model:</p>
<ul>
  <li>Converted text to lowercase</li>
  <li>Removed URLs</li>
  <li>Removed special characters and punctuation</li>
  <li>Handled missing values</li>
  <li>Stored cleaned text in a separate column</li>
</ul>
<p>These steps reduce noise and improve model performance.</p>

<h2>Exploratory Data Analysis (EDA)</h2>
<p>Initial analysis and visualizations were performed:</p>
<ul>
  <li>Distribution of phishing vs legitimate emails</li>
  <li>Text length distribution</li>
  <li>Inspection of cleaned versus original text</li>
</ul>
<p>This helped in understanding dataset balance and structure.</p>

<h2>Feature Engineering</h2>
<h3>TF-IDF Vectorization</h3>
<p>Text data was converted into numerical form using TF-IDF:</p>
<ul>
  <li>Transforms text into numerical feature vectors</li>
  <li>Captures importance of words and phrases</li>
  <li>Reduces the impact of frequently occurring words</li>
</ul>
<p>This allows the model to process textual input effectively.</p>

<h2>Model Building</h2>
<h3>Algorithm Used: Logistic Regression</h3>
<ul>
  <li>Supervised learning algorithm suitable for binary classification</li>
  <li>Efficient and scalable for large text datasets</li>
  <li>Performs well with high-dimensional sparse data</li>
</ul>
<p>The model was trained on TF-IDF-transformed features to classify emails.</p>

<h2>Model Evaluation</h2>
<p>The model was evaluated using:</p>
<ul>
  <li><b>Accuracy Score</b> to measure overall performance</li>
  <li><b>Confusion Matrix</b> to analyze predictions</li>
  <li><b>Classification Report</b> including:
    <ul>
      <li>Precision</li>
      <li>Recall</li>
      <li>F1-score</li>
    </ul>
  </li>
</ul>
<p>These metrics provide detailed insights into model performance.</p>

<h2>Visualizations</h2>

<h3>Email Class Distribution</h3>
<p>Shows the distribution of phishing and legitimate emails in the dataset.</p>
<img src="https://github.com/IshitaSinha2002/Email-Classifier/blob/main/email%20labels.png" width: 500px; height: 400px; object-fit: cover;>

<h3>Confusion Matrix</h3>
<p>Displays actual versus predicted classifications.</p>
<img src="https://github.com/IshitaSinha2002/Email-Classifier/blob/main/cm.png" width: 500px; height: 400px; object-fit: cover;>

<h2>Key Insights</h2>
<ul>
  <li>Phishing emails often contain urgency, threats, or reward-based language</li>
  <li>Legitimate emails tend to have structured and contextual communication</li>
  <li>TF-IDF effectively captures important textual patterns</li>
  <li>Logistic Regression provides strong baseline performance</li>
</ul>

<h2>Prediction System</h2>
<p>A prediction system was implemented to classify new email text.</p>
<p>The process involves:</p>
<ul>
  <li>Cleaning the input text</li>
  <li>Transforming it using the trained TF-IDF vectorizer</li>
  <li>Passing it to the trained model</li>
  <li>Returning the predicted class</li>
</ul>

<h3>Sample Input and Output</h3>
<p>
Input: Your account has been suspended. Click here to verify.<br>
Output: Phishing
</p>

<h2>Conclusion</h2>
<p>This project demonstrates how NLP and machine learning techniques can be used to detect phishing emails.
It showcases a complete workflow from preprocessing and feature extraction to model evaluation and prediction.</p>
