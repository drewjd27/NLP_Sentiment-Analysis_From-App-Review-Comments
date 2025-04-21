# Sentiment Analysis on BRImo Application Reviews

This project focuses on sentiment analysis of user reviews for the BRImo application. The goal is to classify user reviews into positive, neutral, or negative sentiments using various machine learning and deep learning models.

## Project Structure

```
.
├── .gitignore
├── notebook_sentiment-analysis.ipynb
├── README.md
├── requirements.txt
├── scraping.ipynb
├── submission.zip
├── ulasan_aplikasi.csv
└── .ipynb_checkpoints/
```

### Key Files
- **`notebook_sentiment-analysis.ipynb`**: Main notebook containing data preprocessing, modeling, and evaluation.
- **`scraping.ipynb`**: Notebook for scraping user reviews from the Google Play Store.
- **`ulasan_aplikasi.csv`**: Dataset containing user reviews.
- **`requirements.txt`**: List of dependencies required to run the project.

---

## How to Rerun the Project

### Prerequisites
1. Install Python 3.11 or later.
2. Install Jupyter Notebook or JupyterLab.

### Steps to Run
1. **Clone the Repository**:
   ```bash
   git clone <https://github.com/drewjd27/NLP_Sentiment-Analysis_From-App-Review-Comments.git>
   cd <repository-folder>
   ```

2. **Install Dependencies**:
   Use the `requirements.txt` file to install the necessary Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Scraping Notebook**:
   If you need to scrape new data, open `scraping.ipynb` in Jupyter Notebook and execute all cells.

4. **Run the Sentiment Analysis Notebook**:
   Open `notebook_sentiment-analysis.ipynb` in Jupyter Notebook and execute all cells step by step:
   - **Data Preprocessing**: Clean and preprocess the dataset.
   - **Model Training**: Train machine learning and deep learning models.
   - **Evaluation**: Evaluate the models' performance.

5. **Inference/Testing**:
   At the end of the `notebook_sentiment-analysis.ipynb`, you can input new sentences to predict their sentiment.

---

## Models Used
1. **Machine Learning Models**:
   - Naive Bayes
   - Random Forest
   - Logistic Regression
   - Decision Tree

2. **Deep Learning Models**:
   - CNN
   - Bi-LSTM
   - RNN-LSTM

---

## Results
The project compares the performance of traditional machine learning models with deep learning models. Deep learning models generally outperform traditional models in terms of accuracy.

---

## Dataset
The dataset (`ulasan_aplikasi.csv`) contains user reviews scraped from the Google Play Store. It includes fields such as:
- `content`: The review text.
- `score`: The rating given by the user.
- `appVersion`: The version of the app reviewed.
- `reviewId`: ID unik untuk setiap ulasan.
- `userName`: Nama pengguna yang memberikan ulasan.
- `userImage`: Foto profil yang memberikan ulasan.
- `content`: Teks ulasan yang diberikan oleh pengguna.
- `score`: Nilai bintang yang diberikan oleh yang memberikan ulasan terhadap aplikasi (1 hingga 5 bintang).
- `thumbsUpCount`: Jumlah like yang dimiliki ulasan.
- `reviewCreatedVersion`: Versi saat ulasan diberikan.
- `at`: Waktu saat ulasan diberikan.
- `replyContent`: Balasan oleh pemilik aplikasi terhadap ulasan .
- `repliedAt`: Waktu saat balasan ulasan diterima
- `appVersion`: Versi aplikasi

---

## Notes
- Ensure that the `nltk` library's required datasets (e.g., stopwords) are downloaded before running the notebooks.
- The project uses TensorFlow for deep learning models. Ensure GPU support is enabled for faster training if available.

---
```
