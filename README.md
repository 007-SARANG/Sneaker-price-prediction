

# 👟 The Price Prediction of Sneakers Based on Machine Learning

A full-stack Django web application that predicts sneaker prices using machine learning techniques. This platform allows users and admins to upload sneaker data, visualize pricing trends, and make intelligent price predictions based on historical data.



## 🔍 Project Overview

**Sneaker Price Prediction** is a Django-based web app that enables users to forecast sneaker prices using machine learning. With a focus on user-friendly data interaction, it provides visual insights into sneaker trends and pricing, while also allowing admins to manage uploaded datasets.



## ✨ Features

- 🔐 User registration & authentication (user/admin roles)
- 📂 Upload and manage sneaker datasets (CSV format)
- 📈 Visualize sneaker price trends by region, model, and date
- 🤖 Predict sneaker prices using trained ML models
- 📊 Interactive and responsive data dashboards
- 💻 Mobile-friendly interface with modern UI (Bootstrap-based)

---

## 🛠️ Tech Stack

| Layer         | Tools Used                           |
|---------------|---------------------------------------|
| Frontend      | HTML, CSS, Bootstrap 5                |
| Backend       | Python, Django                        |
| ML & Data     | Pandas, NumPy, Scikit-learn           |
| Database      | SQLite                                |
| Visualization | Matplotlib, Seaborn                   |
| Templates     | Django Templating Engine              |



## ⚙️ Installation

### 🔧 Prerequisites

- Python 3.8+
- pip
- virtualenv (recommended)

### 🔌 Setup Instructions

1. **Clone the repository**
```bash
   git clone https://github.com/007-SARANG/Sneaker-price-prediction.git
   cd sneaker-price-prediction/price\ prediction
   ```


3. **Create a virtual environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

4. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

5. **Apply migrations**

   ```bash
   python manage.py migrate
   ```

6. **Run the server**

   ```bash
   python manage.py runserver
   ```

7. **Access the app**
   Open your browser and visit: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

---

## 🚀 Usage

* Register or log in as a user/admin.
* Upload sneaker price datasets (in CSV format).
* Navigate to the dashboard to explore trends.
* Use the prediction interface to get estimated prices based on model, release date, and region.

---

## 📊 Machine Learning Model

* **Dataset**: [StockX Sneaker Data 2019 (Kaggle)](https://www.kaggle.com/datasets/stockx/stockx-sneaker-data-2019)
* **Model Used**: `RandomForestRegressor`, trained in `users/views.py`
* **Target Variable**: `Sale Price`
* **Features used by the implementation**: order date, brand, sneaker name, retail price, release date, shoe size, and buyer region
* **Evaluation shown by the app**: MAE, MSE, and RMSE from an 80/20 random split; split and forest seeds are fixed to 42

The model is fit from the uploaded/local CSV during each training or prediction request; a trained model is not persisted. The split is random rather than time-based, so these metrics are an exploratory holdout result and do not establish performance on future market data. The repository does not include a separate `ml_model/` training package.



---

## 🧑‍💻 Contributing

Contributions are welcome!

1. Fork the repo
2. Create a new branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add feature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a pull request ✅

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙌 Acknowledgements

* [Django](https://www.djangoproject.com/)
* [BootstrapMade Arsha Template](https://bootstrapmade.com/arsha-free-bootstrap-html-template-corporate/)
* [StockX Dataset - Kaggle](https://www.kaggle.com/datasets/stockx/stockx-sneaker-data-2019)
* [Scikit-learn](https://scikit-learn.org/)
* [Matplotlib](https://matplotlib.org/)

---

### 🔗 Connect with the Developer

**Sahithi Nandikula**
🌐 [GitHub](https://github.com/sahithinandikula)
📬 Open for collaborations and feedback!

```

