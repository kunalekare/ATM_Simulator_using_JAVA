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

## 📸 Screenshots

### 🔐 Login Screen

![Login](<img width="995" height="597" alt="image" src="https://github.com/user-attachments/assets/c606d861-2ca9-4839-bcda-4f9d12155d54" />
)

### 📝 Signup Page

![Signup](screenshots/signup.png)

### 💰 Deposit Screen

![Deposit](screenshots/deposit.png)

### 📄 Mini Statement

![Mini Statement](screenshots/mini.png)

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
