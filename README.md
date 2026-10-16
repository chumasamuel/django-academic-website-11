# PRACTICAL 11

## Django Web Application – Course Management System

**Student:** Samuel Fernando Chuma
**Register Number:** 19
**Practical:** 11
**Technology:** Django
**Language:** Python
**Mode:** Individual

---

## Aim

To develop a web application using Django framework with templates, URL routing, views, models and database integration.

---

## Learning Objectives

* Understand the basic structure of a Django project.
* Create and configure a Django application.
* Implement URL routing.
* Create Django views.
* Use HTML templates with Django.
* Display course information dynamically.
* Understand Django models and database operations.
* Run and test a Django application using the development server.

---

## Technologies Used

* Python
* Django 5.2.17
* HTML5
* CSS3
* SQLite
* Visual Studio Code

---

## Project Structure

```text
PRACTICAL_11/
│
├── manage.py
│
├── practical11/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
└── courses/
    ├── migrations/
    ├── templates/
    │   └── courses/
    │       ├── home.html
    │       ├── courses.html
    │       └── contact.html
    │
    ├── __init__.py
    ├── admin.py
    ├── apps.py
    ├── models.py
    ├── tests.py
    ├── urls.py
    └── views.py
```

---

## Main Features

### 1. Home Page

The home page introduces the Course Management System and provides navigation to the other pages.

### 2. Courses Page

The courses page displays available courses using Django templates.

### 3. Contact Page

The contact page provides basic contact information for the department.

### 4. Django URL Routing

Separate URL patterns are used to connect browser requests with the appropriate Django views.

### 5. Django Templates

HTML pages are stored inside:

```text
courses/templates/courses/
```

The templates are rendered using Django's template system.

### 6. Django Application

The main application is called:

```text
courses
```

It is registered in the Django project's `INSTALLED_APPS`.

---

## Installation

Open the project folder in Visual Studio Code.

Open the terminal and run:

```bash
python -m pip install django
```

Check the installed Django version:

```bash
python -m django --version
```

Expected version:

```text
5.2.17
```

---

## Running the Project

Navigate to the folder containing `manage.py`:

```bash
cd "D:\Samuel Chuma\PRACTICAL_11"
```

Run the Django development server:

```bash
python manage.py runserver
```

The application will be available at:

```text
http://127.0.0.1:8000/
```

Open the address in a web browser.

---

## Important URLs

| Page    | URL         |
| ------- | ----------- |
| Home    | `/`         |
| Courses | `/courses/` |
| Contact | `/contact/` |
| Admin   | `/admin/`   |

---

## Database

Django uses SQLite as the default database for this practical.

The database file is:

```text
db.sqlite3
```

Django database migrations can be applied using:

```bash
python manage.py makemigrations
python manage.py migrate
```

---

## Creating an Administrator

To create a Django administrator account, run:

```bash
python manage.py createsuperuser
```

Follow the instructions shown in the terminal.

After creating the account, access:

```text
http://127.0.0.1:8000/admin/
```

---

## Testing

The project can be tested using:

```bash
python manage.py test
```

The Django development server can also be used to verify the different pages and navigation links.

---

## Expected Result

The Django application should successfully display:

* Home page
* Courses page
* Contact page
* Navigation between pages
* Course information
* Django admin interface
* SQLite database integration

---

## Conclusion

This practical demonstrates the fundamentals of developing a web application using Django. It provides practical experience with Django project structure, applications, URL routing, views, templates, database migration and the Django administration interface.
