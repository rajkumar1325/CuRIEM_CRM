# CuRiemCRM — Full Stack CRM Platform

> Manage clients, projects & tasks in one system.

---

## 🌐 Login — Frontend

The public-facing site where users can sign up or log in as **Admin**, **Employee**, or **Customer**. Includes a live workspace creation form with a 14-day free trial.

![Login Frontend](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/login-frontend)

---

## 🔐 Login — Backend (Auth Users Database)

All users are stored in the `auth_users` table with a BCrypt hashed password and a role: `ADMIN`, `EMPLOYEE`, or `CUSTOMER`. Login is secured with **JWT tokens**.

![Login Backend](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/login-backend)

---

## 📋 Leads — Frontend

Track all incoming leads with filters by status — New, Contacted, Qualified, Converted, Lost. View summary stats and edit or delete any lead from the table.

![Leads Frontend](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/login-frontend)

### Leads — Backend (Database Table)

Stores lead info: name, email, company, status, source, agent, conversion date, deal status, and received amount.

![Leads Backend](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/leads-backend)

---

## 👥 Customer — Frontend

Displays all customers in a card layout showing status (Active / Closed), contact info, product, and contract value. Each card has a **View** button for full details.

![Customer Frontend](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/customer-frontend)

### Customer — Backend (Database Table)

Stores customer records: company, email, phone, address, plan, contract value, purchase date, and status.

![Customer Backend](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/customer-backend)

---

## ⚙️ Backend — API, Controllers & DTOs

Built with **Java Spring Boot**. This layer handles all incoming API requests, routes them to the right service, and returns structured responses via DTOs.

![DB API Controller DTO](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/DB-api,controller,dto)

### Backend — Enums, Repositories & More

All database entities (Lead, Customer, Employee, Orders, Feedback, etc.) mapped via JPA with their repositories and enums.

![DB Enum Repo](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/DB-enum,repo,etc)

### Backend — Security & Services

Security layer includes JWT filter, custom user details service, and role-based access control. Services contain all business logic.

![DB Security Service](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/DB-security,service)

---

## 🗄️ Database Schema

Full entity-relationship diagram showing all 20+ tables and their relationships across Leads, Customers, Projects, Tasks, Orders, Calendar, Support, and more.

![Database Schema](https://raw.githubusercontent.com/rajkumar1325/CuRIEM_CRM/main/Assets/diagram.png)
