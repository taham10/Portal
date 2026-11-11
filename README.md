# E-Commerce Order Management Portal

A Python-based **E-Commerce Order Management System** developed using Jupyter Notebook. The portal provides an efficient way to manage products, inventory, customer orders, order statuses, sales reports, and database backups through a menu-driven interface.

## 📌 Project Overview

The E-Commerce Order Management Portal is designed for online shopping businesses to simplify their daily operations. It allows administrators to manage products and inventory while processing customer orders and tracking their progress.

The system uses JSON file handling for persistent data storage, ensuring that product and order information remains available between sessions.

## ✨ Features

### 1. Admin Authentication
- Secure admin login.
- Maximum of three login attempts.
- Access restricted to authorized administrators.

### 2. Product Management
- Add new products.
- View all available products.
- Search products using Product ID.
- Prevent duplicate Product IDs.
- Validate product information.

### 3. Inventory Management
- Update product prices.
- Update available stock.
- Automatically reduce inventory when an order is placed.
- Restore inventory when an order is cancelled.
- Prevent orders exceeding available stock.

### 4. Order Management
- Place customer orders.
- Add multiple products to a single order.
- Automatically calculate item subtotals and total amounts.
- Generate unique Order IDs.
- Search orders using Order ID.
- View complete order details.

### 5. Order Status Management

Orders can have the following statuses:

- Pending
- Processing
- Shipped
- Delivered
- Cancelled

Administrators can update order statuses while following the system's status restrictions.

### 6. Order Cancellation
- Cancel existing orders.
- Ask for confirmation before cancellation.
- Automatically restore product inventory.
- Prevent cancellation of delivered or already cancelled orders.

### 7. Sales Reports
Generate sales reports containing:
- Total number of orders.
- Delivered orders.
- Pending, processing, and shipped orders.
- Cancelled orders.
- Total revenue from delivered orders.

### 8. Inventory Reports
- Total number of products.
- Total available inventory units.
- Identify products with low stock (5 units or fewer).

### 9. Data Backup
- Create database backups.
- Automatically create a backup directory.
- Store backup copies of the JSON database.
- Handle file and permission errors.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Jupyter Notebook | Development and execution environment |
| JSON | Data storage |
| `json` | Reading and writing database records |
| `os` | File and directory management |
| `shutil` | Database backup operations |
| `datetime` | Recording order dates and times |

## 📂 Project Structure

```text
E-Commerce-Order-Management-Portal/
│
├── E-Commerce_Order_Management.ipynb
│
├── ecommerce_data.json
│
└── backup/
    └── ecommerce_backup.json
```

*Note: The JSON database and backup directory are created automatically when the application runs.*

## 🚀 Installation and Execution

### Prerequisites
- Python 3.x
- Jupyter Notebook or JupyterLab

### Step 1: Clone the Repository

```bash
git clone https://github.com/taham10/E-Commerce-Order-Management-Portal.git
```

### Step 2: Navigate to the Project Directory

```bash
cd E-Commerce-Order-Management-Portal
```

### Step 3: Install Jupyter Notebook

```bash
pip install notebook
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

### Step 5: Run the Application

1. Open `E-Commerce_Order_Management.ipynb`.
2. Execute the notebook cells in order.
3. Run the final cell containing `main()` to launch the portal.
4. Log in using the administrator credentials.

## 🔐 Default Admin Credentials

| Field | Credentials |
|---|---|
| Username | `admin` |
| Password | `admin123` |

**Note:** These are demonstration credentials. Change them before using the system in a real environment.

## 📋 Main Menu

The application provides the following menu-driven options:

```text
========== MAIN MENU ==========
1. Add New Product
2. View All Products
3. Search Product
4. Update Inventory
5. Place Customer Order
6. Search Order
7. Update Order Status
8. Cancel Order
9. Generate Sales Report
10. Inventory Report
11. Create Data Backup
12. Exit
===============================
```

## 💾 Data Storage

The application uses a JSON file (`ecommerce_data.json`) as its database.

The database stores two main categories of information:

- **Products:** Product ID, name, category, price, and available stock.
- **Orders:** Order ID, customer name, ordered items, total amount, status, and order date.

The system automatically loads existing records when launched and saves changes whenever products or orders are modified.

## 🎯 Project Objectives

- Apply Python programming concepts to a real-world business scenario.
- Implement functions and modular programming.
- Understand lists and dictionaries for data management.
- Practice file handling using JSON.
- Implement exception handling and input validation.
- Develop inventory and order management operations.
- Generate automated sales and inventory reports.

## 🔮 Future Improvements

- Customer registration and authentication.
- Graphical user interface (GUI).
- Integration with a relational database such as MySQL.
- Online payment integration.
- Customer order tracking.
- Export sales reports to PDF or Excel.
- Password hashing and improved authentication security.

## 👩‍💻 Author

**Taham Ahmad**

BS Business Analytics
FAST NUCES

---

*Developed as a Python programming project.*
