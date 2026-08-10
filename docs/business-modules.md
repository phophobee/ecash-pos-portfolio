# eCash POS — Business Modules

eCash POS is organized around several core business modules.

## 1. Master Data

Master data provides the foundation for daily business transactions.

### Products

* Product code
* Barcode
* Product name
* Category
* Subcategory
* Unit
* Purchase price
* Selling price
* Multiple pricing levels

### Customers

Customer information and transaction-related data.

### Suppliers

Supplier information and purchasing-related data.

---

## 2. Point of Sale

The POS module handles daily sales transactions.

Main capabilities include:

* Product search
* Barcode scanning
* Product selection
* Multiple units
* Multiple prices
* Quantity management
* Payment processing
* Transaction recording
* Thermal receipt printing

---

## 3. Purchasing

The purchasing module manages procurement activities.

```text
Supplier
   ↓
Purchase Transaction
   ↓
Purchase Detail
   ↓
Inventory Update
   ↓
Accounts Payable
```

---

## 4. Sales

The sales module manages customer transactions.

```text
Customer
   ↓
Sales Transaction
   ↓
Sales Detail
   ↓
Inventory Update
   ↓
Accounts Receivable
```

---

## 5. Inventory

Inventory management tracks product quantities and stock movements.

Features include:

* Stock monitoring
* Stock movement
* Stock adjustment
* Stock opname
* Multi-unit inventory
* Inventory reporting

---

## 6. Accounts Receivable

The receivables module helps businesses monitor outstanding customer payments.

Capabilities include:

* Customer receivables
* Payment tracking
* Outstanding balances
* Receivable reporting

---

## 7. Accounts Payable

The payables module manages outstanding supplier obligations.

Capabilities include:

* Supplier payables
* Payment tracking
* Outstanding balances
* Payable reporting

---

## 8. Reporting

Business reports provide information to support operational decisions.

Examples include:

* Sales reports
* Purchasing reports
* Inventory reports
* Stock reports
* Customer reports
* Supplier reports
* Receivable reports
* Payable reports
* Profit-related reports

---

## Integrated Business Process

The modules are designed to work together rather than operate as isolated features.

```text
Products
   │
   ├───────────────┐
   │               │
   ▼               ▼
Purchasing       Sales
   │               │
   ▼               ▼
Inventory ◄────────┘
   │
   ├──────────────► Reports
   │
   ├──────────────► Payables
   │
   └──────────────► Receivables
```

This integration allows business transactions to automatically contribute to inventory and financial information.
