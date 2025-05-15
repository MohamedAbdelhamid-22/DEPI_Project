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

```
PolyMind/
├── deployment/ # Django backend and frontend
│   ├── manage.py
│   ├── requirements.txt
│   └── ...
├── streamlit_app/ # Streamlit dashboard interface
│   └── app.py
├── notebooks/ # Jupyter notebooks for model building
│   ├── model_training.ipynb
│   ├── data_preprocessing.ipynb
│   └── dynamic_pricing.ipynb
├── documentation/ # Report and presentation
│   └── project_report.pdf
├── data/ # Raw and processed datasets (add your own)
│   └── ...
└── README.md
```

## ⚙️ Installation & Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/MohamedAbdelhamid-22/DEPI_Project.git
   cd DEPI_Project
   ```

2. **Set Up Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Application**
   - For Django backend:
     ```bash
     cd deployment
     python manage.py runserver
     ```
   - For Streamlit dashboard:
     ```bash
     cd streamlit_app
     streamlit run app.py
     ```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

You can now copy this entire block and paste it directly into your `README.md` file. The formatting will be preserved when viewed on GitHub or any Markdown viewer.
