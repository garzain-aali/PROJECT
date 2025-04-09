
# 🧑‍💻 User Management System & File Organizer

This repository contains two simple and useful beginner-level projects:

1. **User Management System (C++)**
2. **File Organizer by Extension (Python)**

---

## 📘 1. User Management System (C++)

A console-based user management app built using C++. You can register users, log in, show the list of users, search, and delete users using a simple menu.

### ✅ Features
- Register new users
- Login verification
- List all users
- Search for a user
- Delete a user

### 🔄 Example Menu
```
1. Register User
2. Login
3. Show User List
4. Search User
5. Delete User
6. Exit
```

### 🧠 How it works:
- Uses classes and vectors to manage users.
- Data is stored temporarily during the program's execution.
- Ideal for understanding object-oriented programming in C++.

### 🔧 How to Run:
```bash
g++ user_management.cpp -o user_management
./user_management
```

---

## 📂 2. File Organizer by Extension (Python)

A simple Python script to automatically organize all files in a folder based on their extensions. Great for cleaning your **Downloads** or any cluttered directory.

### ✅ Features
- Moves files into folders like `jpg`, `pdf`, `mp4`, etc.
- Creates folders automatically if not present.
- Works on any directory path given by the user.

### 📦 How to Use
```bash
python file_organizer.py
```

Then, input the path:
```
Enter Your Path -> C:\Users\YourName\Downloads
```

### 🧠 Example
Before:
```
photo.jpg, song.mp3, notes.pdf
```

After:
```
📁 jpg → photo.jpg  
📁 mp3 → song.mp3  
📁 pdf → notes.pdf
```

---

## 🛠 Requirements

- C++ Compiler (for C++ project)
- Python 3.x (for file organizer)
  - No external libraries needed

---

## 📄 License
This project is licensed under the MIT License — feel free to use and modify it.
