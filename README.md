# IndoStock - Design and Build of a Warehouse Inventory Management Database System

IndoStock is a prototype of a warehouse inventory management information system based on a Relational Database Management System (RDBMS), specifically designed for the Indomaret modern minimarket case study. This project integrates five master data entities (Employees, Categories, Shelves, Suppliers, Products) with three main transactional entities (Goods In, Goods Out, Goods Return).

The system is built using Microsoft Access as the database engine and Visual Basic for Applications (VBA) as the logic for dynamic interface control.

## 🚀 Key System Features
- **Dynamic Role-Based Authorization (VBA):** Restricts navigation menu access rights in real time. Accounts with the *Pramuniaga* role are automatically locked out of administrative menus (Employee Data, Suppliers, and Reports), while the *Store Leader* has full authorization.
- **Metric Calculation & Aggregation Automation (SQL):** Automatic calculation of cumulative physical stock balances through RDBMS aggregate functions as goods in and goods out transactions occur, to eliminate the risk of *human error*.
- **Anomaly Prevention Validation System:** Implementation of mathematical control logic to absolutely block transactions if the quantity of outgoing goods exceeds the physical warehouse stock balance (*Insufficient Stock*).
- **Referential Integrity & Delete Anomaly Prevention:** Robust database relationship configuration without triggering *Cascade Delete*, in order to preserve the safety of the transactional logistics audit trail (*audit trail*).
- **Context-Sensitive Help System:** Integration of an interactive digital help file (.chm) created with HelpNDoc, which can be invoked directly from the dashboard sidebar interface using the Windows API.

## 📁 Repository Structure
- `/Database`: Contains the physical database prototype file `IndoStock.accdb`.
- `/Aplikasi_Manual`: Contains the interactive digital help file `manual.chm` that is directly integrated with the system help button inside the application.

## 🎓 Publication & Testing Results
This project has been presented and comprehensively tested using the *Black-Box Testing* method. An in-depth theoretical and technical analysis of the system has been documented in our group's scientific article, which has a *Similarity Index* of **5% (Turnitin)**.

- **Official Scientific Article:** Available for open access through the academic repository on [ResearchGate]().

## 👥 Development Team (Class of 2025B)
This project was built as a final assignment for the Database course, Information Systems Study Program, Universitas Negeri Surabaya, by:
1. Muhromin (Project Leader & System Analyst)
2. Yasmin Nur Fadila (System Designer)
3. Inka Nadia Faridiani (Implementer)
4. Muhammad Nadhif Afkar (Documentation)