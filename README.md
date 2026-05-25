# 📚 Bookstore Management System (Python)

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge\&logo=python)
![Tkinter](https://img.shields.io/badge/GUI-Tkinter-orange?style=for-the-badge)
![SQLite](https://img.shields.io/badge/Database-SQLite-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Project-Learning%20Project-lightgrey?style=for-the-badge)

---

## 📌 Overview

This is a simple **Bookstore Management System** built using **Python Tkinter (GUI)** and **SQLite (Database)**.

It allows users to perform basic CRUD operations on a book database through a graphical interface.

---

## 🖥️ Features

* 📖 Add new book records
* 🔍 Search books by Title, Author, Year, or ISBN
* 📋 View all stored books
* ✏️ Update selected book details
* ❌ Delete selected book
* 💾 Persistent storage using SQLite database

---

## 🏗️ Project Structure

```text id="bs1"
Bookstore/
│
├── backendinterface.py   # SQLite database operations
├── frontend.py          # Tkinter GUI application
├── books.db             # SQLite database (auto-generated)
└── README.md
```

---

## ⚙️ Tech Stack

* Python 3.x
* Tkinter (GUI framework)
* SQLite3 (Database)

---

## 🧠 How It Works

### 1. Backend (SQLite)

The backend handles all database operations:

* Create table (`book`)
* Insert records
* View all records
* Search records
* Update records
* Delete records

### 2. Frontend (Tkinter GUI)

The UI allows users to interact with the system:

* Input fields for book details
* Listbox to display records
* Buttons for CRUD operations

---

## 🗄️ Database Schema

```sql id="bs2"
CREATE TABLE book (
    id INTEGER PRIMARY KEY,
    title TEXT,
    author TEXT,
    year INTEGER,
    isbn INTEGER
);
```

---

## 🚀 How to Run

### 1️⃣ Clone the Repository

```bash id="bs3"
git clone https://github.com/your-username/bookstore.git
cd bookstore
```

---

### 2️⃣ Run the Application

```bash id="bs4"
python frontend.py
```

---

## 🧾 Application Flow

1. User opens GUI application
2. Data is stored in SQLite database (`books.db`)
3. User can:

   * Add new book entries
   * Search existing books
   * Update or delete records
4. All changes are saved permanently

---

## 🧩 Key Modules

### 📌 Backend Functions

* `connect()` → Creates database and table
* `insert()` → Adds new book
* `view()` → Displays all books
* `search()` → Searches books
* `update()` → Updates selected book
* `delete()` → Deletes book

### 📌 Frontend Functions

* `view_command()`
* `search_command()`
* `add_command()`
* `update_command()`
* `delete_command()`

---

## 📸 UI Preview

*(You can add a screenshot here of your Tkinter app for better GitHub presentation)*

---

## 📈 Future Improvements

* 🔐 User authentication system
* 🌐 Web version using Flask/Django
* 📊 Better UI using CustomTkinter / PyQt
* ☁️ Cloud database integration
* 📦 Export data to CSV/PDF

---

## 👨‍💻 Author

Built as a beginner Python project to understand:

* GUI development using Tkinter
* Database handling using SQLite
* CRUD operations in desktop applications

---

## ⭐ Support

If you like this project, consider giving it a ⭐ on GitHub!
