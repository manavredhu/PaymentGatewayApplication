<div align="center">

# 💳 Payment Gateway System

### 🚀 A Scalable Low-Level Design (LLD) Project in Modern C++

*Designed using SOLID Principles & Industry-Standard Design Patterns*

<p>

<img src="https://img.shields.io/badge/C%2B%2B-17-blue?style=for-the-badge&logo=c%2B%2B">

<img src="https://img.shields.io/badge/Low--Level-Design-success?style=for-the-badge">

<img src="https://img.shields.io/badge/OOP-Architecture-orange?style=for-the-badge">

<img src="https://img.shields.io/badge/Design%20Patterns-5-red?style=for-the-badge">

</p>

---

*A modular payment gateway simulation supporting multiple payment providers through extensible architecture and clean object-oriented design.*

</div>

---

# 🌟 Overview

This project simulates how modern payment gateway platforms such as **Paytm**, **Razorpay**, and future providers process online payments.

The architecture is designed to be **scalable**, **maintainable**, and **extensible**, allowing new payment providers to be integrated with minimal code changes.

Instead of writing a monolithic payment processor, this project follows **real-world software engineering practices** by separating responsibilities into independent components.

---

# ✨ Highlights

✅ Multiple Payment Providers

✅ Factory-based Gateway Selection

✅ Standardized Payment Flow

✅ Retry Mechanism (Proxy)

✅ Clean Object-Oriented Design

✅ SOLID Principles

✅ Highly Extensible Architecture

✅ Real-world Low-Level Design

---

# 🏛 System Architecture

<p align="center">

<img src="images/uml.png" width="100%">

</p>

---

# 📋 Requirements

<p align="center">

<img src="images/requirements.png" width="85%">

</p>

---

# ⚙️ Payment Workflow

```text
                User
                  │
                  ▼
        Payment Controller
                  │
                  ▼
         Payment Service
                  │
                  ▼
         Gateway Factory
                  │
       ┌──────────┴──────────┐
       │                     │
       ▼                     ▼
   Paytm Gateway      Razorpay Gateway
       │                     │
       ▼                     ▼
 Banking System      Banking System
       │                     │
       └──────────┬──────────┘
                  ▼
          Payment Confirmation
                  │
                  ▼
           Success / Failure
```

---

# 🧩 Design Patterns

| Pattern | Purpose |
|----------|----------|
| 🏭 Factory | Creates the appropriate payment gateway |
| 🎯 Strategy | Supports multiple payment providers |
| 🔒 Singleton | Ensures a single shared instance |
| 🛡 Proxy | Implements retry mechanism |
| 📝 Template Method | Standardizes payment workflow |

---

# 📂 Project Structure

```text
PaymentGatewayApplication
│
├── PaymentGatewayApplication.cpp
├── README.md
├── .gitignore
│
└── images
      ├── uml.png
      └── requirements.png
```

---

# 🚀 Supported Providers

| Gateway | Status |
|----------|--------|
| ✅ Paytm | Supported |
| ✅ Razorpay | Supported |
| ⏳ Stripe | Planned |
| ⏳ PayPal | Planned |

---

# 🎯 SOLID Principles Applied

✔ Single Responsibility Principle

✔ Open-Closed Principle

✔ Liskov Substitution Principle

✔ Interface Segregation Principle

✔ Dependency Inversion Principle

---

# 💡 OOP Concepts Used

- Encapsulation
- Abstraction
- Inheritance
- Polymorphism
- Composition
- Dependency Injection

---

# 🔄 Payment Lifecycle

```text
Validate Payment
        │
        ▼
Initialize Transaction
        │
        ▼
Gateway Processing
        │
        ▼
Bank Processing
        │
        ▼
Confirmation
        │
        ▼
Transaction Complete
```

---

# 📈 Extensibility

Adding a new payment provider requires only:

```text
✔ Create a new Banking System

✔ Create a new Payment Gateway

✔ Register it inside GatewayFactory

✔ No changes to existing business logic
```

This follows the **Open-Closed Principle**, making the architecture easy to scale.

---

# 🛠 Tech Stack

| Technology | Usage |
|------------|------|
| C++17 | Core Language |
| OOP | Software Design |
| LLD | Architecture |
| Design Patterns | Scalability |

---

# 🔮 Future Improvements

- Stripe Integration
- PayPal Integration
- UPI Support
- Wallet Support
- Subscription Payments
- Payment Analytics
- Transaction History
- Database Integration
- REST API
- Unit Testing
- Docker Support
- CI/CD Pipeline

---

# 🎓 Learning Outcomes

This project demonstrates practical understanding of:

- Low-Level Design
- Object-Oriented Programming
- Software Architecture
- SOLID Principles
- Factory Pattern
- Strategy Pattern
- Singleton Pattern
- Proxy Pattern
- Template Method Pattern

---

# 👨‍💻 Author

## Manav Redhu

**B.Tech — Artificial Intelligence & Data Science**

🌐 GitHub: https://github.com/manavredhu

---

<div align="center">

### ⭐ If you found this project interesting, consider giving it a Star!

*"Good software architecture is built by design, not by accident."*

</div>
