# 🚌 Bus Reservation Management System

A full-stack **Bus Reservation Management System** built using **Python Django**, **HTML/CSS**, **Bootstrap**, and **MySQL**. This project offers an easy and intuitive interface to book bus tickets, view available routes, manage bookings, and handle administrative tasks securely.

---

## ⚙️ Tech Stack

- **Backend:** Python Django (MVC Framework)
- **Frontend:** HTML5, CSS3, Bootstrap 5
- **Database:** MySQL
- **Tools:** XAMPP / phpMyAdmin, VS Code / PyCharm
- **Other:** Django Templates, Static Files, Django Admin Panel

---

## ✨ Key Features

### 👤 User
- Register & Login
- View available buses and timings
- Book and cancel tickets
- View booking history

### 🛠️ Admin
- Secure login
- Add/Edit/Delete buses, routes, timings
- View all bookings and manage users
- Admin dashboard for analytics

---

## 🚀 Getting Started – Run Locally

### 🔽 Step 1: Clone the Repository

```bash
git clone https://github.com/Dipanshu-sandhaki/BUS-Reservation-Management-System.git
cd BUS-Reservation-Management-System
```

### 🧱 Step 2: Setup Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate     # On Windows
source venv/bin/activate  # On Linux/Mac
```

### 📦 Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

> If `requirements.txt` not available, install manually:

```bash
pip install django mysqlclient
```

### 🗂️ Step 4: Setup MySQL Database

1. Start **XAMPP** and go to **phpMyAdmin**
2. Create a database:
```sql
CREATE DATABASE bus_db;
```

3. In `settings.py`, update database config:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'bus_db',
        'USER': 'root',
        'PASSWORD': '',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

### ↺ Step 5: Apply Migrations & Create Superuser

```bash
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
```

### ▶️ Step 6: Run the Server

```bash
python manage.py runserver
```

- Open `http://127.0.0.1:8000/` to view the app  
- Admin login: `http://127.0.0.1:8000/admin/`

---

## 📁 Project Structure

```
BUS-Reservation-Management-System/
|
├── bus_app/               # Main Django app
│   ├── models.py          # DB Models
│   ├── views.py           # Logic & Controllers
│   ├── templates/         # HTML Templates
│   └── static/            # CSS, JS, Bootstrap
│
├── BusReservation/        # Django Project settings
│   └── settings.py        # Configurations
│
├── manage.py              # Django CLI
├── requirements.txt       # Python Dependencies
└── README.md              # Project Overview
```

---

## 🖼️ Screenshots (Add in `/screenshots` folder)

| Home Page | Booking Form | Admin Dashboard |
|-----------|--------------|-----------------|
| ![Home](screenshots/home.png) | ![Booking](screenshots/booking.png) | ![Admin](screenshots/admin.png) |

---

## 🔧 Future Enhancements

- ✉️ Email confirmations for bookings
- 📲 Mobile responsive UI
- 💳 Payment gateway integration
- 🧾 PDF ticket download
- 📊 Admin analytics dashboard

---

## 🙋‍♂️ About Me

**Dipanshu Sandhaki**  
🎓 MCA Student | Aspiring Full Stack Developer  
🌍 Based in Dehradun, India  
📨 [LinkedIn](https://www.linkedin.com/in/dipanshusandhaki)

---

## ⭐ Show Some Love

If you like this project:

- ⭐ Star this repo
- 🛠 Fork and use it
- 🐛 Report bugs or suggest features
- 📢 Share it with others!

---

## 📜 License

This project is licensed under the [MIT License](LICENSE)
