**This project implements a Machine Learning–based Network Intrusion Detection System (NIDS) that classifies network traffic as Normal or Anomaly using supervised learning algorithms.**

Steps to 
**1️⃣ Clone the Repository**
   git clone <your-github-repository-link>
   cd NIDS

**2️⃣ Create and Activate Virtual Environment (Recommended)**
    python -m venv venv
    
  **Activate the virtual environment**
   **Windows**
     venv\Scripts\activate
  **Linux / macOS**
  source venv/bin/activate
  
**3️⃣ Install Required Dependencies**
  pip install numpy pandas seaborn matplotlib scikit-learn lightgbm xgboost tabulate optuna

**4️⃣ Dataset Setup**
Create a folder named MINI_NIDS inside the project directory and place the dataset files as shown:
NIDS/
│── MINI_NIDS/
│   │── Train_data.csv
│   │── Test_data.csv
│── nids.ipynb
│── README.md

**Update dataset paths if required:**
train = pd.read_csv("MINI_NIDS/Train_data.csv")
test = pd.read_csv("MINI_NIDS/Test_data.csv")

**5️⃣ Remove Google Colab Specific Code**
This project is meant to run locally, so remove or comment out the following lines:
from google.colab import drive
drive.mount('/content/drive')

**6️⃣ Run the Project**
**Option A: Jupyter Notebook (Recommended)**
  jupyter notebook
  Open nids.ipynb and run all cells sequentially.
 
**Option B: Python Script**
  If converted to a script:
  python nids.py
