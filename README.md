# 📚 Library Management System (Golang)

A command-line based **Library Management System** built with Go. The system supports multiple user roles (Guest, Reader, Administrator) with different levels of access to manage books, borrowing, and user operations.

---

## 🧩 Features

### 🔐 Authentication
- `register` – Register a new user account
- `login` – Log in with your credentials
- `guest-mode` – Use the system without logging in
- `exit` – Log out and exit the system
- `help` – Get instructions for using the system

### 👤 User Roles and Commands

#### **1. Guest**
- `title` – Search books by title
- `author` – Search books by author
- `isbn` – Search books by ISBN

#### **2. Reader (Logged-in User)**
All guest features, plus:
- `pw` – Reset your own password
- `borrow` – Borrow a book
- `return` – Return a borrowed book
- `extend` – Extend the return deadline of a book
- `deadline` – Query the return deadline of a borrowed book
- `overdue` – View the number of overdue books
- `unreturned` – View all unreturned books
- `history` – View your borrow history

#### **3. Administrator**
All reader features, plus:
- `adduser` – Add a new user and set their role
- `addbook` – Add a new book to the system
- `userpw` – Reset a user's password (use with caution)
- `removebook` – Remove a book from the system (ensure fines are cleared for lost books)

> ⚠️ **Caution:** When removing a book due to a loss, ensure the student has returned it and the fine is paid, or it may affect the entire system's integrity.

---

## 🛠️ Built With

- **Golang** — Core language
- **CLI** — Command-line interface for easy interaction

---

## 🚀 Getting Started

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/library-management-system.git
    ```

2. Navigate into the project directory:
    ```bash
    cd library-management-system
    ```

3. Run the system:
    ```bash
    go run main.go
    ```

4. Follow the on-screen instructions to register, log in, and explore the features.

---
