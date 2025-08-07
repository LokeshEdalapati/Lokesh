# Chronic Illness Prediction System

This project is a Django-based web application that predicts the risk of chronic illnesses such as diabetes, hypertension, and heart disease using machine learning models. It enables users to input medical data through a web form and receive predictive results in real time.

---

##  Features

-  Predicts chronic disease risks using classification models
-  Machine Learning with Scikit-learn
-  Input validation & SQL injection protection
-  Simple web interface for user interaction
-  Backend tested with real-world sample data

---

##  Technologies Used

- **Backend**: Django (Python)
- **Frontend**: HTML, CSS (Django templates)
- **Machine Learning**: Scikit-learn
- **Database**: MySQL
- **Tools**: Git, GitHub

---

##  Project Structure

Chronic_Diseases_Prediction/
├── manage.py
├── requirements.txt
├── templates/
├── static/
├── prediction/
│ ├── models.py
│ ├── views.py
│ ├── urls.py
├── ML_Model/
│ └── model.pkl
├── db.sqlite3 or MySQL (connected)
└── README.md
Setup Instructions (Local Development)

 1.  Clone the Repository

git clone https://github.com/LokeshEdalapati/Lokesh.git
cd Lokesh
2.  Create Virtual Environment (Optional but recommended)
python -m venv env
env\Scripts\activate  # Windows
3.  Install Dependencies
pip install -r requirements.txt
4.  Configure MySQL in settings.py
Make sure your database settings look like this:
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'your_db_name',
        'USER': 'root',
        'PASSWORD': '',
        'HOST': '127.0.0.1',
        'PORT': '3306',
    }
}
5.  Run Migrations
python manage.py makemigrations
python manage.py migrate
6.  Create Superuser (for admin login)
python manage.py createsuperuser
7. ▶ Run the Server
python manage.py runserver
Visit http://127.0.0.1:8000/ in your browser to use the app.
