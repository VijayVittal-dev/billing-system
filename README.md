# 🛒 Stock & Billing Management System

A simple **C-based Stock and Billing System** that manages items in a store using **hash tables**.
It allows adding, deleting, and viewing stock, as well as handling a **cart system with billing** (including taxes and discounts).

---

## 📌 Features

* 📦 **Stock Management**

  * Add new items with HSN code, name, quantity, and price
  * Update quantity if item already exists
  * Delete items fully or partially from stock
  * View current stock in a tabular format

* 🛒 **Cart System**

  * Add items to cart using HSN code
  * Adjust stock automatically when items are added to cart
  * Generate a **detailed bill** with GST (CGST & SGST) and discount calculations
  * Save bills to a file (`bill.txt`)
  * Print generated bills directly from the file

* 🧮 **Billing Features**

  * Taxable amount calculation
  * CGST @2.5%
  * SGST @2.5%
  * Discount @5%
  * Final amount with summary

---

## 🛠️ Technologies Used

* **C Language**
* **File Handling** (`bill.txt`)
* **Hash Table with Linear Probing** for stock storage
* **Dynamic Memory Allocation** for items

---

## 📂 Project Structure

```bash
stock-billing-system/
│── stock_billing.c    # Main source code
│── bill.txt           # Bill file generated at runtime
│── README.md          # Documentation
```

---

## 🚀 Getting Started

### 1️⃣ Compile the program

```bash
gcc stock_billing.c -o stock_billing
```

### 2️⃣ Run the program

```bash
./stock_billing
```

---

## 📋 Usage Flow

1. **Main Menu Options**

   * Open Cart
   * Add to Stock
   * Delete from Stock
   * View Current Stock
   * Exit

2. **Cart Options**

   * Add item
   * Empty the cart
   * Generate bill
   * Print bill
   * Exit

---

## 📊 Sample Bill (bill.txt)

```
                 EVERyTHING SHOPPING MALL
Opp. Sony digital, Nakkalgutta, Hanamkonda, Telangana-506345.
Phone no.: +91 9218199111
GSTIN: AB2929292Z833K
PAN No.: A123456DK8K
----------------------------------------------------------------------------------
HSN-Code        item-name                 cost-per-item   quantity            cost
----------------------------------------------------------------------------------
1234            Soap                              40.0        3.0           120.0
5678            Shampoo                          120.0        1.0           120.0
----------------------------------------------------------------------------------
Taxable Amount                                               4.0           240.0
CGST @2.5%                                                                6.0
SGST @2.5%                                                                6.0
Discount @5%                                                             -12.0
----------------------------------------------------------------------------------
Total Amount:                                                            240.0
----------------------------------------------------------------------------------
                                  Thank You! Visit Again.
```

---

## 🔮 Future Enhancements

* Add **persistent database storage** instead of in-memory hash table
* Add **user authentication** (Admin vs Cashier)
* Support **multiple carts** and billing history
* Improve **UI with ncurses** for a more interactive terminal interface

---

## 👨‍💻 Author

Developed by **Vijay Vittal**

