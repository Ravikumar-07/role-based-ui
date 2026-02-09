# Role-Based Navbar & UI Access Control (React)

## 📌 Project Overview
This project demonstrates a **Role-Based Navigation and UI Access Control System** built using **React and React Router**.  
The application dynamically renders navigation menus and restricts page access based on the logged-in user’s role.

It is designed to reflect **real-world enterprise applications** such as HRMS, ATS, Admin Dashboards, and Portals.

---

## 🎯 Key Features
- Role-based dynamic navbar rendering
- Protected routes using permission logic
- Separate dashboards for Admin, HR, and Candidate
- Unauthorized access handling
- Centralized authentication state using Context API
- Clean and scalable project structure
- Built using modern React (Vite + React Router v6)

---

## 👥 User Roles & Access

| Role | Visible Menus | Accessible Routes |
|----|----|----|
| Admin | Admin Panel | `/admin` |
| HR | HR Dashboard | `/hr` |
| Candidate | Job Applications | `/candidate` |

✔ Menus are shown dynamically  
✔ Routes are protected from unauthorized access  
✔ Direct URL access is restricted  

---

## 🧠 How Role-Based Access Works

1. User logs in and selects a role
2. Role is stored in global state using Context API
3. Navbar renders menu items based on the user role
4. Routes are protected using a `ProtectedRoute` component
5. Unauthorized users are redirected to an error page
6. Root route (`/`) redirects users to their role-specific dashboard

---
