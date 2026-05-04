# CuRiemCRM — Full Stack CRM Platform

> Manage clients, projects & tasks in one system.

---

## 🌐 Landing Page

The public-facing site where users can sign up or log in as **Admin**, **Employee**, or **Customer**. Includes a live workspace creation form with a 14-day free trial.

![Landing Page](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/2026-05-04_23-32-49.png)

---

## 🔐 Authentication — Users Database

All users are stored in the `auth_users` table with a BCrypt hashed password and a role: `ADMIN`, `EMPLOYEE`, or `CUSTOMER`. Login is secured with **JWT tokens**.

![Auth Users DB](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/2026-05-04_23-39-46.png)

---

## 📋 Leads Dashboard

Track all incoming leads with filters by status — New, Contacted, Qualified, Converted, Lost. View summary stats and edit or delete any lead from the table.

![Leads Dashboard](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/2026-05-04_23-36-24.png)

### Leads — Database Table

Stores lead info: name, email, company, status, source, agent, conversion date, deal status, and received amount.

![Leads DB](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/2026-05-04_23-37-02.png)

---

## 👥 Customers Dashboard

Displays all customers in a card layout showing status (Active / Closed), contact info, product, and contract value. Each card has a **View** button for full details.

![Customers Dashboard](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/2026-05-04_23-37-42.png)

### Customers — Database Table

Stores customer records: company, email, phone, address, plan, contract value, purchase date, and status.

![Customers DB](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/2026-05-04_23-38-33.png)

---

## ⚙️ Backend — Spring Boot

Built with **Java Spring Boot** following a clean layered architecture — Controllers, Services, Repositories, DTOs, and Entities. Security via **JWT + Spring Security RBAC**.

![Backend Controllers & DTOs](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/2026-05-04_23-40-24.png)

### Entities, Repositories & Security

All database entities (Lead, Customer, Employee, Orders, Feedback, etc.) mapped via JPA. Security layer includes JWT filter, custom user details, and role-based access control.

![Backend Entities & Security](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/2026-05-04_23-40-43.png)

---

## 🗄️ Database Schema

Full entity-relationship diagram showing all 20+ tables and their relationships across Leads, Customers, Projects, Tasks, Orders, Calendar, Support, and more.

![Database Schema](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/diagram.png)
