# PolyMind

**PolyMind** is a machine learning-powered web application designed to help businesses forecast sales, predict demand, and implement intelligent dynamic pricing strategies. Built with Django and Streamlit, the project integrates advanced predictive models and dynamic dashboards to deliver actionable retail insights.

## 🚀 Features

- 🔮 **Sales Forecasting** – Predict future sales based on historical trends, calendar events, and business activity.  
- 📦 **Demand Prediction** – Estimate demand with features like promotions, seasonality, holidays, and store-specific data.  
- 💰 **Dynamic Pricing** – Recommend optimized prices that maximize revenue while respecting demand elasticity.  
- 🌐 **Interactive Website** – A Django-powered interface for inputting parameters and retrieving model predictions.  
- 📊 **Streamlit Dashboards** – Visualize trends, forecasts, and pricing recommendations through dynamic dashboards.

## 🛠️ Technologies Used

- **Backend:** Django (Python Web Framework)  
- **Frontend:** HTML, CSS, JavaScript, Bootstrap  
- **ML Libraries:** XGBoost, Scikit-learn, Pandas, NumPy  
- **Dashboards:** Streamlit  
- **Model Integration:** `pickle` for model loading in Django and Streamlit  
- **Database:** PostgreSQL (for local development and prototyping)  
- **Visualization:** Matplotlib, Seaborn (in notebooks and reports)

## 📁 Project Structure

PolyMind/
├── deployment/ # Django backend and frontend
│ ├── manage.py
│ ├── requirements.txt
│ └── ...
├── streamlit_app/ # Streamlit dashboard interface
│ └── app.py
├── notebooks/ # Jupyter notebooks for model building
│ ├── model_training.ipynb
│ ├── data_preprocessing.ipynb
│ └── dynamic_pricing.ipynb
├── documentation/ # Report and presentation
│ └── project_report.pdf
├── data/ # Raw and processed datasets (add your own)
│ └── ...
├── README.md

bash
Copy
Edit

## ⚙️ Installation & Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/MohamedAbdelhamid-22/DEPI_Project.git
   cd DEPI_Project
Create and Activate a Virtual Environment


python -m venv venv
source venv/bin/activate     # On Windows: venv\Scripts\activate
Install Dependencies


pip install -r deployment/requirements.txt
Run Django App


python deployment/manage.py migrate
python deployment/manage.py runserver
Run Streamlit Dashboard


cd streamlit_app
streamlit run app.py
Open in Browser

Django Web App: http://127.0.0.1:8000/

Streamlit Dashboard: usually at http://localhost:8501/

## 📊 Dynamic Pricing Module
The application includes a dynamic pricing engine that adjusts prices based on:

📈 Forecasted Demand

🧮 Price Elasticity Estimates

📦 Inventory Levels

📆 Seasonal and Promotional Factors

The pricing model outputs optimal values that maximize revenue without negatively affecting demand, simulating real-world business responsiveness.

🧠 Machine Learning Model
Algorithm: XGBoost Regressor

Serialized Using: pickle

Training Data: Includes item metadata, holidays, store info, promotions, and dates

Pipeline Integrity: Feature preprocessing (scaling, encoding) reused in production

🧪 How to Use
🌐 Django Website

Input form collects forecasting parameters (e.g., item type, store, date)

Results page displays predicted sales and suggested prices

📈 Streamlit Dashboard

Visualize demand forecasts, pricing trends, and performance summaries

📂 Upload the Dataset
To test the system click here to upload the dataset

https://drive.google.com/drive/folders/1xm83NomBq76rEK9Ha4RcsPvT38cwP5CW

🛡️ Challenges and Solutions
Cross-Environment Compatibility: Aligned Python versions and library dependencies between Jupyter and Django.

Consistent Feature Engineering: Exported transformers for reuse.

Categorical Input Handling: Used dropdown menus mapped to encoded variables.

Pricing Logic: Modeled pricing constraints and elasticity with domain assumptions.

🚧 Future Improvements
☁️ Deploy on Heroku or AWS

🧠 Auto-ML model retraining and evaluation pipeline

📈 Add export options for dashboards and prediction results

🤝 Contributing
We welcome contributions! If you'd like to help improve PolyMind, please fork the repo and open a pull request.
For large changes, open an issue to discuss what you'd like to contribute.

📬 Contact
GitHub: MohamedAbdelhamid-22

Built as part of the Digital Egypt Pioneers Initiative to demonstrate real-world applications of AI in business intelligence.
