# 💳 Payment Gateway System (C++ | Low-Level Design)

> A scalable Payment Gateway System built in **C++** demonstrating **Low-Level Design (LLD)** principles and multiple **Design Patterns** including Factory, Strategy, Proxy, Singleton, and Template Method.

![C++](https://img.shields.io/badge/C%2B%2B-17-blue?style=for-the-badge&logo=c%2B%2B)
![OOP](https://img.shields.io/badge/OOP-Design-orange?style=for-the-badge)
![LLD](https://img.shields.io/badge/Low--Level-Design-success?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

# 📌 Overview

This project simulates how modern payment gateways (such as **Paytm**, **Razorpay**, etc.) process payments while maintaining a clean, extensible, and maintainable architecture.

The system is designed so that **new payment providers can be added without changing existing business logic**, following the **Open-Closed Principle (SOLID)**.

---

# ✨ Features

- ✅ Supports multiple payment gateways
- ✅ Easy integration of new payment providers
- ✅ Standardized payment workflow
- ✅ Payment validation
- ✅ Payment confirmation
- ✅ Retry mechanism using Proxy
- ✅ Clean Object-Oriented Design
- ✅ Extensible architecture
- ✅ Demonstrates multiple Design Patterns

---

# 🏗️ System Architecture

The project is divided into multiple layers:

```
Client
   │
   ▼
PaymentController
   │
   ▼
PaymentService
   │
   ▼
GatewayFactory
   │
   ▼
PaymentGateway
   │
   ▼
Banking System
```

---

# 📊 UML Class Diagram

> UML Design

![UML Diagram](images/uml.png)

---

# 📋 Requirements

The system was designed with the following requirements:

- Support multiple payment providers
- Easily add new gateways
- Standard payment processing flow
- Validation before payment
- Error handling
- Retry mechanism

Future Improvements:

- Linear Retry Strategy
- Exponential Backoff
- Recurring Payments
- Subscription Billing

---

# 🧩 Design Patterns Used

## 🏭 Factory Pattern

Creates the appropriate payment gateway at runtime.

```
GatewayFactory
        │
        ├── PaytmGateway
        └── RazorpayGateway
```

---

## 🎯 Strategy Pattern

Different banking systems implement different payment processing strategies.

```
BankingSystem
      ▲
      │
 ┌────┴─────┐
 │          │
Paytm     Razorpay
```

---

## 🛡 Proxy Pattern

Adds retry functionality without modifying the original payment gateway.

```
Client
   │
Proxy
   │
Real Gateway
```

---

## 🔒 Singleton Pattern

Used for:

- PaymentService
- GatewayFactory
- PaymentController

Ensures only one instance exists throughout the application.

---

## 📝 Template Method Pattern

Provides a common payment flow:

```
Validate
     │
     ▼
Initiate
     │
     ▼
Confirm
```

while allowing individual gateways to customize implementation.

---

# 📂 Project Structure

```
PaymentGatewayApplication/
│
├── PaymentGatewayApplication.cpp
├── README.md
├── .gitignore
│
└── images/
    ├── uml.png
    └── requirements.png
```

---

# ⚙️ Payment Flow

```
User

  │

PaymentController

  │

PaymentService

  │

GatewayFactory

  │

Selected Gateway

  │

Validate Payment

  │

Initiate Payment

  │

Process via Banking System

  │

Confirm Payment

  │

Success / Failure
```

---

# 🚀 Supported Payment Providers

- ✅ Paytm
- ✅ Razorpay

Adding another provider requires only:

- Creating a new gateway
- Creating a new banking system
- Registering it inside `GatewayFactory`

No existing business logic needs modification.

---

# 🧠 OOP Concepts Demonstrated

- Encapsulation
- Abstraction
- Inheritance
- Polymorphism
- Composition
- Dependency Injection

---

# 📚 SOLID Principles

✔ Single Responsibility Principle

✔ Open Closed Principle

✔ Liskov Substitution Principle

✔ Interface Segregation Principle

✔ Dependency Inversion Principle

---

# 🔮 Future Enhancements

- Stripe Integration
- PayPal Integration
- UPI Support
- Wallet Support
- Payment Logs
- Transaction History
- REST API Version
- Database Integration
- JWT Authentication
- Unit Testing
- Docker Support
- CI/CD Pipeline

---

# 🛠 Tech Stack

- C++
- Object-Oriented Programming
- Low-Level Design
- Design Patterns

---

# 📷 Project Images

## UML Diagram

![UML](images/uml.png)

---

## Requirements

![Requirements](images/requirements.png)

---

# ⭐ Learning Outcomes

This project helped in understanding:

- Low-Level Design
- Object-Oriented Design
- Design Patterns
- Scalable Software Architecture
- Extensible System Design
- SOLID Principles
- Dependency Management

---

# 👨‍💻 Author

**Manav Redhu**

B.Tech (Artificial Intelligence & Data Science)

GitHub: https://github.com/manavredhu

---

## ⭐ If you like this project, consider giving it a Star!
