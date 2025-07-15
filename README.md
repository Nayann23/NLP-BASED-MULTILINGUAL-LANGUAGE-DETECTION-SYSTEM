# NLP-BASED MULTILINGUAL LANGUAGE DETECTION SYSTEM

## 📁 Project Structure

```
nlp-language-detection-system/
│
├── language.csv                # Dataset with text samples and language labels
├── LANGUAGE-DETECTION.ipynb    # Main Jupyter Notebook
├── README.md                   # Project documentation
```

---

## 📝 Dataset

The project uses a `language.csv` file containing two columns:

- **Text**: A sample sentence or phrase  
- **Language**: The language in which the text is written

### Example:

```csv
Text,Language
"Bonjour, comment ça va ?",French
"Hello, how are you?",English
"¿Cómo estás?",Spanish
```

---

## 🚀 Getting Started

### 1. Clone the repository:

```bash
git clone https://github.com/Nayann23/NLP-BASED-MULTILINGUAL-LANGUAGE-DETECTION-SYSTEM.git
cd nlp-language-detection-system
```

### 2. Install dependencies:

```bash
pip install numpy pandas scikit-learn
```

### 3. Open and run the notebook:

You can open the notebook using Jupyter or VS Code:

```bash
jupyter notebook LANGUAGE-DETECTION.ipynb
```

Or in VS Code:

- Open the project folder
- Click on `LANGUAGE-DETECTION.ipynb`
- Run cells step by step

---

## 👨‍💻 How It Works

- Loads and preprocesses the dataset.
- Transforms the text using `CountVectorizer`.
- Splits the data into training and testing sets.
- Trains a `Multinomial Naive Bayes` classifier.
- Accepts user input and predicts the language.
- Loops until the user types `"Stop"`.

---

## 📈 Model Accuracy

The model provides an accuracy score on the test data after training.  
This can be improved by:

- Adding more data samples per language
- Using more advanced NLP techniques (e.g., TF-IDF, word embeddings)

---

## ✅ Example Output

```bash
Enter Text To Detect Language: Hallo, wie geht's?
Your text 'Hallo, wie geht's?.' Written in  German Language

Enter Text To Detect Language: Stop
```

---

## 🔧 Future Enhancements

- Add support for more languages
- Improve model with deep learning (e.g., LSTM, BERT)
- Build a web interface using Flask or Streamlit
- Deploy as an API for integration
