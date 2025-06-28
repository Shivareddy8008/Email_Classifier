# Email_Classifier
# 📧 Spam Email Detection using NLP & Machine Learning

A machine learning project that classifies email messages as **Spam** or **Ham** (not spam) using **Natural Language Processing (NLP)** techniques and a **Multinomial Naive Bayes** classifier. The model is deployed with an interactive **Gradio web interface** for real-time predictions.

---

## 📁 Dataset

- **Name**: `spam_ham_dataset.csv`
- **Entries**: 5171 email messages
- **Columns**:
  - `label`: Text label ("spam" or "ham")
  - `text`: The raw email message
  - `label_num`: Numeric encoding of label (1 = spam, 0 = ham)

---

## ⚙️ Features & Workflow

1. **Text Preprocessing**:
   - Lowercasing
   - Tokenization
   - Stopword removal
   - Alphanumeric filtering

2. **Feature Extraction**:
   - Applied **TF-IDF Vectorization** (`max_features=5000`) to convert text to numeric form

3. **Model Training**:
   - Used **Multinomial Naive Bayes**
   - Split: 75% Training / 25% Testing

4. **Model Evaluation**:
   - **Accuracy**: ~94.7%
   - **Precision**: ~88.5%
   - **Recall**: ~93.1%

5. **Deployment**:
   - Gradio interface for interactive use
   - Users can paste email text and get instant classification (Spam or Ham)

---
Output Image :
![Screenshot 2025-06-28 225753](https://github.com/user-attachments/assets/b016101c-11b5-49cb-8c3c-db43440c4586)






## 🚀 How to Run

### 1. Clone the Repo
```bash
git clone https://github.com/your-username/spam-email-detector.git
cd spam-email-detector
