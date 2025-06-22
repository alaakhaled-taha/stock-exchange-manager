# 📊 Stock Exchange Manager

A comprehensive **stock trading simulation system** developed using **JavaFX**. This project showcases modern Java GUI design, database integration, and modular architecture through multi-role interfaces, real-time approvals, and financial transaction management.


---

## 🚀 Overview

This application enables simulation of a basic financial trading system with the following key roles:

* **Users**: Can deposit funds, view balances, and request stock transactions.
* **Admins**: Oversee the trading system, approve transactions, and manage user accounts.

---

## 🧱 Architecture

The project follows the **Model-View-Controller (MVC)** pattern with full separation of concerns. Each screen is backed by:

* **Controllers**: Handle logic and event interaction.
* **FXML Files**: Define the layout/UI using JavaFX Scene Builder.
* **Models**: Abstract database entities (users, orders, stocks).

---

## 📦 Modules and Responsibilities

### 🎛️ Controllers

| Controller                      | Responsibility                                                      |
| ------------------------------- | ------------------------------------------------------------------- |
| `AdminController`               | Manages system users, stocks, and admin operations                  |
| `ApprovalSystemAdminController` | Handles review and approval/rejection of pending stock transactions |
| `HomeAdminController`           | Admin dashboard and session management                              |
| `HomeUserController`            | Displays user home page, balance, and transaction history           |
| `DepositUserController`         | Allows users to deposit funds into their trading accounts           |
| `ItemCompanyController`         | Displays stocks grouped by company                                  |
| `itemController`                | Generic controller for displaying stock or transaction items        |

### 🧩 FXML Views

FXML files correspond directly to the controller logic:

* `Admin.fxml`, `ApprovalSystemAdmin.fxml`, `DepositUser.fxml`, `HomeAdmin.fxml`, `HomeUser.fxml`, `ItemCompany.fxml`, `item.fxml`, etc.

---

## 💾 Database Layer

The application integrates with a backend database for persistent storage using custom classes:

| Class      | Description                             |
| ---------- | --------------------------------------- |
| `UserDB`   | Handles operations related to user data |
| `StockDB`  | Manages stock listing and pricing       |
| `OrdersDB` | Tracks stock purchase/sell requests     |

All database operations follow encapsulated access logic and ensure clean separation from UI code.

---

## ✨ Features

* 🔐 **Role-Based Access** – Separate interfaces for users and admins
* ✅ **Approval Workflow** – Admins approve/reject stock transactions
* 💵 **Deposit System** – Users can add funds to their virtual wallet
* 🧠 **Dynamic Content Rendering** – Stock listings and user transactions update live
* 📊 **User Dashboard** – Real-time view of balance, stocks, and history
* 🖥️ **Responsive UI** – JavaFX-powered graphical interface with Scene Builder design
* 🧹 **Clean Codebase** – Modular Java classes and layered architecture

---

## 📷 User Interface

| Admin Dashboard                                                                                                                                        | Transaction Approval                                                                                                                                      | User Wallet                                                                                                                                             |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Admin](https://github.com/sbme-tutorials/sbme27-s24-task2-stockexchangemanager-pixel-pioneers/assets/148906681/3a2ee733-dd2d-4b2c-b728-7405a33982f0) | ![Approval](https://github.com/sbme-tutorials/sbme27-s24-task2-stockexchangemanager-pixel-pioneers/assets/148906681/02e8872d-380b-4b84-8f0d-6a3cc9d1bb96) | ![Wallet](https://github.com/sbme-tutorials/sbme27-s24-task2-stockexchangemanager-pixel-pioneers/assets/148906681/ec71d9bc-57e5-483c-b1cc-93bff9bd5144) |

---

## 🛠️ Setup & Execution

### 📋 Requirements

* Java JDK 11+
* JavaFX SDK
* IDE with JavaFX support (e.g., IntelliJ IDEA)
* Scene Builder (recommended for editing FXML)

### 🔧 Running the Application

1. **Clone the Repository**

   ```bash
   git clone https://github.com/<your-username>/sbme27-s24-task2-stockexchangemanager-pixel-pioneers.git
   cd sbme27-s24-task2-stockexchangemanager-pixel-pioneers
   ```

2. **Configure JavaFX**

   * Set VM options:

     ```bash
     --module-path /path/to/javafx-sdk/lib --add-modules javafx.controls,javafx.fxml
     ```

3. **Run Main Class**

   * Launch `Main.java` from your IDE.

---

## 📈 Future Enhancements

* 🌐 Cloud-based database support
* 📱 Mobile app integration (e.g., Flutter or JavaFXPorts)
* 📉 Real-time stock market simulation
* 📢 Notification system for pending approvals or market changes

---


