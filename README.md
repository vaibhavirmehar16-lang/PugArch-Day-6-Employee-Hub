# PugWork. — People Ops, Simplified

[![Live Demo](https://img.shields.io/badge/Demo-Live%20on%20Render-4f46e5?style=for-the-badge&logo=render)](https://pugarch-day-6-employee-hub.onrender.com/)
[![GitHub Repo](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)](https://github.com/vaibhavirmehar16-lang/PugArch-Day-6-Employee-Hub/tree/main)
[![React 19](https://img.shields.io/badge/React-19.0.0-61dafb?style=for-the-badge&logo=react)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.7.2-3178c6?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-6.2.0-646cff?style=for-the-badge&logo=vite)](https://vitejs.dev/)

---

## 📌 Project Overview
**PugWork.** is an enterprise-grade People Operations and Workforce Analytics web platform tailored for modern HR teams. Featuring a high-end glassmorphic aesthetic, live attendance clocking, department payroll distribution calculations, interactive helpdesk ticket resolutions, and real-time personnel filters, PugWork bridges the gap between raw workforce data and operational insights.

* **Live Deployment:** [https://pugarch-day-6-employee-hub.onrender.com/](https://pugarch-day-6-employee-hub.onrender.com/)
* **Source Code Repository:** [https://github.com/vaibhavirmehar16-lang/PugArch-Day-6-Employee-Hub/tree/main](https://github.com/vaibhavirmehar16-lang/PugArch-Day-6-Employee-Hub/tree/main)

---

## 🎯 Problem Statement
Legacy human resource management systems often suffer from:
1. Cluttered, outdated enterprise user interfaces that hinder rapid record navigation.
2. Rigid monolithic data structures lacking client-side dynamic search and multi-parameter filtering.
3. Decoupled tracking where attendance shifts, support tickets, and payroll calculations exist across fragmented spreadsheets.

**PugWork.** solves this by delivering a lightweight, single-page reactive dashboard with cohesive workforce analytics, time-tracking logs, and payroll breakdowns in a modern, Gen-Z styled interface.

---

## ✨ Features

### 1. Enterprise Authentication & Security
* Glassmorphic login portal with architectural backdrop and subtle depth lighting.
* One-click demo credentials autofill (`admin@workforce.com`).
* Interactive password visibility toggle (Show/Hide) and 30-day session persistence via browser storage.

### 2. Live Employee Directory
* Real-time search by employee name, role, or email with zero network latency.
* Multi-parameter department filtering (`Engineering`, `Product`, `Design`, `HR`, `Marketing`).
* Employment status filtering (`Active`, `On Leave`, `Inactive`) with ascending/descending salary and alphabetical sorting.
* Modal dialogue to append custom employee records into persistent local storage.

### 3. Real-Time Shift & Time Tracking (Attendance)
* Interactive **Clock In / Clock Out** action toggle stamping current localized timestamps.
* Visual status categorization (`Present`, `Remote`, `Late`).

### 4. Automated Payroll & Finance Metrics
* Department-level dynamic budget calculation and total salary distribution metrics.
* Real-time derivation of monthly disbursements and per-employee departmental averages.

### 5. Helpdesk & Team Inquiries
* Ticket triage desk with categorization (`Hardware`, `Payroll`, `Leave`, `General`).
* Direct status toggle (`Open` ↔ `Resolved`) updating the sidebar's live notification badge.

### 6. Data Portability & Reporting
* Client-side CSV export generating formatted records of verified workforce details.

---

## 🛠️ Technology Stack

| Layer | Technologies |
| :--- | :--- |
| **Frontend Framework** | React 19 (Functional Components, Hooks) |
| **Language** | TypeScript (Strict Typing & Custom Interfaces) |
| **Tooling & Bundler** | Vite 6 |
| **Icons & Design Assets** | Lucide React |
| **Styling Paradigm** | Modern Inline CSS Modules, Glassmorphism, CSS Grid & Flexbox |
| **State & Persistence** | React State (`useState`, `useMemo`), Browser `localStorage` API |
| **Hosting & CI/CD** | Render (Static Site Deployment connected via GitHub Webhooks) |

---

## 🏗️ Architecture

PugWork follows a clean Single Page Application (SPA) reactive architecture: