# ⚡ Electric Saving System (Python CLI Project)

A simple and practical **Electric Saving & Billing System** built using **Python**.

This project simulates electricity consumption tracking, monthly unit limits, over-usage penalties, and user authentication using a command-line interface.

It demonstrates real-world billing logic using core Python concepts such as classes, objects, lists, dictionaries, random number generation, and date-time handling.

---

## 🚀 Features

- 👤 User Registration System
- 🔐 Secure Login Authentication
- ⚡ Random Monthly Electricity Consumption Simulation
- 📊 Monthly Unit Limit Tracking
- 💰 Automatic Over-Usage Fee Calculation
- 🔄 Automatic Monthly Reset Detection
- 🗂️ In-Memory Data Storage (List of Dictionaries)
- 🧠 Object-Oriented Programming (OOP) Design

---

## 🛠️ Technologies Used

- Python 3
- datetime module
- random module
- Classes & Objects (OOP)
- Lists & Dictionaries
- Exception Handling

---

## 📂 Project Structure

```
Electric-Saving-System/
│
├── electric_system.py
└── README.md
```

---

## 🧠 System Design Overview

The system contains two main classes:

### 1️⃣ ElectricBill Class

Handles:

- Electricity usage tracking
- Remaining unit calculation
- Over-usage fee calculation
- Monthly reset logic
- Random usage generation

---

### 2️⃣ Security Class

Handles:

- User registration
- Login authentication
- Storing user data in memory
- Connecting user data to billing system

---

## 🗄️ Data Storage Structure

All users are stored in a list called `database`.

Example user structure:

```python
{
    "name": "John",
    "password": "1234",
    "usedUnits": 80,
    "monthlyLimit": 150,
    "lastReset": datetime.now()
}
```

---

## ⚙️ How the System Works

### 1️⃣ User Registration

- User provides name and password
- System checks if user already exists
- If not, user is stored in database

---

### 2️⃣ User Login

- User enters credentials
- System verifies login
- If successful:
  - Random electricity usage is generated
  - Monthly reset is checked
  - Units are updated
  - Usage report is displayed

---

## ⚡ Electricity Logic

### Monthly Unit Limit

Default monthly limit:

```
150 kWh
```

---

### Random Usage Simulation

Each login simulates:

```
30 – 200 kWh consumption
```

---

### Over-Usage Fee

If:

```
usedUnits > monthlyLimit
```

Then:

```
overUsedUnits = usedUnits - monthlyLimit
fee = overUsedUnits × 1.4
```

Example:

```
Used: 180
Limit: 150
Overused: 30
Fee: 30 × 1.4 = $42
```

---

### Monthly Reset Logic

System checks:

```
If current month ≠ lastReset month
```

If true:

- Units reset to 0
- New billing cycle starts

---

## 🖥️ Sample Menu

```
====================================
        ELECTRIC SAVING SYSTEM
====================================

1) Register as New User
2) Login as Existing User
3) Exit System
```

---

## ▶️ How to Run the Program

### Step 1: Check Python Installation

```
python --version
```

---

### Step 2: Run the Program

```
python electric_system.py
```

or

```
python3 electric_system.py
```

---

## 🧠 Concepts Practiced

- Object-Oriented Programming (OOP)
- Class methods and attributes
- Real-world billing simulation
- Date comparison logic
- Random data generation
- Input validation
- State management
- CLI system design

---

## 🎯 Learning Outcomes

After building this project, you understand:

- How to design multi-class systems
- How to simulate billing systems
- How to track monthly usage
- How to implement authentication logic
- How to manage in-memory databases
- How to apply penalty calculations

---

## 🔮 Future Improvements

- Save data permanently (JSON / Database)
- Add admin dashboard
- Add real-time billing history
- Add tariff tiers (different rates per unit range)
- Add graphical user interface (Tkinter)
- Convert to Web App (Flask / Django)
- Encrypt passwords
- Add consumption reports & analytics

---

## 👨‍💻 Author

Takundah Gorogodo  
CSE Student | System Developer | Problem Solver

---

## 📄 License

This project is open-source and created for educational purposes.  
Free to use and modify for learning.
