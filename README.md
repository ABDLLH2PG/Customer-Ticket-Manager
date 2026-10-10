# 🎫 Customer Ticket Management System (OOP) 🚀

[ **🇸🇦 Read this project in Arabic** ](./README-AR.md)

A robust, console-based queue and ticketing application developed in **C++**. This project demonstrates the practical application of **Object-Oriented Programming (OOP)** alongside **Data Structures (Queues & Stacks)** to simulate a real-world ticketing system with automated wait time calculations.

---

## 🏗️ Project Modules & Features

### 1️⃣ Core Queue Operations 🚶‍♂️
- 🎟️ **Ticketing:** Issue sequential tickets with customized prefixes for different departments (e.g., A1, B2).
- ✅ **Client Service:** Serve the next client in line and automatically update the queue's state and statistics.
- 📊 **Monitoring:** Track Total Tickets, Served Clients, and Currently Waiting Clients in real-time.

### 2️⃣ Wait Time Estimation ⏳
- ⏱️ **Dynamic Calculations:** Automatically calculates the Expected Serve Time for each new ticket based on the department's average service time and the current queue size.
- 🕒 **Time Stamping:** Captures the exact issuance date and time for every ticket.
- 🔄 **Auto-Updating:** Automatically recalculates expected waiting times for remaining clients whenever a client is served.

### 3️⃣ Queue Visualization 👁️
- ➡️ **Directional Views:** View the entire queue visually formatted from Right-to-Left (RTL) or Left-to-Right (LTR).
- 🖨️ **Detailed Ticket Info:** Print comprehensive details for all active tickets in the line, simulating physical printed tickets.

---

## 💻 Code Architecture & OOP Design 🧬

### The Object-Oriented Paradigm
This project is built with clean architecture using advanced OOP concepts:
- **Nested Classes:** Utilizing an inner `clsTicket` class encapsulated entirely within the `clsQueueLine` class, restricting direct external access and maintaining high data security.
- **Encapsulation:** Protecting variables like `_TotalTickets` and `_AverageServeTime` using standard access modifiers and custom methods.
- **Modularity:** Passing custom configurations via constructors (Prefix, Average Serve Time) to generate independent queue lines (e.g., Pay Bills vs. Subscriptions).

---

## 🛠️ Key Technical Highlights ✨
- ⚙️ **Standard Template Library (STL):** 
  - Extensive use of `std::queue` for core First-In-First-Out (FIFO) queue logic.
  - Strategic use of `std::stack` to temporarily reverse data flow for visualizing the queue in LTR format.
- 🛡️ **Custom Libraries:** Integration of external custom classes like `clsDate` for accurate system datetime string generation.
- 🚀 **Memory Efficiency:** Safe updating and popping of objects in memory without memory leaks.
