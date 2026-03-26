# 🏦 ATM Simulator System (Java + MySQL)

## 📌 Overview

ATM Simulator System is a desktop-based banking application built using **Java Swing** and **MySQL**.
It simulates real ATM functionalities like account creation, deposit, withdrawal, and balance enquiry.

---

## 🚀 Features

* 📝 Account Registration (3-step form)
* 💰 Deposit Money
* 💸 Withdraw Money
* 📄 Mini Statement
* 🔐 PIN Change
* 💳 Balance Enquiry

---

## 🛠 Tech Stack

* **Frontend:** Java Swing
* **Backend:** Java (JDBC)
* **Database:** MySQL

---
## 📸 Screenshots

### 🔐 Login Screen

<img width="995" height="597" alt="image" src="https://github.com/user-attachments/assets/c606d861-2ca9-4839-bcda-4f9d12155d54" />
### 📝 Signup Page
<img width="1044" height="993" alt="image" src="https://github.com/user-attachments/assets/e3dc4e07-772d-4595-a940-440f71facac6" />
<img width="1054" height="934" alt="image" src="https://github.com/user-attachments/assets/0f4cfa3d-1c4e-4091-bb31-c758c9656b41" />
<img width="1041" height="1007" alt="image" src="https://github.com/user-attachments/assets/af50daf0-4692-47e0-aed2-a1623d4c4169" />
<img width="1045" height="1008" alt="image" src="https://github.com/user-attachments/assets/3c2e4b84-995f-47e9-8def-1b13cc09ca57" />

### 💰 Deposit Screen
<img width="1145" height="1027" alt="image" src="https://github.com/user-attachments/assets/afbc7160-bed0-464d-b230-f20f362952a5" />
<img width="1187" height="1022" alt="image" src="https://github.com/user-attachments/assets/999e317f-d1ad-43f3-8173-f59dc995c88e" />


### 📄 Mini Statement
<img width="1202" height="1023" alt="image" src="https://github.com/user-attachments/assets/8b560f27-c6a9-4a1c-b5ec-3456cfe35752" />
<img width="1205" height="1020" alt="image" src="https://github.com/user-attachments/assets/44a8cfaa-7f2d-499e-8e42-3ab80504fe97" />
<img width="1182" height="1024" alt="image" src="https://github.com/user-attachments/assets/f4c69dfe-1130-47b8-898f-d9f1ce597b7d" />
<img width="1187" height="1017" alt="image" src="https://github.com/user-attachments/assets/9cda7cf9-3f1a-45c3-8e02-846411ea1095" />

<img width="1200" height="1023" alt="image" src="https://github.com/user-attachments/assets/252bf025-f23d-4151-a246-56fed70149f8" />
<img width="483" height="749" alt="image" src="https://github.com/user-attachments/assets/e4bf6b2b-56cc-4b8a-8b27-88704cf61741" />

---

## ⚙️ How to Run

### 1️⃣ Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/ATM_Simulator_using_JAVA.git
```

### 2️⃣ Setup Database

Open MySQL and run:

```sql
create database bankmanagementsystem;
use bankmanagementsystem;

create table signup(
formno varchar(20), name varchar(20), father_name varchar(20),
dob varchar(20), gender varchar(20), email varchar(30),
marital_status varchar(20), address varchar(40),
city varchar(25), pincode varchar(20), state varchar(25)
);

create table signuptwo(
formno varchar(20), religion varchar(20), category varchar(20),
income varchar(20), education varchar(20), occupation varchar(20),
pan varchar(20), aadhar varchar(20),
seniorcitizen varchar(20), existingaccount varchar(20)
);

create table signupthree(
formno varchar(20), accountType varchar(40),
cardnumber varchar(25), pin varchar(10), facility varchar(100)
);

create table login(
formno varchar(20), cardnumber varchar(25), pin varchar(10)
);

create table bank(
pin varchar(10), date varchar(50),
type varchar(20), amount varchar(20)
);
```

---

### 3️⃣ Configure Database Connection

Edit `Conn.java`:

```java
Connection c = DriverManager.getConnection(
    "jdbc:mysql://localhost:3306/bankmanagementsystem",
    "root",
    "YOUR_PASSWORD"
);
```

---

### 4️⃣ Run Project

Run:

```
Login.java
```

---


## 📦 Download & Run

👉 You can also run using JAR file (if provided)

```
java -jar ATM-Simulator.jar
```

---

## 👨‍💻 Author

* **Your Name**

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!
