## ⚙️ Steps to Run the Project (NIDS)
### 1️⃣ Clone the Repository
git clone < your-github-rephttps://github.com/ShobhitDhuliya/NIDSository-link >
cd NIDS

### 2️⃣ Create and Activate Virtual Environment (Recommended)
python -m venv venv
venv\Scripts\activate   # Windows
source venv/bin/activate   # Linux / macOS

### 3️⃣ Install Required Dependencies
pip install numpy pandas seaborn matplotlib scikit-learn lightgbm xgboost tabulate optuna
✔ Tested on Python 3.12

### 4️⃣ Dataset Setup
Create a folder named MINI_NIDS inside the project directory and place the dataset files as shown below:
```text
NIDS/
│── MINI_NIDS/
│   │── Train_data.csv
│   │── Test_data.csv
│── nids.ipynb
│── README.md
```
Ensure the dataset paths in the code are correct:
train = pd.read_csv("MINI_NIDS/Train_data.csv")
test = pd.read_csv("MINI_NIDS/Test_data.csv")

### 5️⃣ Remove Google Colab Specific Code
Remove or comment out the following lines if present:
from google.colab import drive
drive.mount('/content/drive')

### 6️⃣ Run the Project
Using Jupyter Notebook (Recommended):
jupyter notebook
Open nids.ipynb and run all cells sequentially.
Or run as a Python script:
python nids.py

### ✅ Output
The project trains and evaluates multiple machine learning models for a Network Intrusion Detection System (NIDS) and reports Accuracy, Precision, Recall, F1-Score, Confusion Matrix, and performance comparison plots.
