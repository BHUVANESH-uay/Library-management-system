# 📚 Library Management System (CLI-Based) — Golang

A command-line based **Library Management System** built with Go, designed to simulate real-world library operations. The system supports multiple user roles (Guest, Reader, Administrator) and provides features such as book search, borrowing, returning, and administrative control.

---

## 🧩 Features

### 🔐 Authentication
- `register` – Create a new user account
- `login` – Log in with credentials
- `guest-mode` – Use the system without logging in
- `exit` – Logout and exit the application

### 👤 Role-Based Access

#### Guest:
- Search books by `title`, `author`, or `isbn`

#### Reader:
- All guest features +
- Reset own password (`pw`)
- Borrow and return books
- Extend return deadlines
- View deadlines, overdue books, unreturned books, and borrow history

#### Administrator:
- All reader features +
- Add new users (`adduser`)
- Add and remove books (`addbook`, `removebook`)
- Reset user passwords (`userpw`)

> 🛑 Admins are advised to reset passwords and remove books cautiously, especially in cases involving lost books and fines.

---

## 🛠️ Built With

- **Golang** — Core language
- CLI — Terminal-based interface
- Simple file-based storage (or easily extendable to DB)

---

## 🚀 Getting Started

```bash
go run main.go
