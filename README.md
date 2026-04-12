
# 📰 Fake News Detection System

A machine learning system that detects fake news using multiple classifiers (Logistic Regression, Decision Tree, Gradient Boosting, Random Forest) with **TF-IDF vectorization**. Achieves high accuracy on news article classification.

---

## ✨ Features
- Compare **4 ML classifiers** side-by-side  
- Uses **TF-IDF Vectorization** for text preprocessing  
- **Interactive testing** – test any news article instantly  
- Includes **manual test validation**  
- Clean preprocessing pipeline (removes URLs, punctuation, numbers)  

---

## 🛠️ Tech Stack
```

Python 3.x
├── pandas           # Data manipulation
├── scikit-learn     # ML algorithms & metrics
├── numpy            # Numerical operations
└── re/string        # Text preprocessing

```

---

## 📦 Installation

### 1. Clone the repository
```

git clone <repo-url>
cd <repo-folder>

```

### 2. Install dependencies
```

pip install pandas scikit-learn numpy

```

### 3. Setup Datasets
```

📁 Go to the /dataset folder
🔗 Use the dataset links provided inside the folder
📥 Download Fake.csv and True.csv
📌 Place them inside the /dataset directory

```

### 4. Run the project
```

python fakeNewsDetection.py

```

---

## 🚀 Quick Start
```

1. Run: python fakeNewsDetection.py
2. Enter any news headline/article when prompted
3. Get predictions from ALL 4 models instantly!

```

### Example Input
```

"Scientists discover new species of fish in Pacific Ocean"

```

### Sample Output
```

LR Prediction: Not A Fake News
DT Prediction: Not A Fake News
GBC Prediction: Not A Fake News
RFC Prediction: Not A Fake News

```

---

## 📊 Model Performance

| Model                | Key Strength        | Typical Accuracy |
|---------------------|-------------------|------------------|
| Logistic Regression | Fast inference     | ~98%             |
| Decision Tree       | Interpretable      | ~97%             |
| Gradient Boosting   | High accuracy      | ~99%             |
| Random Forest       | Robust ensemble    | ~99%             |

---

## 🔍 How It Works
```

1. Text Preprocessing → wordopt()
   ↓ Removes: URLs, punctuation, numbers, special characters
2. TF-IDF Vectorization
3. Train 4 classifiers on 44K+ news articles
4. Predict: Fake News (0) or Real News (1)

```

---

## 📁 Project Structure
```

fakeNewsDetection.py     # Main ML pipeline

dataset/
├── README.md            # Dataset download links
├── Fake.csv             # (after download)
└── True.csv             # (after download)

README.md                # Project documentation

````

---

## 🎯 Usage Example
```python
news = "Government announces new tax reforms next month"
manual_testing(news)

# Output: All models predict "Not A Fake News"
````

---

## 🔮 Future Enhancements

* Web UI (Streamlit / Flask)
* BERT / Transformer-based models
* Real-time API deployment
* Cross-validation improvements
* Model saving using joblib

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch

```
git checkout -b feature/your-feature-name
```

3. Commit your changes

```
git commit -m "Add your feature"
```

4. Push to GitHub

```
git push origin feature/your-feature-name
```

5. Open a Pull Request

---

## 📌 Note

Datasets are **not included in the repository** due to size constraints.
Please download them using the links provided in the `/dataset` folder.

---

