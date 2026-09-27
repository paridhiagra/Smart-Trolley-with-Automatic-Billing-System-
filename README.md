<div align="center">

# 🛒 Smart Billing System for Smart Trolley

### RFID-Based Automated Billing Prototype using Arduino Nano

An embedded systems project that uses **RFID-based product identification**, **Arduino Nano processing**, and an **LCD display** to automatically calculate and display the shopping bill in real time.

<p>
  <img src="https://img.shields.io/badge/Arduino-Nano-00979D?style=for-the-badge&logo=arduino&logoColor=white">
  <img src="https://img.shields.io/badge/Embedded-C-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/RFID-Product%20Detection-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/LCD-Display-orange?style=for-the-badge">
  <img src="https://img.shields.io/badge/Arduino%20IDE-Development-red?style=for-the-badge&logo=arduino&logoColor=white">
</p>

</div>

---

## 📸 Project Preview

<p align="center">
  <img src="smart trolley.png" alt="Smart Trolley Prototype" width="850">
</p>

> 🛒 **Smart Trolley prototype** designed to demonstrate automatic product identification and real-time billing.

---

## 📖 Overview

The **Smart Billing System for Smart Trolley** is an embedded systems prototype designed to automate the shopping billing process using **RFID technology**.

When a customer places an RFID-tagged product inside the trolley, the **RFID reader detects the product**, and the **Arduino Nano processes the scanned information**. The corresponding product details and price are then used to update the running bill, which is displayed on an **LCD screen**.

The main goal of the system is to reduce manual billing effort, provide transparent real-time billing, and reduce dependency on traditional checkout counters.

📌 The concept is based on the **Smart Trolley: Automatic Billing System Using Arduino** report, which describes automatic product detection, real-time billing, customer monitoring, security verification, and possible future integration with digital payment and IoT systems.

---

## 🎯 Objectives

* 🛒 Develop a smart shopping trolley with automatic billing.
* 📡 Identify products using RFID/barcode technology.
* 💰 Calculate and update the bill in real time.
* 🖥️ Display product information and the running total.
* ⏱️ Reduce customer waiting time at billing counters.
* 🤖 Reduce manual billing effort.
* 🔒 Provide a mechanism for detecting unpaid items.
* 💡 Develop a cost-effective and scalable retail automation concept.

---

## ✨ Key Features

### 📡 RFID-Based Product Identification

The RFID reader detects the unique identification information associated with a product.

### 💰 Real-Time Billing

The system updates the running bill whenever a product is added or removed.

### 🖥️ LCD Display

The LCD provides customers with information about the products and the current bill.

### ⚡ Arduino Nano Processing

The Arduino Nano acts as the central controller and coordinates the RFID reader, billing logic, and display.

### 🔄 Automatic Billing

Product information is processed automatically instead of requiring manual entry at a conventional billing counter.

### 🔒 Security & Alert Concept

The proposed system can verify whether items have been billed before the customer leaves the store and trigger an alert when unpaid items are detected.

### 📦 Scalable Architecture

The concept can be extended for larger retail environments and additional automation features.

---

## 🛠️ Tech Stack

| Category                  | Technology                       |
| ------------------------- | -------------------------------- |
| 🔧 Microcontroller        | Arduino Nano                     |
| 💻 Programming            | Embedded C / Arduino Programming |
| 📡 Product Identification | RFID                             |
| 🖥️ Display               | LCD                              |
| 🔌 Development            | Arduino IDE                      |
| ⚡ Power                   | Battery / Power Supply           |
| 🛒 Platform               | Shopping Trolley                 |

---

## 🔩 Hardware Components

| Component            | Purpose                                         |
| -------------------- | ----------------------------------------------- |
| 🔧 **Arduino Nano**  | Main controller of the system                   |
| 📡 **RFID Reader**   | Detects product identification                  |
| 🏷️ **RFID Tags**    | Unique identification of products               |
| 🖥️ **LCD Display**  | Displays product details and running bill       |
| 🔋 **Power Supply**  | Provides power to the system                    |
| 🔌 **Jumper Wires**  | Hardware connections                            |
| 🛒 **Trolley Frame** | Holds the groceries and electronic components   |
| 🔔 **Alert System**  | Provides security notification for unpaid items |

---

## ⚙️ Working Principle

The Smart Trolley follows a simple automated billing process:

```text
        🛒 Product Added
               │
               ▼
       📡 RFID Detection
               │
               ▼
        🔧 Arduino Nano
               │
               ▼
     🔎 Identify Product
               │
               ▼
       💰 Calculate Price
               │
               ▼
        🖥️ Update LCD
               │
               ▼
       📊 Running Bill
               │
               ▼
        🔒 Security Check
```

### 1️⃣ Product Scanning

When a customer places a product inside the trolley, the RFID reader detects its unique identification code.

### 2️⃣ Data Processing

The RFID data is sent to the **Arduino Nano**, which processes the information.

### 3️⃣ Product Identification

The system retrieves the corresponding product name and price from the stored product information.

### 4️⃣ Bill Calculation

The product price is added to the current running total.

### 5️⃣ LCD Update

The LCD dynamically displays the product information and updated bill.

### 6️⃣ Product Removal

If an item is removed, the corresponding amount can be deducted from the running bill.

### 7️⃣ Security Verification

The proposed system can perform a verification check at the store exit to identify unpaid products.

### 8️⃣ System Reset

After completing the purchase, the billing information is cleared and the trolley can be prepared for the next customer.

---

## 🔄 System Architecture

<p align="center">
  <img src="images/system-architecture.png" alt="Smart Trolley System Architecture" width="850">
</p>

### 🧩 Architecture Flow

```text
              🏷️ RFID Tag
                   │
                   ▼
            📡 RFID Reader
                   │
                   ▼
          ┌─────────────────┐
          │   🔧 Arduino    │
          │      Nano       │
          └───────┬─────────┘
                  │
          ┌───────┴────────┐
          ▼                ▼
    🖥️ LCD Display     💰 Billing
                           │
                           ▼
                    🔒 Security
```

---

## 🔌 Circuit Diagram

<p align="center">
  <img src="images/circuit.png" alt="Smart Trolley Circuit Diagram" width="850">
</p>

> ⚡ The circuit integrates the **Arduino Nano, RFID reader, LCD display, power supply, and supporting components**.

---

## 📊 Project Workflow

<p align="center">
  <img src="images/workflow.png" alt="Smart Trolley Workflow" width="850">
</p>

```text
🛒 Add Product
      ↓
📡 Scan RFID
      ↓
🔧 Process with Arduino
      ↓
🔎 Identify Product
      ↓
💰 Update Bill
      ↓
🖥️ Display Total
      ↓
💳 Complete Purchase
      ↓
🔒 Verify Items
      ↓
🔄 Reset Trolley
```

---

## 🖥️ LCD Output Example

| 🛒 Action       | 🖥️ LCD Output  |
| --------------- | --------------- |
| First Product   | `Milk - ₹45`    |
| Second Product  | `Bread - ₹35`   |
| Product Added   | `Total: ₹80`    |
| Product Removed | `Total Updated` |

> 💡 **Note:** These are example LCD outputs demonstrating how product information and the running total can be displayed.

---

## 📂 Project Structure

```text
Smart-Billing-System/
│
├── 📄 SmartBilling.ino
├── 🖼️ smart trolley.png
├── 📄 README.md
│
├── 📁 images/
│   ├── 🖼️ system-architecture.png
│   ├── 🖼️ circuit.png
│   ├── 🖼️ workflow.png
│   └── 🖼️ prototype.jpg
│
└── 📁 documentation/
    └── 📄 Smart-Trolley-Report.pdf
```

---

## 🎯 Skills Demonstrated

* 🔧 Embedded Systems
* 💻 Arduino Programming
* 📡 RFID Integration
* 🖥️ LCD Interfacing
* 🔌 Hardware Integration
* ⚡ Real-Time Processing
* 🧩 Circuit Design
* 🛠️ Prototype Development
* 🧪 Hardware Testing
* 🔄 Hardware-Software Integration

---

## 🚀 Applications

The Smart Trolley concept can be applied to:

* 🛒 Smart Shopping Trolleys
* 🏪 Supermarkets
* 🏬 Retail Stores
* 💳 Automated Billing Systems
* 📦 Retail Inventory Systems
* 🤖 Embedded Systems Demonstrations

---

## 🔮 Future Scope

The report proposes several possible extensions to make the system more advanced:

### 🌐 IoT Integration

IoT connectivity can be used for **real-time inventory management** and stock monitoring.

### 💳 Digital Payment

The trolley can be extended to support **UPI, debit/credit cards, and e-wallets**.

### ⚖️ Weight Sensors

Weight sensors can provide an additional mechanism for product verification.

### 📷 Computer Vision

Computer vision can be explored for improved product detection and verification.

### 🎙️ Voice Recognition

Voice-based assistance can be integrated to improve accessibility and usability.

### 📱 Mobile Integration

The system could potentially communicate shopping and billing information to a mobile application.

> 🚧 These features represent **future/proposed extensions** of the system rather than features claimed as fully implemented in the prototype.

---

## 📚 Learning Outcomes

Through this project, I strengthened my understanding of:

* 📡 RFID-based embedded applications
* 🔧 Arduino Nano programming
* 🖥️ LCD interfacing
* 🔌 Hardware-software integration
* 💰 Real-time billing logic
* ⚡ Electronic component integration
* 🧪 Prototype testing
* 🛒 Retail automation concepts

---

## 🌟 Project Highlights

<div align="center">

|    ⚡ Feature    | 💡 Description                   |
| :-------------: | :------------------------------- |
|     📡 RFID     | Automatic product identification |
| 🔧 Arduino Nano | Central processing unit          |
|    💰 Billing   | Real-time bill calculation       |
|     🖥️ LCD     | Live bill display                |
|   🔒 Security   | Unpaid-item verification concept |
|    🛒 Trolley   | Integrated shopping platform     |

</div>

---

## 📜 Project Information

**Project:** Smart Billing System for Smart Trolley
**Domain:** Embedded Systems & Retail Automation
**Controller:** Arduino Nano
**Identification:** RFID
**Display:** LCD
**Development Environment:** Arduino IDE

---

## 👩‍💻 Author

**Paridhi Agrawal**

🎓 Electronics & Communication Engineering
💻 Embedded Systems | Software Development | Technology

---

<div align="center">

### 🛒 Scan • Calculate • Display • Shop

⭐ **Smart Trolley – Making Shopping Smarter with Embedded Technology**

</div>
