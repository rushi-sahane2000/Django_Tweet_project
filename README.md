🐦 Django Tweet App

A simple Tweet application built using Django that allows users to create, view, update, and delete tweets.
This project demonstrates CRUD operations, Django templates, forms handling, and database integration.

📌 Features

📝 Create a new tweet

📋 View all tweets

✏️ Edit existing tweet

❌ Delete tweet

📸 Image upload support (if implemented)

🔐 CSRF protection

🛠 Django Admin panel

🛠 Tech Stack

Backend: Django (Python)

Database: SQLite

Frontend: HTML, CSS, Bootstrap

Version Control: Git

📂 Project Structure
tweet_project/
│
├── tweetapp/
│   ├── migrations/
│   ├── templates/
│   ├── models.py
│   ├── views.py
│   ├── forms.py
│   ├── urls.py
│
├── tweet_project/
│   ├── settings.py
│   ├── urls.py
│
├── manage.py
├── db.sqlite3
└── README.md

⚙️ Installation Guide
1️⃣ Clone Repository
git clone https://github.com/your-username/tweet-app.git
cd tweet-app

2️⃣ Create Virtual Environment
python -m venv venv


Activate environment:

Windows

venv\Scripts\activate


Linux/Mac

source venv/bin/activate

3️⃣ Install Dependencies
pip install django


(Or install from requirements.txt if available)

4️⃣ Run Migrations
python manage.py makemigrations
python manage.py migrate

5️⃣ Create Superuser
python manage.py createsuperuser

6️⃣ Start Server
python manage.py runserver


Visit:

Main App → http://127.0.0.1:8000/

Admin Panel → http://127.0.0.1:8000/admin/

🧩 Example Model
from django.db import models

class Tweet(models.Model):
    text = models.TextField(max_length=280)
    created_at = models.DateTimeField(auto_now_add=True)

    def __str__(self):
        return self.text[:20]

🎯 What I Learned

Django project structure

Models & ORM

URL routing

Templates & Forms

CRUD operations

Admin customization

🚀 Future Improvements

User authentication system

Like & comment feature

Pagination

REST API using Django REST Framework

Deployment on cloud

👨‍💻 Author

Rushikesh Sahane
Final Year BE Computer Engineering Student
Focused on Backend Development & Problem Solving 🚀
