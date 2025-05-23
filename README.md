# J2ee_Bussiness_LAB3
The repository to complete a lab 3  for J2EE Components


# 💼 CanSecure Bank – EJB Banking System

A Java EE banking application built using **EJB**, **JPA**, and **JSP**, deployed on **WildFly**. It supports customer registration, account management, and basic banking operations like deposit, withdrawal, and balance checks.

---

## 🧭 Overview

This project demonstrates a modular Jakarta EE architecture using:

- **EJB** (Enterprise Java Beans) – Business logic
- **JPA** (Jakarta Persistence API) – ORM and DB access
- **JSP + Servlet** – Frontend and request handling
- **WildFly** – Application server

---

## 📊 Data Model

### `Customer`
- `customerId`: `Integer` (Primary Key)
- `name`: `String`
- `email`: `String`
- `accounts`: `List<Account>` (One-to-Many)

### `Account`
- `accountId`: `Integer` (Primary Key)
- `balance`: `double`
- `customer`: `Customer` (Many-to-One)

---

## 🛠️ JPA Configuration

The `persistence.xml` defines the persistence unit `BankPU`.

