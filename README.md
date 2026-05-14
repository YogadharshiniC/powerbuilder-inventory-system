<div align="center">

# 📦 PowerBuilder Inventory Management System

### A Desktop-Based Enterprise ERP Application

![PowerBuilder](https://img.shields.io/badge/PowerBuilder-2022+-blue?style=for-the-badge&logo=sap&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-Database-orange?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Windows-informational?style=for-the-badge&logo=windows&logoColor=white)
![Type](https://img.shields.io/badge/Type-Desktop%20App-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

> A robust, enterprise-grade Inventory Management System built with **PowerBuilder** and **SQL**, designed to streamline stock tracking, product management, and warehouse operations through a clean desktop interface.

</div>

---

## 📖 Table of Contents

- [About the Project](#-about-the-project)
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [How to Run](#-how-to-run)
- [Screenshots](#-screenshots)
- [Learning Outcomes](#-learning-outcomes)
- [Future Improvements](#-future-improvements)
- [License](#-license)

---

## 🏢 About the Project

The **PowerBuilder Inventory Management System (Mini ERP)** is a desktop-based enterprise application developed to manage inventory operations efficiently. It leverages PowerBuilder's powerful **DataWindow** technology for seamless database interaction and provides a complete solution for stock and product lifecycle management.

This project was developed as a **learning and enterprise practice project** to demonstrate proficiency in PowerBuilder development, SQL integration, and enterprise application design patterns.

---

## ✨ Features

| Feature | Description |
|---|---|
| 📋 **Product Management** | Add, view, update, and delete product records |
| 📦 **Stock Management** | Real-time stock level tracking and updates |
| 🔍 **Dynamic Search** | Filter and search records with flexible query support |
| 🗄️ **DataWindow Integration** | Powerful data display and manipulation via PB DataWindows |
| 🔄 **Full CRUD Operations** | Complete Create, Read, Update, Delete functionality |
| 🔗 **Database Integration** | Direct SQL database connectivity and transaction management |
| 🖥️ **Desktop UI** | User-friendly Windows desktop interface |
| 📊 **Data Reporting** | Tabular data views with sorting and filtering |

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| ![PowerBuilder](https://img.shields.io/badge/PowerBuilder-2022+-blue) | Core application development framework |
| ![SQL](https://img.shields.io/badge/SQL-Database-orange) | Backend database for persistent data storage |
| **DataWindow** | PowerBuilder component for data-bound UI |
| **PowerScript** | Server-side scripting for business logic |
| **PBL Libraries** | Modular code organization via PowerBuilder Libraries |

---

## 📁 Project Structure

```
Mini_erp/
│
├── 📂 Mini_erp/                    # Main project directory
│   ├── mini_erp.pbw                # PowerBuilder Workspace (entry point)
│   │
│   ├── erp_app.pbt                 # ERP Application Target
│   ├── erp_app.pbl                 # ERP Application Library (main app logic)
│   │
│   ├── erpwindows.pbl              # ERP Windows Library (UI windows)
│   ├── datawindows.pbl             # DataWindows Library (data components)
│   │
│   ├── dynamic_search.pbt          # Dynamic Search Target
│   ├── dynamic_search.pbl          # Dynamic Search Library
│   │
│   ├── erp_app.usr.opt             # User-specific IDE options (erp app)
│   └── dynamic_search.usr.opt      # User-specific IDE options (search)
│
└── README.md
```

> **Note:** `.pbl` = PowerBuilder Library | `.pbt` = PowerBuilder Target | `.pbw` = PowerBuilder Workspace | `.opt` = User Options (IDE-specific, not committed)

---

## 🚀 Getting Started

### Prerequisites

Before running this project, ensure you have the following installed:

- ✅ **PowerBuilder 2022** or a compatible version (2019+)
- ✅ **SQL Server** (or compatible RDBMS — SQL Anywhere, Oracle, etc.)
- ✅ Windows 10/11 OS
- ✅ Appropriate ODBC/database driver configured

### Database Setup

1. Open your SQL Server Management Studio (SSMS) or equivalent tool.
2. Create a new database (e.g., `mini_erp_db`).
3. Run the SQL schema scripts to set up required tables:
   - `products` table
   - `stock` table
   - Any related lookup/reference tables
4. Configure an **ODBC Data Source** on your machine pointing to this database.

---

## ▶️ How to Run

```text
Step 1: Clone or download this repository to your local machine.

Step 2: Open PowerBuilder IDE.

Step 3: Go to File → Open Workspace
        Navigate to: Mini_erp/mini_erp.pbw
        Click Open.

Step 4: In the System Tree, right-click on erp_app target
        → Set as Active Target

Step 5: Configure the database profile:
        Tools → Database Profiles → New/Edit
        Set the ODBC connection to your configured data source.

Step 6: Click Run (F5) or use the toolbar Run button
        to compile and launch the application.
```

> **Tip:** If you encounter library errors, right-click each `.pbl` in the System Tree and select **Regenerate** to rebuild the library entries.

---

## 📸 Screenshots

> Screenshots will be added here. Place images in a `/screenshots` folder and reference them below.

| Module | Preview |
|---|---|
| 🏠 **Main Dashboard** | *(screenshot placeholder — `screenshots/dashboard.png`)* |
| 📦 **Product Management** | *(screenshot placeholder — `screenshots/products.png`)* |
| 📋 **Stock Management** | *(screenshot placeholder — `screenshots/stock.png`)* |
| 🔍 **Dynamic Search** | *(screenshot placeholder — `screenshots/search.png`)* |

---

## 🎓 Learning Outcomes

Through this project, the following skills and concepts were practised and strengthened:

- 🔵 **PowerBuilder Architecture** — Understanding workspace, targets, and PBL library structure
- 🔵 **DataWindow Technology** — Building and configuring data-bound components for efficient UI/DB interaction
- 🔵 **PowerScript Programming** — Writing event-driven business logic scripts
- 🔵 **SQL Integration** — Connecting PowerBuilder apps to relational databases via ODBC/direct connections
- 🔵 **CRUD Design Patterns** — Implementing full Create, Read, Update, Delete workflows
- 🔵 **Enterprise Application Design** — Structuring modular, maintainable desktop applications
- 🔵 **Dynamic Querying** — Building flexible, parameterized search functionality
- 🔵 **Transaction Management** — Handling database commits and rollbacks programmatically

---

## 🔮 Future Improvements

- [ ] 📊 Add inventory reports and PDF export functionality
- [ ] 🔐 Implement user authentication and role-based access control (RBAC)
- [ ] 🔔 Low-stock alerts and notification system
- [ ] 📈 Dashboard with charts for stock movement analytics
- [ ] 🧾 Purchase order and invoice generation
- [ ] 🌐 REST API integration for web/mobile connectivity
- [ ] 🗂️ Audit trail / change log for data modifications
- [ ] 🔄 Supplier and purchase management module
- [ ] 🖨️ Print-ready reports using PowerBuilder reporting

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

```
MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files, to deal in the Software
without restriction, including without limitation the rights to use, copy,
modify, merge, publish, distribute, sublicense, and/or sell copies of the Software.
```

---

<div align="center">

### 💼 Developed by Yogadharshini C

*Enterprise Application Developer | PowerBuilder Practitioner*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin)](https://linkedin.com)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=flat-square&logo=github)](https://github.com)

---

*⭐ If you found this project useful or interesting, please consider giving it a star!*

</div>
