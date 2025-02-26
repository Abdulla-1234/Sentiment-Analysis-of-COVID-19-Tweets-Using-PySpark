# Machine Learning Based Sentiment Analysis of COVID-19 Twitter Data Using PySpark

![Sentiment Analysis Banner](white_png.png)

## Overview
This project implements a **sentiment analysis system** using **PySpark** for analyzing **COVID-19-related Twitter data**. It employs **machine learning techniques** such as **K-Nearest Neighbors (KNN), Logistic Regression, Decision Tree, and Support Vector Machine (SVM)** to classify tweets as **positive, negative, or neutral**.

## Features
- **Big Data Processing**: Uses **Apache Spark** for large-scale data processing.
- **Machine Learning Models**: Implements multiple classifiers for better accuracy.
- **Text Preprocessing**: Includes tokenization, stopword removal, and stemming.
- **Visualization**: Displays results using word clouds, accuracy metrics, and performance graphs.
- **Deployment Ready**: Can be integrated with real-time Twitter streaming.

## System Architecture
![System Architecture](https://github.com/Abdulla-1234/Sentiment-Analysis-of-COVID-19-Tweets-Using-PySpark/blob/main/Images/System%20Architecture.png)

The system consists of the following components:
1. **Data Collection**: Extracts Twitter data from **data/Coronavirus Tweets.csv**.
2. **Preprocessing**: Cleans and tokenizes text data.
3. **Feature Engineering**: Converts text into numerical representations (TF-IDF, CountVectorizer).
4. **Model Training**: Uses ML algorithms (KNN, SVM, Logistic Regression, Decision Tree).
5. **Evaluation & Visualization**: Analyzes model performance using confusion matrices and accuracy metrics.

## Technologies Used
- **Programming Language**: Python
- **Framework**: Apache Spark (PySpark)
- **ML Algorithms**: KNN, Logistic Regression, Decision Tree, SVM
- **Visualization**: Matplotlib, Seaborn, WordCloud
- **Data Storage**: Pandas, NumPy

## Folder Structure
```
Sentiment_Analysis/
│── README.md                      # Project documentation
│── Coronavirus_Tweet_Sentiment_Analysis_Capstone_Project.ipynb  # Jupyter Notebook for analysis
│── white_png.png                   # Image used in the README
│── data/
│   ├── Coronavirus Tweets.csv       # Raw Twitter dataset
│── Report/
│   ├── Report.pdf                   # Detailed project report
│   ├── BDA_final.pptx                # Presentation slides
```

## Installation & Setup
### Prerequisites
- **Python 3.x**
- **Apache Spark & PySpark**
- **Twitter API Credentials** (if collecting new data)

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/Sentiment_Analysis.git
   cd Sentiment_Analysis
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run data preprocessing:
   ```sh
   python src/preprocess.py
   ```
4. Train the machine learning model:
   ```sh
   python src/model.py
   ```
5. Evaluate performance:
   ```sh
   python src/evaluate.py
   ```

## Results
### Confusion Matrix CV
| Logistic regression | Decision tree | SVM | KNN |
|---------------|----------------|----------------|----------------|
| ![LR](https://github.com/Abdulla-1234/Sentiment-Analysis-of-COVID-19-Tweets-Using-PySpark/blob/main/Images/Confusion%20matrix_Logistic_Regression.png) | ![Decision tree](https://github.com/Abdulla-1234/Sentiment-Analysis-of-COVID-19-Tweets-Using-PySpark/blob/main/Images/Confusion%20matrix_Dession_tree.png) | ![SVM](https://github.com/Abdulla-1234/Sentiment-Analysis-of-COVID-19-Tweets-Using-PySpark/blob/main/Images/Confusion%20matrix_SVM.png) | ![KNN](https://github.com/Abdulla-1234/Sentiment-Analysis-of-COVID-19-Tweets-Using-PySpark/blob/main/Images/Confusion%20matrix_KNN.png) |

#### TF-IDF Vectorizer
| Logistic regression | Decision tree | SVM | KNN |
|---------------|----------------|----------------|----------------|
| ![LR](https://github.com/Abdulla-1234/Sentiment-Analysis-of-COVID-19-Tweets-Using-PySpark/blob/main/Images/TF-IDF_Legistic_Regression.png) | ![DT](https://github.com/Abdulla-1234/Sentiment-Analysis-of-COVID-19-Tweets-Using-PySpark/blob/main/Images/TF-IDF_Dession_tree.png) | ![SVM](https://github.com/Abdulla-1234/Sentiment-Analysis-of-COVID-19-Tweets-Using-PySpark/blob/main/Images/TF-IDF_SVM.png) | ![KNN](https://github.com/Abdulla-1234/Sentiment-Analysis-of-COVID-19-Tweets-Using-PySpark/blob/main/Images/TF-IDF_KNN.png) |

### Performance Metrics and Accuracy
| Count Vector | TF-IDF Vector |
|---------------|----------------|
| ![count](https://github.com/Abdulla-1234/Sentiment-Analysis-of-COVID-19-Tweets-Using-PySpark/blob/main/Images/performance_count%20vector.png) | ![vector](https://github.com/Abdulla-1234/Sentiment-Analysis-of-COVID-19-Tweets-Using-PySpark/blob/main/Images/performance_vector_TF-IDF.png) |

## Future Enhancements
- **Real-time sentiment tracking** using streaming APIs.
- **Multi-language sentiment analysis** support.
- **Integration with social media dashboards** for live analysis.

## Authors
- [Mohammad Abdulla](https://www.linkedin.com/in/mohammad-abdulla-doodakula-8a3307258/)

---
**Contributions are welcome! Feel free to fork, improve, or raise issues for discussion. 🚀**
