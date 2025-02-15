# Django Food Ordering System 🍔

A full-stack food ordering web application built with Django. Manage menus, process orders, and track user interactions.

## Features ✨
- **User Authentication**: Sign up, login, and profile management.
- **Menu Management**: Add/update food items with prices and descriptions.
- **Cart System**: Add items to cart and modify quantities.
- **Order Tracking**: View order history and status.
- **Admin Dashboard**: Manage users, menus, and orders.
- **Responsive Design**: Works on mobile and desktop.

---

## Prerequisites 📋
- Python 3.8+
- Django 4.0+
- PostgreSQL
- Git

---

## Installation 🛠️

### 1. Clone the Repository
```bash
git clone https://github.com/kalp12/Food-ordering-django.git
cd Food-ordering-django
```
### 2. Set Up Virtual Environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate    # Windows
### 3. Install Dependencies
pip install -r requirements.txt
### 4. Configure Database
Create .env file:

env

SECRET_KEY='your_django_secret_key'
DEBUG=True
DATABASE_URL='postgres://user:password@localhost/dbname'
### 5. Run Migrations

python manage.py migrate
### 6. Create Superuser (Admin)

python manage.py createsuperuser
### 7. Run Development Server

python manage.py runserver
Visit http://localhost:8000

### Project Structure 📂

        Food-ordering-django/
        ├── core/               # Main Django app
        │   ├── models.py       # Database models
        │   ├── views.py        # Business logic
        │   └── admin.py        # Admin panel config
        ├── templates/          # HTML templates
        │   ├── menu.html       # Food menu
        │   └── checkout.html   # Order page
        ├── static/             # CSS/JS/Images
        ├── manage.py           # Django CLI
        └── requirements.txt    # Dependencies

### Deployment 🚀
Deploy to Heroku:

```bash
heroku create your-app-name
heroku addons:create heroku-postgresql:hobby-dev
git push heroku main
