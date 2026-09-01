# 🍦 DarkScoop — Ice Cream Shop Web-Application

> A modern and responsive ice cream shop website built with **Django**, featuring flavour discovery, product presentation, user authentication, contact functionality, and a clean, engaging UI.

---

## 📌 Overview

**DarkScoop** is a Django-based ice cream shop web application designed to provide customers with an attractive and easy-to-use online experience.

The project focuses on combining a modern frontend with Django's backend capabilities, including reusable templates, database-driven content, authentication, and form handling.

The application was developed as a full-stack Django project to practice and demonstrate real-world web development concepts.

---

## ✨ Features

### 🍨 Ice Cream Flavours

* Browse available ice cream flavours
* Dedicated flavours page
* Display flavour name, description, and images
* Showcase latest/popular flavours
* Responsive flavour cards

### 🏠 Home Page

* Attractive hero section
* Ice cream shop introduction
* Featured flavours
* Call-to-action buttons
* Responsive design

### 👤 User Authentication

* User registration
* User login
* User logout
* Authentication-based user experience
* Protected actions for authenticated users

### 📩 Contact System

* Customer contact form
* Name, email, phone, subject, and message fields
* Contact information stored in the database
* Backend form validation

### 📱 Responsive UI

* Mobile-friendly layout
* Tablet support
* Desktop-friendly design
* Responsive navigation
* Bootstrap-based components

### 🎨 Modern Design

* Custom CSS styling
* Ice-cream themed colour palette
* Reusable base template
* Consistent navigation and footer
* Interactive buttons and cards

---

## 🛠️ Tech Stack

### Backend

* **Python**
* **Django**

### Frontend

* **HTML5**
* **CSS3**
* **Bootstrap**
* **JavaScript**

### Database

* **SQLite** *(development)*

### Development Tools

* Git
* GitHub
* VS Code
* Python Virtual Environment

---

## 🏗️ Project Structure

```text
DarkScoop/
│
├── manage.py
│
├── darkscoop/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── home/
│   ├── migrations/
│   ├── templates/
│   │   └── home/
│   │       ├── index.html
│   │       ├── about.html
│   │       ├── flavours.html
│   │       ├── contact.html
│   │       └── ...
│   │
│   ├── static/
│   │   └── home/
│   │       ├── css/
│   │       ├── js/
│   │       └── images/
│   │
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
│
├── db.sqlite3
│
├── requirements.txt
│
└── README.md
```

> Adjust the structure above if your actual Django app/project names are different.

---

# 🚀 Getting Started

Follow the steps below to run DarkScoop locally.

## 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/darkscoop.git
```

Navigate into the project:

```bash
cd darkscoop
```

---

## 2. Create a Virtual Environment

### Windows

```bash
python -m venv venv
```

Activate it:

```bash
venv\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

If you don't have a `requirements.txt` yet:

```bash
pip freeze > requirements.txt
```

---

## 4. Apply Migrations

```bash
python manage.py makemigrations
```

```bash
python manage.py migrate
```

---

## 5. Create a Superuser

To access the Django administration panel:

```bash
python manage.py createsuperuser
```

Follow the terminal instructions to create your admin account.

---

## 6. Run the Development Server

```bash
python manage.py runserver
```

The application will be available at:

```text
http://127.0.0.1:8000/
```

Django Admin:

```text
http://127.0.0.1:8000/admin/
```

---

# 📸 Screenshots

Add screenshots of your project here to make the repository more attractive to recruiters and developers.

### 🏠 Home Page

```text
![DarkScoop Home Page](screenshots/home.png)
```

### 🍨 Flavours Page

```text
![DarkScoop Flavours](screenshots/flavours.png)
```

### 📩 Contact Page

```text
![DarkScoop Contact](screenshots/contact.png)
```

### 🔐 Login Page

```text
![DarkScoop Login](screenshots/login.png)
```

> Recommended: create a `screenshots/` folder in your repository and place your actual screenshots there.

---

# 🎯 Main Pages

| Page        | Description                                         |
| ----------- | --------------------------------------------------- |
| 🏠 Home     | Landing page with hero section and featured content |
| 🍨 Flavours | Displays available ice cream flavours               |
| ℹ️ About    | Information about DarkScoop                         |
| 📩 Contact  | Customer contact form                               |
| 🔐 Login    | User authentication                                 |
| 📝 Register | New user registration                               |
| ⚙️ Admin    | Django administration panel                         |

---

# 🗄️ Database

DarkScoop uses Django's ORM for database interaction.

The project includes database functionality for features such as:

* User authentication
* Contact submissions
* Ice cream flavour data
* Administrative management

During development, **SQLite** is used as the default database.

---

# 🔐 Django Admin

DarkScoop uses Django's built-in administration system to manage application data.

Administrators can manage:

* Users
* Contact submissions
* Ice cream flavours
* Application data

Access the admin panel:

```text
http://127.0.0.1:8000/admin/
```

---

# 🧠 Django Concepts Demonstrated

This project demonstrates practical usage of several Django concepts:

* Django project structure
* Django applications
* URL routing
* Function-based views
* Django templates
* Template inheritance
* Static files
* Django models
* Django ORM
* Model migrations
* Django forms
* Form validation
* User authentication
* Django Admin
* Database integration
* Bootstrap integration
* Responsive design

---

# 🔄 Application Flow

```text
                 ┌─────────────────┐
                 │     Customer    │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │    DarkScoop    │
                 │    Homepage     │
                 └────────┬────────┘
                          │
             ┌────────────┼────────────┐
             ▼            ▼            ▼
        ┌─────────┐  ┌─────────┐  ┌─────────┐
        │Flavours │  │  About  │  │ Contact │
        └─────────┘  └─────────┘  └────┬────┘
                                       │
                                       ▼
                                ┌──────────────┐
                                │   Database   │
                                └──────────────┘
```

---

# 🔮 Future Improvements

The project can be extended with additional e-commerce functionality.

### 🛒 Shopping Features

* Shopping cart
* Add/remove products
* Quantity management
* Checkout system
* Order history

### 💳 Payments

* Online payment integration
* Payment confirmation
* Order payment status

### 📦 Order Management

* Order tracking
* Order status
* Customer order history
* Admin order management

### ⭐ Customer Features

* Product reviews
* Ratings
* Wishlist
* Favourite flavours

### 🔎 Advanced Features

* Search functionality
* Category filtering
* Price filtering
* Pagination
* Recommendation system

### 🚀 Deployment

* PostgreSQL database
* Environment variables
* Production settings
* Static file management
* Deployment using a cloud platform

---

# 📚 What I Learned

While building DarkScoop, I gained practical experience with:

* Building a Django application from scratch
* Designing reusable templates
* Working with Django models and migrations
* Connecting frontend forms with backend logic
* Implementing authentication
* Managing data through Django Admin
* Using Django ORM
* Organizing static files
* Building responsive web pages
* Debugging Django errors
* Structuring a real-world web application

---

# 👨‍💻 Author

**Chaitanya Modi**

Backend / Python Developer

* Python
* Django
* FastAPI
* REST APIs
* SQL
* PostgreSQL
* Git & GitHub

---

# 📄 License

This project is created for **educational and portfolio purposes**.

---

## ⭐ Support

If you found this project useful or interesting, consider giving the repository a ⭐ on GitHub.
