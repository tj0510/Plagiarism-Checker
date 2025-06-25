# Plagiarism-Checker 🕵️

This project is a simple Python-based plagiarism checker that compares multiple `.txt` files in a folder using **TF-IDF vectorization** and **cosine similarity**. It's ideal for detecting content similarity in student assignments, research papers, or text-based documents.

## 🚀 Features

- Reads all `.txt` files in the current directory.
- Uses **TF-IDF (Term Frequency-Inverse Document Frequency)** for vectorizing the text.
- Calculates **cosine similarity** between every pair of files.
- Outputs similarity scores and identifies potentially plagiarized document pairs.

## 🧠 Technologies Used

- Python 🐍
- scikit-learn (for TF-IDF and cosine similarity)
- OS module (for file handling)

## 🗂️ How It Works

1. All `.txt` files in the directory are read.
2. Each file’s text is converted into a numerical vector using `TfidfVectorizer`.
3. Cosine similarity is computed between each pair of documents.
4. Results with high similarity are flagged as potentially plagiarized.

## 🛠️ Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/plagiarism-checker.git
   cd plagiarism-checker
   ```

2. Install dependencies:
   ```bash
   pip install scikit-learn
   ```

3. Add the `.txt` files you want to check into the project folder.

4. Run the script (from a Jupyter Notebook or a Python file):
   ```bash
   python plagcheck.py
   ```

   *(Or open and run the notebook file: `Copy_of_plagcheck.ipynb`)*

## 📄 Example Output

```
[student1.txt] <--> [student2.txt]: Similarity = 0.87
[student3.txt] <--> [student5.txt]: Similarity = 0.92
```

## 📌 Notes

- The script checks all pairs of `.txt` files. Ensure each file contains clean and meaningful text.
- Results are based on cosine similarity; a higher value (close to 1) indicates more similarity.

## 🧑‍💻 Author

- **Your Name** ([@yourusername](https://github.com/yourusername))

## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
