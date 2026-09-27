<div align="center">

# 🛒 Smart Trolley with Automatic Billing System

### 📡 RFID-Based Automated Billing System using Arduino Nano

An embedded systems mini project that uses **RFID technology, Arduino Nano, LCD, and GSM communication** to identify products, calculate the shopping bill in real time, allow item removal, and send the generated bill through SMS.

<p>
  <img src="https://img.shields.io/badge/Arduino-Nano-00979D?style=for-the-badge&logo=arduino&logoColor=white">
  <img src="https://img.shields.io/badge/RFID-EM--18-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/GSM-SIM800L-orange?style=for-the-badge">
  <img src="https://img.shields.io/badge/LCD-20x4-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Embedded-C-red?style=for-the-badge">
</p>

</div>

---

## 📸 Project Preview

<p align="center">
  <img src="images/prototype.jpg" alt="Smart Trolley Hardware Prototype" width="850">
</p>

> 🛒 The hardware prototype integrates the Arduino Nano, EM-18 RFID reader, LCD, GSM module, buttons, LEDs, buzzer, and supporting circuitry.

---

## 📖 Overview

The **Smart Trolley with Automatic Billing System** is an embedded systems project designed to automate the traditional shopping and billing process.

The system uses an **EM-18 RFID reader** to identify RFID-tagged products. The unique RFID tag ID is transmitted to an **Arduino Nano**, which processes the received data and performs the corresponding billing operation.

When a product is scanned, its **name and price are displayed on the LCD**, and the total bill is updated automatically. The system also provides an option to remove a previously added item using a button and RFID scan.

A **SIM800L GSM module** is integrated to send the generated bill or text message to a mobile number. The prototype also uses **green/red LEDs and a buzzer** to provide status and error feedback.

The project demonstrates the practical application of **RFID, embedded programming, LCD interfacing, GSM communication, and hardware-software integration**.

---

## 🎯 Objectives

* 🛒 Develop a smart trolley with an automatic billing mechanism.
* 📡 Identify products using RFID technology.
* 💰 Calculate the total bill automatically.
* 🖥️ Display product information and total price on an LCD.
* ➕ Add products to the shopping bill through RFID scanning.
* ➖ Remove products and decrease the total cost.
* 📱 Send the generated bill/message using GSM communication.
* 🔔 Provide visual and audio feedback through LEDs and buzzer.
* ⚡ Build a low-cost and practical embedded systems prototype.

---

## ✨ Key Features

### 📡 RFID-Based Product Detection

The **EM-18 RFID module** reads the unique ID of RFID tags attached to products.

### 💰 Automatic Bill Calculation

When a recognized product is scanned, its corresponding price is added to the running total.

### 🖥️ Real-Time LCD Display

The LCD displays the scanned product information and the updated total bill.

### ➕ Product Addition

Scanning a recognized product adds it to the current shopping bill.

### ➖ Product Removal

The system provides a dedicated removal operation. By pressing and holding the **green push button** and scanning the product RFID tag, the selected item is removed and the total cost decreases.

### 📱 GSM Bill Notification

Using the **SIM800L GSM module**, the system can send the generated bill/text message to a configured mobile number.

### 🟢🔴 Status Indicators

* 🟢 **Green LED** → Recognized/authorized tag
* 🔴 **Red LED** → Unrecognized/unauthorized tag
* 🔔 **Buzzer** → Alert/error feedback

### 🔄 Continuous Operation

The system continuously monitors RFID tags and processes new scans while powered on.

---

## 🛠️ Technology Stack

| Category                   | Technology           |
| -------------------------- | -------------------- |
| 🔧 Microcontroller         | Arduino Nano         |
| 📡 RFID Reader             | EM-18 RFID Module    |
| 🏷️ Identification         | 125 kHz RFID Tags    |
| 🖥️ Display                | 20×4 LCD             |
| 📱 Communication           | SIM800L GSM/GPRS     |
| 💻 Programming             | Arduino / Embedded C |
| 🧰 Development Environment | Arduino IDE          |
| 🔔 Alert                   | Buzzer               |
| 💡 Indicators              | Red & Green LEDs     |
| 🎛️ Input                  | Push Buttons         |
| ⚡ Power Regulation         | Buck Converter       |
| 🔌 Interface               | I2C LCD Module       |

---

## 🔩 Hardware Components

| Component            | Quantity | Purpose                       |
| -------------------- | :------: | ----------------------------- |
| 🔧 Arduino Nano      |     1    | Main microcontroller          |
| 📱 SIM800L           |     1    | GSM communication             |
| 📡 EM-18 RFID Reader |     1    | RFID tag detection            |
| 🖥️ 20×4 LCD         |     1    | Product and bill display      |
| 🏷️ EM-18 RFID Tags  |     4    | Product identification        |
| 🔴 Red LED           |     1    | Error/unauthorized indication |
| 🟢 Green LED         |     1    | Valid/recognized indication   |
| 🔔 Buzzer            |     1    | Alert/feedback                |
| 🔌 I2C Module        |     1    | LCD interfacing               |
| 🔘 Push Buttons      |     2    | User input/control            |
| 🔋 3.7V Battery      |     1    | Power source                  |
| 🔗 Jumper Wires      |     —    | Circuit connections           |
| ⚡ Resistors          |     —    | Circuit protection/support    |

The component list and quantities are based on the hardware model documented in the project report.

---

## 🧩 Main Components

### 🔧 Arduino Nano

The Arduino Nano is the central controller of the project. It receives RFID data from the EM-18 module, processes the tag ID, manages the billing logic, controls the LCD and indicators, and communicates with the GSM module.

**Key specifications:**

* Microcontroller: **ATmega328P**
* Operating Voltage: **5V**
* Clock Speed: **16 MHz**
* Digital I/O: **14**
* Analog Inputs: **8**
* PWM Outputs: **6**
* Flash Memory: **32 KB**
* SRAM: **2 KB**
* EEPROM: **1 KB**

---

### 📡 EM-18 RFID Module

The **EM-18** is used for RFID tag detection.

It operates at **125 kHz** and provides the unique RFID tag ID through serial communication.

**Main features:**

* Operating frequency: **125 kHz**
* Supply voltage: **5V**
* Interface: UART / Serial
* Typical range: **5–10 cm**
* Output: Unique RFID tag ID

---

### 📱 SIM800L GSM Module

The **SIM800L** provides cellular communication between the smart trolley and a mobile phone.

It can be controlled by the Arduino through **AT commands** and supports GSM/GPRS functionality.

In this project, it is used to send the generated bill/text message to a mobile number.

---

### 🖥️ 20×4 LCD

The LCD is used to provide real-time information to the customer.

It can display:

* 🏷️ Product name
* 💰 Product price
* 🧾 Total bill
* ⚠️ Status messages
* 📡 RFID identification/status

The project report specifically documents the **20×4 LCD** as part of the hardware model.

---

## ⚙️ Working Principle

The complete system works through the following process:

```text
                 🛒 Product
                     │
                     ▼
              🏷️ RFID Tag
                     │
                     ▼
              📡 EM-18 Reader
                     │
                     ▼
              🔧 Arduino Nano
                     │
          ┌──────────┼───────────┐
          │          │           │
          ▼          ▼           ▼
       🖥️ LCD     💡 LEDs     🔔 Buzzer
          │
          ▼
      💰 Bill Update
          │
          ▼
      📱 SIM800L
          │
          ▼
      📲 SMS / Bill
```

---

## 🔄 System Workflow

### 1️⃣ Power Supply

The system is powered by a controlled **5V DC supply**, with voltage regulation provided for the Arduino Nano and EM-18 RFID module.

### 2️⃣ System Initialization

When powered on, the Arduino Nano initializes communication with the EM-18 RFID module and prepares the connected components.

### 3️⃣ RFID Tag Detection

When an RFID tag enters the EM-18 reader's detection range, the tag responds with its unique identification number.

### 4️⃣ Data Transmission

The EM-18 module sends the detected tag ID to the Arduino Nano through **UART serial communication**.

### 5️⃣ Data Processing

The Arduino compares the received tag ID with previously stored product information.

### 6️⃣ Product Addition

If the RFID tag is recognized, the corresponding product name and price are displayed on the LCD and the price is added to the total bill.

### 7️⃣ Product Removal

To remove an item, the user presses and holds the **green push button** and scans the item's RFID tag. The system displays the removed-item message and decreases the total bill.

### 8️⃣ Status Feedback

The system provides feedback using:

```text
🟢 Green LED  → Recognized Tag
🔴 Red LED    → Unrecognized Tag
🔔 Buzzer     → Alert / Error
🖥️ LCD        → Status & Billing Information
```

### 9️⃣ Bill Generation

After shopping, the generated bill can be sent to a mobile number using the **SIM800L GSM module**.

### 🔟 Continuous Operation

The system continues running in a loop and remains ready to process new RFID tags.

The hardware implementation and working sequence are documented in the project report.

---

## 🧠 Billing Logic

```text
              RFID TAG SCANNED
                     │
                     ▼
              Read Unique ID
                     │
                     ▼
          Is ID in Product List?
               /          \
             YES           NO
              │             │
              ▼             ▼
       Identify Product   🔴 Error
              │             │
              ▼             ▼
       Get Product Price  Buzzer/LED
              │
              ▼
        Add to Total Bill
              │
              ▼
         Display on LCD
```

### ➖ Removal Logic

```text
       Hold Green Button
              │
              ▼
        Scan RFID Tag
              │
              ▼
       Identify Product
              │
              ▼
       Remove from Bill
              │
              ▼
      Decrease Total Cost
              │
              ▼
        Update LCD
```

---

## 📱 GSM Bill System

The **SIM800L GSM module** provides cellular communication.

When the customer completes the shopping process, the system can send the generated bill/text message to the configured mobile number.

```text
🛒 Shopping Complete
        ↓
🧾 Generate Bill
        ↓
🔧 Arduino Nano
        ↓
📱 SIM800L GSM
        ↓
📡 Cellular Network
        ↓
📲 Customer Mobile
```

The report demonstrates this functionality through the yellow push-button operation described in the results section.

---

## 🔌 Circuit Diagram

<p align="center">
  <img src="images/circuit-diagram.png" alt="Smart Trolley Circuit Diagram" width="900">
</p>

### 🔗 Major Connections

```text
EM-18 RFID
    │
    │ UART
    ▼
Arduino Nano
    │
    ├──────────► 20×4 LCD
    │
    ├──────────► Green LED
    │
    ├──────────► Red LED
    │
    ├──────────► Buzzer
    │
    ├──────────► Push Buttons
    │
    └──────────► SIM800L
                     │
                     ▼
                GSM Network
```

---

## 🖥️ Hardware Output

### 🏷️ Product Scanning

When a product RFID tag is scanned, the LCD displays the **product name and price**, while the total bill is updated.

<p align="center">
  <img src="images/product-scan.jpg" alt="Product RFID Scanning Output" width="700">
</p>

### ➖ Product Removal

When the removal operation is activated and the product RFID tag is scanned, the system displays the removed-item message and decreases the total cost.

<p align="center">
  <img src="images/item-removal.jpg" alt="Item Removal Output" width="700">
</p>

### 📱 GSM Bill Message

The GSM module can send the generated bill/text message to the customer's mobile number.

<p align="center">
  <img src="images/gsm-bill.jpg" alt="GSM Bill Message" width="700">
</p>

The report documents these three hardware-model operations in its results section.

---

## 📊 Results

Real-time testing of the hardware model was carried out using the **Arduino Nano and EM-18 RFID module**.

The system successfully:

* 📡 Read RFID tag IDs.
* 🔧 Processed the received RFID data.
* 🖥️ Displayed tag/product information on the LCD.
* 🟢 Indicated recognized tags using the green LED.
* 🔴 Indicated unrecognized tags using the red LED.
* 🔔 Provided alert feedback through the buzzer.
* ➕ Added scanned products to the bill.
* ➖ Removed products and decreased the total cost.
* 📱 Sent the generated bill/text message through GSM.

The report describes the prototype as successfully implemented and tested in continuous operation.

---

## 💻 Software Setup

The project uses the **Arduino IDE** for programming and uploading the Arduino sketch.

### 🔧 Required Software

* Arduino IDE
* Arduino Nano board package
* Appropriate COM port
* USB connection/programmer

### 🚀 Uploading the Program

1. Install **Arduino IDE**.
2. Connect the Arduino Nano to the computer.
3. Open Arduino IDE.
4. Select:

```text
Tools → Board → Arduino Nano
```

5. Select the appropriate COM port:

```text
Tools → Port → COMx
```

6. Open the project sketch.
7. Compile the program.
8. Click **Upload**.
9. Wait for the **Done Uploading** message.

The report documents Arduino IDE setup, board selection, COM-port configuration, compilation, and sketch uploading.

---

## 📂 Project Structure

```text
Smart-Trolley-Automatic-Billing/
│
├── 📄 README.md
│
└── 📁 documentation/
    └── 📄 mini-project-report.pdf
```

> 📌 Rename the image filenames above according to the actual files in your repository.

---

## 🎯 Skills Demonstrated

* 🔧 Embedded Systems
* 💻 Arduino Programming
* 📡 RFID Integration
* 🖥️ LCD Interfacing
* 📱 GSM Communication
* 🔌 UART / Serial Communication
* 💰 Billing Logic
* 🔘 Push-Button Interfacing
* 💡 LED Interfacing
* 🔔 Buzzer Interfacing
* ⚡ Power Management
* 🧩 Hardware Integration
* 🧪 Prototype Testing
* 🛠️ Circuit Implementation

---

## 🌍 Applications

The technologies demonstrated in this project can be applied to:

* 🛒 Smart Shopping Trolleys
* 🏪 Supermarkets
* 🏬 Retail Stores
* 📦 Inventory Management
* 👥 Attendance Monitoring
* 🔐 Access Control
* 🤖 RFID-Based Automation Systems
* 📱 GSM-Based Notification Systems

The report also identifies inventory management, attendance monitoring, and access control as applications of the RFID-based system.

---

## 🔮 Future Scope

The project can be further extended by integrating additional technologies such as:

* 🌐 IoT-based inventory management
* 📱 Mobile application integration
* 💳 Digital/contactless payment
* ⚖️ Weight sensors for item verification
* 📷 Computer vision
* 🎙️ Voice recognition
* 🖥️ Touchscreen interface
* 📡 Advanced wireless communication

These technologies are discussed in the report as techniques or possible extensions of smart-trolley systems.

---

## 📚 Learning Outcomes

This project provided practical exposure to:

* 📡 RFID-based identification
* 🔧 Arduino Nano microcontroller programming
* 🖥️ LCD interfacing
* 📱 GSM communication
* 🔌 UART serial communication
* 💡 LED and buzzer control
* 🔘 Push-button input handling
* 💰 Real-time billing logic
* ⚡ Hardware integration
* 🧪 Hardware testing and debugging

---

## 🏆 Project Highlights

<div align="center">

|  🔧 Hardware | ⚡ Function             |
| :----------: | :--------------------- |
| Arduino Nano | Main Controller        |
|     EM-18    | RFID Detection         |
|   20×4 LCD   | Product & Bill Display |
|    SIM800L   | GSM Bill Communication |
|   Green LED  | Valid Tag Indicator    |
|    Red LED   | Invalid Tag Indicator  |
|    Buzzer    | Alert Feedback         |
| Push Buttons | User Control           |

</div>

---

## 👥 Project Team

### 👩‍💻 Paridhi Agrawal

**ECE | PSIT Kanpur**

### 👩‍💻 Mishthi Chaurasia

**ECE | PSIT Kanpur**

### 👨‍💻 Mradul Singh

**ECE | PSIT Kanpur**

**Department:** Electronics & Communication Engineering
**Institute:** Pranveer Singh Institute of Technology, Kanpur
**Session:** 2024–25

The team members and project details are taken from the submitted mini-project report.

---

## 📄 Project Documentation

📘 **Mini Project Report:**
`Smart Trolley with Automatic Billing System`

The complete report covers the project overview, automation techniques, hardware components, Arduino programming, implementation, testing, results, cost analysis, conclusion, and future scope.

---

<div align="center">

## 🛒 Scan • Calculate • Remove • Pay • Shop

### 📡 Smart Shopping through Embedded Automation

⭐ **Built with Arduino Nano + EM-18 RFID + LCD + SIM800L**

</div>
