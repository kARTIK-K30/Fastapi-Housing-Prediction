# 🏡 FastAPI Housing Price Prediction

### Machine Learning Powered Real Estate Valuation System

A machine learning-based web application that predicts house prices using property features such as area, bedrooms, bathrooms, parking, furnishing status, and available amenities.

Built using **Python, FastAPI, Scikit-learn, HTML, and CSS**, this project integrates a trained Linear Regression model with a responsive web interface to provide estimated property valuations.

---

## 🚀 Project Overview

The objective of this project is to develop an intelligent housing price prediction system that estimates property prices based on multiple property characteristics.

Instead of manually entering training data, the application uses a real-world housing dataset from Kaggle containing 545 records and 13 columns.

The machine learning model learns relationships between property features and housing prices to generate predictions for new property inputs.

---

## ✨ Key Features

- **Machine Learning Prediction:** Uses Linear Regression to estimate house prices.
- **Real-World Dataset:** Trained using a Kaggle housing prices dataset.
- **Interactive Web Interface:** User-friendly property information form.
- **Multiple Property Features:** Considers 12 input features.
- **Categorical Data Processing:** Uses One-Hot Encoding for categorical variables.
- **FastAPI Backend:** Handles requests and generates predictions.
- **Responsive Frontend:** HTML and CSS-based interface.
- **API Documentation:** Interactive Swagger UI.

---

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Backend Framework | FastAPI |
| Machine Learning | Scikit-learn |
| Data Processing | Pandas, NumPy |
| Model Serialization | Joblib |
| Frontend | HTML, CSS |
| Template Engine | Jinja2 |
| Server | Uvicorn |
| Dataset | Kaggle Housing Prices Dataset |

---

## 📊 Dataset Information

**Dataset:** Housing Prices Dataset by Yasser H.

The dataset contains:

- 545 records
- 13 columns
- 12 input features
- 1 target variable (`price`)

### Input Features

| Feature | Description |
|---|---|
| area | Property area |
| bedrooms | Number of bedrooms |
| bathrooms | Number of bathrooms |
| stories | Number of stories |
| parking | Available parking spaces |
| mainroad | Main road access |
| guestroom | Guest room availability |
| basement | Basement availability |
| hotwaterheating | Hot water heating facility |
| airconditioning | Air conditioning availability |
| prefarea | Preferred area |
| furnishingstatus | Furnishing condition |

**Target Variable:** `price`

---

## 🧠 Machine Learning Workflow

The project follows these steps:

1. Load the housing dataset using Pandas.
2. Separate input features and target variable.
3. Identify numerical and categorical columns.
4. Apply One-Hot Encoding to categorical features.
5. Build a Scikit-learn machine learning pipeline.
6. Split the dataset into training and testing sets.
7. Train the Linear Regression model.
8. Evaluate predictions using MAE and R² Score.
9. Save the trained model using Joblib.
10. Integrate the model with FastAPI for real-time predictions.

### Model Configuration

- Algorithm: Linear Regression
- Training Data: 80%
- Testing Data: 20%
- Random State: 42
- Encoding: One-Hot Encoding
- Evaluation Metrics: Mean Absolute Error (MAE) and R² Score

---

## 📁 Project Structure

```text
Fastapi-Housing-Prediction/
│
├── data/
│   └── Housing.csv
│
├── models/
│   └── house_model.pkl
│
├── templates/
│   └── index.html
│
├── static/
│   └── style.css
│
├── train_model.py
├── main.py
├── requirements.txt
├── .gitignore
└── README.md
```

---

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/kARTIK-K30/Fastapi-Housing-Prediction.git
```

### 2. Navigate to the Project Directory

```bash
cd Fastapi-Housing-Prediction
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate the Virtual Environment

**Windows PowerShell:**

```powershell
.\venv\Scripts\Activate.ps1
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Download the Dataset

Download the Housing Prices Dataset from Kaggle.

Place the downloaded CSV file inside the `data` folder:

```text
data/Housing.csv
```

### 7. Train the Machine Learning Model

```bash
python train_model.py
```

After successful training, the model will be saved at:

```text
models/house_model.pkl
```

### 8. Start the FastAPI Server

```bash
python -m uvicorn main:app --reload
```

---

## 🌐 Application URLs

Once the server starts, access the application using:

| Resource | URL |
|---|---|
| Web Application | http://127.0.0.1:8000/ |
| Swagger API Documentation | http://127.0.0.1:8000/docs |
| ReDoc Documentation | http://127.0.0.1:8000/redoc |

---

## 🔍 How It Works

1. Open the web application.
2. Enter the property's area and structural details.
3. Select the available amenities.
4. Choose the furnishing status.
5. Click on **Generate Property Valuation**.
6. The FastAPI backend receives the submitted information.
7. The trained machine learning model processes the input.
8. The predicted house price is displayed on the webpage.

---

## 📈 Model Evaluation

The model is evaluated using:

- **Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted prices.
- **R² Score:** Measures how well the model explains variations in housing prices.

Actual evaluation scores are generated when `train_model.py` is executed.

---

## 🔮 Future Enhancements

- Experiment with advanced regression algorithms such as Random Forest and XGBoost.
- Improve prediction accuracy through hyperparameter tuning.
- Add interactive data visualization.
- Deploy the application on a cloud platform.
- Integrate a database to store prediction history.
- Add user authentication and personalized dashboards.
- Provide property valuation insights and market comparisons.

---

## 👨‍💻 Developer

**Kartik Kumar**

B.Tech – Data Science

GitHub: [@kARTIK-K30](https://github.com/kARTIK-K30)

Project Repository: [FastAPI Housing Price Prediction](https://github.com/kARTIK-K30/Fastapi-Housing-Prediction)

---

## ⭐ Support

If you find this project interesting or useful, consider giving the repository a ⭐ on GitHub!

**Built with Python, Machine Learning, and FastAPI.**
