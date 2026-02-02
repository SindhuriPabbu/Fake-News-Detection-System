## Fake News Detection System
A machine learning system that detects fake news using multiple classifiers (Logistic Regression, Decision Tree, Gradient Boosting, Random Forest) with **TF-IDF vectorization**. Achieves high accuracy on news article classification.

## ✨ Features
* 4 ML Classifiers compared side-by-side
* TF-IDF Vectorization for text preprocessing
* Interactive testing - test any news article instantly
* Manual test set for validation
* Clean preprocessing pipeline (removes URLs, punctuation, numbers)

## 🛠️ Tech Stack
```
Python 3.x
├── pandas           # Data manipulation
├── scikit-learn     # ML algorithms & metrics
├── numpy            # Numerical operations
└── re/string        # Text preprocessing
```
## 📦 Installation
1. Clone the repository
```
git clone <repo-url>
```
2. Install dependencies
```
pip install pandas scikit-learn numpy
```
3. Download datasets
```
📥 Place Fake.csv and True.csv in project root
Datasets: Kaggle Fake News Dataset
```
4. Run the detector
```
python fakeNewsDetection.py
```
## 🚀 Quick Start
```
1. Run: python fakeNewsDetection.py
2. Enter any news headline/article when prompted
3. Get predictions from ALL 4 models instantly!
```
```
Example input:
"Scientists discover new species of fish in Pacific Ocean"
```
Sample Output:
```
LR Prediction: Not A Fake News 
DT Prediction: Not A Fake News 
GBC Prediction: Not A Fake News 
RFC Prediction: Not A Fake News
```
## 📊 Model Performance
| Model  | Key Strength | Typical Accuracy |
| ------------- |:-------------:|:-------------:|
| Logistic Regression |	Fastest inference |	~98%
|Decision Tree	|Interpretable	| ~97% |
| Gradient Boosting | High accuracy |	~99% |
| Random Forest | Robust ensemble |	~99% |

## 🔍 How It Works
```
1. Text Preprocessing → wordopt()
   ↓ Removes: URLs, punctuation, numbers, special chars
2. TF-IDF Vectorization
3. Train 4 Classifiers on 44K+ news articles
4. Predict: Fake News (0) or Real News (1)
```
📁 File Structure
```
fakeNewsDetection.py     # Main ML pipeline
├── Fake.csv             # fake news articles
├── True.csv             # real news articles
└── README.md            # You're reading it!
```
## 🎯 Usage Example
```
# After training, test any news:
news = "Government announces new tax reforms next month"
manual_testing(news)
# Output: All models predict "Not A Fake News"
```
## 🔮 Future Enhancements
* Web UI (Streamlit/Flask)
 * BERT/Transformer models
 * Real-time API endpoint
 * Cross-validation
 * Model persistence (joblib)

## 🤝 Contributing
1. Fork the repository
2. Create feature branch (git checkout -b feature/bert-model)
3. Commit changes (git commit -m 'Add BERT model')
4. Push (git push origin feature/bert-model)
5. Open Pull Request

