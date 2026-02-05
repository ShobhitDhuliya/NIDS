**This project implements a Machine Learning–based Network Intrusion Detection System (NIDS) that classifies network traffic as Normal or Anomaly using supervised learning algorithms.** 

⚙️ Steps to Run the Project

1️⃣ Clone the Repository
Bash
git clone <your-github-repository-link>
cd NIDS

2️⃣ Create and Activate Virtual Environment (Recommended)
Bash
python -m venv venv
Activate the virtual environment
Windows
Bash
venv\Scripts\activate
Linux / macOS
Bash
source venv/bin/activate
3️⃣ Install Required Dependencies

Bash
pip install numpy pandas seaborn matplotlib scikit-learn lightgbm xgboost tabulate optuna
✔ Tested on Python 3.12

4️⃣ Dataset Setup
Create a folder named MINI_NIDS inside the project directory and place the dataset files as shown:

NIDS/
│── MINI_NIDS/
│   │── Train_data.csv
│   │── Test_data.csv
│── nids.ipynb
│── README.md
Update dataset paths if required:
Python
train = pd.read_csv("MINI_NIDS/Train_data.csv")
test = pd.read_csv("MINI_NIDS/Test_data.csv")

5️⃣ Remove Google Colab Specific Code
This project is meant to run locally, so remove or comment out the following lines:
Python
from google.colab import drive
drive.mount('/content/drive')

6️⃣ Run the Project
Option A: Jupyter Notebook (Recommended)
Bash
jupyter notebook
Open nids.ipynb and run all cells sequentially.
Option B: Python Script
If converted to a script:
Bash
python nids.py
