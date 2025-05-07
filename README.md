
Flask Student CRUD App
=======================

This is a simple web application built with Flask that performs basic CRUD operations using SQLite and SQLAlchemy. The app allows you to add, view, update, and delete student records through a clean web interface.

Features
--------

- ✅ Add new students
- 📋 View all student records
- ✏️ Update student information
- ❌ Delete student entries
- 🧩 SQLite for persistent storage
- 🖥️ Jinja2 templates for rendering HTML

Technologies Used
-----------------

- Python 3
- Flask
- SQLAlchemy
- SQLite
- HTML/CSS (Jinja templates)

Getting Started
---------------

Follow these instructions to get the project up and running on your local machine.

### Prerequisites

- Python 3.x installed
- Git (optional, for cloning)
- A code editor (e.g. VSCode)

### 1. Clone the Repository

```
git clone https://github.com/Shaheer-Sheri/Flask_app.git
cd flask-student-crud
```

### 2. Create a Virtual Environment (optional but recommended)

```
python -m venv venv
source venv/bin/activate      # On Windows use: venv\Scripts\activate
```

### 3. Install Dependencies

```
pip install -r requirements.txt
```

### 4. Initialize the Database

Open Python shell:

```
python
```

Then run:

```
from app import db
db.create_all()
exit()
```

This will create a SQLite database file `firstapp.db`.

### 5. Run the Application

```
python app.py
```

Visit http://127.0.0.1:5000 in your browser.

File Structure
--------------

```
flask-student-crud/
│
├── app.py                 # Main Flask application
├── firstapp.db            # SQLite database (generated)
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
├── templates/             # HTML templates
│   ├── index.html
│   └── update.html
```

Routes Overview
---------------

| Route             | Method(s) | Description                          |
|------------------|-----------|--------------------------------------|
| `/`              | GET/POST  | Display form and list of students    |
| `/delete/<sno>`  | GET       | Delete a student by their ID         |
| `/update/<sno>`  | GET/POST  | Update student details               |
| `/home`          | GET       | Static welcome message               |

Example Student Fields
----------------------

- First Name
- Last Name
- Age
- City



