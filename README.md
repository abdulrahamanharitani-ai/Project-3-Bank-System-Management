# Project 3 - Bank System Management (Full Version)

A complete C++ Bank Management System built with **Procedural Programming**, featuring:
- **Login System** with Username & Password
- **User Permissions** (Full Access or Custom Permissions)
- **Clients Management** (List, Add, Delete, Update, Find)
- **Transactions** (Deposit, Withdraw, Total Balances)
- **Manage Users** (List, Add, Delete, Update, Find)

📄 **Source Code**: [Project-3-Bank-System-Management/Project-3-Bank-System-Management.cpp](Project-3-Bank-System-Management/Project-3-Bank-System-Management.cpp)

---

## Related Projects

This project is part of a series:
- [Project 1 - Bank System Management](https://github.com/abdulrahamanharitani-ai/Project-1-Bank-System-Management) — Clients List only
- [Project 2 - Bank System Management](https://github.com/abdulrahamanharitani-ai/Project-2-Bank-System-Management) — Clients + Transactions (Deposit, Withdraw, Total Balances)
- **Project 3 - Bank System Management** — Full System with Login & Permissions ← *You are here*

---

## Features

### 1. Login System
- Secure login with Username and Password.
- Invalid login handling with retry.

### 2. Permissions System
- Full Access (Admin).
- Custom permissions for each user:
  - List Clients
  - Add New Client
  - Delete Client
  - Update Client
  - Find Client
  - Transactions
  - Manage Users

### 3. Clients Management
- Show all clients.
- Add new clients.
- Delete clients.
- Update client info.
- Find client by account number.

### 4. Transactions
- Deposit money.
- Withdraw money (with balance validation).
- Show total balances.

### 5. Manage Users
- List all users.
- Add new users.
- Delete users (except Admin).
- Update user info.
- Find user by username.

---

## Data Structures

### sClient
| Field           | Type     |
|-----------------|----------|
| AccountNumber   | string   |
| PinCode         | string   |
| Name            | string   |
| Phone           | string   |
| AccountBalance  | double   |
| MarkForDelete   | bool     |

### stUser
| Field         | Type     |
|---------------|----------|
| Username      | string   |
| Password      | string   |
| Permissions   | int      |
| MarkForDelete | bool     |

---

## Data Files

The system uses two text files to store data:
- `Clients.txt` — Stores client records.
- `Users.txt` — Stores user records (must include an Admin user).

**Default Admin Credentials:**
- **Username**: `Admin`
- **Password**: `1234`

---

## Example Usage

```cpp
int main()
{
    Login();
    system("pause>0");
    return 0;
}
```

## Screenshots

### 🔐 Login System

| Login Screen | Login with User1 |
|:---:|:---:|
| ![Login](screenshots/Login%20Screen.png) | ![Login User1](screenshots/Login%20with%20User1.png) |

| Invalid Login | Logout |
|:---:|:---:|
| ![Invalid](screenshots/Trying%20to%20Login%20with%20incorrect%20Username%20and%20Password.png) | ![Logout](screenshots/Logout.png) |

### 📋 Main Menu

| Main Menu Screen | Return to Main Menu |
|:---:|:---:|
| ![Main Menu](screenshots/Main%20Menu%20Screen.png) | ![Return Main](screenshots/Return%20to%20Main%20Menu.png) |

### 👥 Clients Management

| Client List | Add New Client |
|:---:|:---:|
| ![List](screenshots/Client%20List.png) | ![Add](screenshots/Add%20New%20Client%20Screen.png) |

| Delete Client | Update Client |
|:---:|:---:|
| ![Delete](screenshots/Delete%20Client%20Screen.png) | ![Update](screenshots/Update%20Client%20Screen.png) |

| Find Client |
|:---:|
| ![Find](screenshots/Find%20Client%20Screen.png) |

### 💰 Transactions

| Transactions Menu | Deposit |
|:---:|:---:|
| ![Menu](screenshots/Transactions%20Menu%20Screen.png) | ![Deposit](screenshots/Deposit%20Screen.png) |

| Withdraw | Total Balances |
|:---:|:---:|
| ![Withdraw](screenshots/Withdraw%20Screen.png) | ![Balances](screenshots/Total%20Balances%20List.png) |

### 👤 Manage Users

| Manage Users Menu | User List |
|:---:|:---:|
| ![Menu](screenshots/Manage%20Users.png) | ![List](screenshots/User%20List.png) |

| Add New User | Delete User |
|:---:|:---:|
| ![Add](screenshots/Add%20New%20User%20Screen.png) | ![Delete](screenshots/Delete%20User%20Screen.png) |

| Cannot Delete Admin | Update User (1) |
|:---:|:---:|
| ![Admin](screenshots/Delete%20User%20With%20Admin%20Case.png) | ![Update1](screenshots/Update%20User%20Screen1.png) |

| Update User (2) | Find User |
|:---:|:---:|
| ![Update2](screenshots/Update%20User%20Screen2.png) | ![Find](screenshots/Find%20User%20Screen.png) |

| Return to Main Menu (from Manage Users) |
|:---:|
| ![Return](screenshots/Return%20to%20Main%20from%20Manage%20User%20Menu.png) |

### 🚫 Access Denied

| User1 Trying to Access Manage Users Without Permission |
|:---:|
| ![Access Denied](screenshots/User1%20Trying%20to%20reach%20Manage%20Users%20Menu%20but%20he%20can%27t%20because%20he%20has%20no%20permission.png) |

## Requirements
Visual Studio 2022 or any C++ compiler supporting C++11 or later.

## Author
Abdulrahman Al-Haritani
