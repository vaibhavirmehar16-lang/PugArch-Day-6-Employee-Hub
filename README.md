# PugWork. — People Ops, Simplified

<p align="center">
  <strong>A Modern Employee Management & Workforce Analytics Dashboard</strong>
</p>

<p align="center">
  <a href="https://pugarch-day-6-employee-hub.onrender.com/">
    <img src="https://img.shields.io/badge/Demo-Live%20on%20Render-4f46e5?style=for-the-badge&logo=render" alt="Live Demo"/>
  </a>
  <a href="https://github.com/vaibhavirmehar16-lang/PugArch-Day-6-Employee-Hub">
    <img src="https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github" alt="GitHub Repository"/>
  </a>
  <img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react" alt="React"/>
  <img src="https://img.shields.io/badge/TypeScript-5.7-3178C6?style=for-the-badge&logo=typescript" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/Vite-6-646CFF?style=for-the-badge&logo=vite" alt="Vite"/>
</p>

---

## 📌 Project Overview

**PugWork** is a modern People Operations and Workforce Analytics web application designed to simplify employee management and HR workflows through a unified, interactive dashboard.

Built with React, TypeScript, and Vite, the platform brings employee records, attendance tracking, payroll insights, training programs, and helpdesk inquiries together in a clean and responsive interface.

The application features a modern glassmorphic design, dynamic employee filtering, workforce analytics, attendance controls, and browser-based data persistence.

- **Live Demo:** [PugWork on Render](https://pugarch-day-6-employee-hub.onrender.com/)
- **GitHub Repository:** [PugArch Day 6 — Employee Hub](https://github.com/vaibhavirmehar16-lang/PugArch-Day-6-Employee-Hub)
- **Project Type:** Frontend Web Application
- **Deployment:** Render

## 🎯 Problem Statement

Traditional employee management workflows often rely on disconnected spreadsheets and outdated interfaces, making workforce information difficult to organize and analyze.

Common challenges include:

1. Finding employee records quickly across large directories.
2. Tracking employee attendance and employment status efficiently.
3. Understanding salary distribution across departments.
4. Managing employee training programs and internal support requests.
5. Generating useful workforce reports without manually processing data.
6. Maintaining a consistent and accessible experience across different screen sizes.

**Solution:** PugWork provides a centralized dashboard with interactive employee management, attendance controls, payroll analytics, training information, and helpdesk functionality.

## ✨ Features

### 1. 🔐 Login Interface

- Modern login interface with a glassmorphic design.
- Demo credential autofill.
- Show/hide password functionality.
- Remember-me option using browser storage.
- Login and logout interactions.

### 2. 👥 Employee Directory

- View employee details, including name, email, role, department, salary, and joining date.
- Search employees by name, role, or email.
- Filter records by department and employment status.
- Sort employees alphabetically or by salary.
- Add new employee records through a modal form.
- Persist employee records using browser `localStorage`.

### 3. 📊 Workforce Analytics

- Display workforce statistics and employee metrics.
- Calculate total payroll expenditure and average salary.
- Summarize employee counts and employment status.
- Present workforce information in an analytics-oriented dashboard.

### 4. 🎓 Training Management

- Display available training programs.
- View trainers, departments, enrollment counts, and program status.
- Track training completion percentages.

### 5. ⏰ Attendance Management

- Interactive clock-in and clock-out controls.
- Display attendance records and timestamps.
- Categorize attendance as Present, Late, or Remote.

### 6. 💰 Payroll Analytics

- Calculate total salary expenditure.
- Compare payroll distribution across departments.
- Display department-level salary metrics.
- Derive average salary figures from employee records.

### 7. 🎫 Helpdesk & Employee Inquiries

- Display employee support tickets.
- Categorize inquiries into Payroll, Leave, Hardware, and General.
- Toggle ticket status between Open and Resolved.
- Display support information in an organized interface.

### 8. 📥 Data Export

- Export employee information to a CSV file.
- Support basic workforce reporting and data portability.

### 9. 🎨 Modern User Interface

- Clean, dashboard-oriented layout.
- Glassmorphism-inspired visual styling.
- Responsive layouts using CSS Grid and Flexbox.
- Interactive icons powered by Lucide React.
- Reusable React components and typed data structures.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Frontend Framework | React 19 |
| Programming Language | TypeScript 5.7 |
| Build Tool & Development Server | Vite 6 |
| Styling | CSS, CSS Grid, Flexbox, glassmorphism |
| Icons | Lucide React |
| State Management | React Hooks (`useState`, `useEffect`, `useMemo`) |
| Browser Persistence | Web Storage API (`localStorage`) |
| Data Modeling | TypeScript interfaces and types |
| Version Control | Git and GitHub |
| Deployment | Render |

## 🏗️ Architecture

PugWork follows a **client-side Single Page Application (SPA) architecture**. React manages the interface and application state, while TypeScript provides structured data models and type checking.

### Architecture Flow

```text
              User Interaction
                     |
                     v
             React User Interface
                     |
                     v
             Application Logic
             /       |        \
            v        v         v
       Employee   Attendance  Payroll &
       Directory  & Tickets   Analytics
            |
            v
       React State
            |
            v
     Browser localStorage
            |
            v
      Persistent Employee Data
```

### Project Structure

```text
PugArch-Day-6-Employee-Hub/
├── index.html
├── package.json
├── package-lock.json
├── vite.config.ts
├── tsconfig.json
├── react-app/
│   └── src/
│       ├── App.tsx
│       ├── main.tsx
│       ├── index.css
│       ├── mockData.ts
│       └── types.ts
└── README.md
```

- **`App.tsx`** — Main application interface, React state, event handlers, filtering, calculations, and dashboard functionality.
- **`main.tsx`** — Application entry point.
- **`index.css`** — Global styles and interface styling.
- **`mockData.ts`** — Initial employee records.
- **`types.ts`** — TypeScript interfaces and types for employees, training programs, attendance, and inquiry tickets.
- **`package.json`** — Project dependencies and development scripts.
- **`vite.config.ts`** — Vite configuration.

## 🗄️ Database Design

PugWork currently uses **browser `localStorage` and in-memory React state**, rather than a traditional backend database.

### Employee Data Model

| Field | Type | Description |
|---|---|---|
| `id` | String | Unique employee identifier |
| `name` | String | Employee name |
| `role` | String | Job title |
| `department` | String | Employee department |
| `status` | String | Active, On Leave, or Inactive |
| `salary` | Number | Employee salary |
| `email` | String | Employee email address |
| `joinDate` | String | Employee joining date |

### Data Persistence

- Initial employee records are loaded from `mockData.ts`.
- Saved employee records are retrieved from `localStorage` when the application initializes.
- Changes to employee records are synchronized with browser storage through `useEffect`.
- Attendance, training, and ticket information currently use predefined sample data and React state.

**Important:** Browser storage is specific to the user's browser and origin. It is not a shared database and does not provide server-side access control or synchronization between users.

## 🔌 API Documentation

**No custom backend API is currently implemented.**

The application operates primarily on the client side using local data and browser APIs.

| Operation | Implementation |
|---|---|
| Fetch initial employees | `INITIAL_EMPLOYEES` from `mockData.ts` |
| Read saved employees | `localStorage.getItem()` |
| Save employee records | `localStorage.setItem()` |
| Manage interface state | React Hooks |
| Export employee data | Client-side CSV generation |

There are no custom REST endpoints, authentication APIs, or server-side database queries in the current implementation.

## ⚙️ Installation

### Prerequisites

Install the following before running the project:

- [Node.js](https://nodejs.org/) — preferably an active LTS release.
- npm, which is included with Node.js.
- [Git](https://git-scm.com/).
- A code editor such as [Visual Studio Code](https://code.visualstudio.com/).

### Step 1: Clone the Repository

```bash
git clone https://github.com/vaibhavirmehar16-lang/PugArch-Day-6-Employee-Hub.git
```

### Step 2: Open the Project Directory

```bash
cd PugArch-Day-6-Employee-Hub
```

### Step 3: Install Dependencies

```bash
npm install
```

### Step 4: Start the Development Server

```bash
npm run dev
```

Open the local URL displayed in the terminal, usually:

```text
http://localhost:5173/
```

### Step 5: Create a Production Build

```bash
npm run build
```

To preview the production build locally:

```bash
npm run preview
```

## 🔑 Environment Variables

The current frontend implementation does not require custom environment variables or API keys.

| Variable | Required | Purpose |
|---|---|---|
| None | No | The current application runs without custom environment configuration. |

If a backend, external API, or database is introduced in a future version, environment variables can be configured for those services.

**Security note:** Never place private API keys, passwords, or other secrets in frontend code or publicly exposed Vite environment variables.

## ▶️ How to Run

After completing installation:

1. Open the project directory in your terminal.
2. Run `npm install` if dependencies have not been installed.
3. Execute `npm run dev`.
4. Open the local development URL in your browser.
5. Explore the employee directory, analytics, training, attendance, payroll, and inquiry sections.
6. Use the available employee-management controls to interact with the dashboard.

### Demo Login

The application includes a demo login interface with prefilled credentials.

- **Email:** `admin@workforce.com`
- **Password:** `admin123`

Use these only for the demonstration interface. The current client-side login flow is not production-grade authentication and should not be used to protect real employee data.

## 🚀 Deployment

The project is deployed on Render.

- **Live Application:** [https://pugarch-day-6-employee-hub.onrender.com/](https://pugarch-day-6-employee-hub.onrender.com/)
- **Source Repository:** [https://github.com/vaibhavirmehar16-lang/PugArch-Day-6-Employee-Hub](https://github.com/vaibhavirmehar16-lang/PugArch-Day-6-Employee-Hub)

For a static-site deployment, configure the build command and publish directory according to the actual Vite configuration. The usual Vite output directory is `dist`; verify the build output before configuring deployment.

## 🖼️ Screenshots
<img width="1332" height="583" alt="image" src="https://github.com/user-attachments/assets/ccfa97d9-d0c2-44ac-8fb3-48a879ebd73a" />
<img width="1337" height="589" alt="image" src="https://github.com/user-attachments/assets/da1d4921-d576-4d12-9554-3bb164b017b5" />
<img width="1330" height="595" alt="image" src="https://github.com/user-attachments/assets/6e1dafd3-d972-4878-8861-f8a1a9f5f5f5" />
<img width="1335" height="589" alt="image" src="https://github.com/user-attachments/assets/077cd08a-d573-4ded-9fdf-e438cf2676d0" />
<img width="1338" height="588" alt="image" src="https://github.com/user-attachments/assets/5ae90462-fe5b-4e94-bf29-10633821ef7e" />
<img width="1331" height="593" alt="image" src="https://github.com/user-attachments/assets/d0189e0d-3151-4a86-925a-209360c63743" />
<img width="1336" height="592" alt="image" src="https://github.com/user-attachments/assets/45f7d6c8-61d4-4b32-ba3d-ecf27f25c29e" />
<img width="1340" height="594" alt="image" src="https://github.com/user-attachments/assets/6173d7fa-eb6e-4d73-90c1-ebdfa24ad3bf" />

## 🧩 Challenges Faced

### 1. Managing Multiple Dashboard Sections

Keeping employee records, attendance, payroll, training, and support tickets organized within a single application required clear separation of data and interface state.

### 2. Dynamic Employee Filtering and Sorting

Combining search terms, department filters, employment status filters, and sorting options required coordinated filtering and transformation of employee records.

### 3. Maintaining Data After Refresh

React state resets on a page reload unless the data is persisted elsewhere. Employee records therefore needed browser-based persistence.

### 4. Consistent Type-Safe Data Models

Different dashboard sections required different fields and status values, making structured data definitions important.

### 5. Workforce Calculations

Payroll totals, average salaries, and employee counts needed to be derived consistently from the employee data.

## ✅ Solutions

- Used React Hooks to manage application state and synchronize saved employee data.
- Defined TypeScript interfaces and types for employees, training programs, attendance records, and support tickets.
- Used derived calculations and filtering logic to update displayed results dynamically.
- Stored employee changes in `localStorage` for persistence across page reloads in the same browser.
- Used reusable styling patterns, CSS Grid, Flexbox, and Lucide React icons to create a consistent dashboard interface.
- Used Vite for local development and production builds.

## 🔮 Future Improvements

- **Backend Integration:** Add a Node.js/Express backend with a REST API.
- **Database:** Integrate PostgreSQL, MySQL, or MongoDB for centralized employee data.
- **Secure Authentication:** Implement server-side authentication, role-based access control, and secure session management.
- **Real Attendance System:** Add server-side attendance records, timestamps, and reporting.
- **Advanced Analytics:** Add charts, department comparisons, workforce trends, and more detailed payroll reports.
- **Employee Profiles:** Introduce editable profiles, profile photos, and detailed employment history.
- **Training Management:** Support enrollment, course assignments, and completion tracking.
- **Helpdesk Enhancements:** Add ticket creation, assignment, priority levels, and activity history.
- **Data Validation:** Improve form validation and error handling.
- **Automated Testing:** Add unit tests and end-to-end tests.
- **Accessibility:** Improve keyboard navigation, semantic markup, and screen-reader support.
- **CI/CD:** Add automated build checks and deployment workflows through GitHub Actions.

## 📚 Learning Outcomes

This project provides practical experience with:

- Building a React application using functional components and Hooks.
- Using TypeScript interfaces and types to model application data.
- Managing UI state and browser-based persistence.
- Implementing search, filtering, sorting, and data calculations.
- Creating responsive dashboard layouts with CSS.
- Using Git and GitHub for source control.
- Building and deploying a frontend application with Vite and Render.

## 👨‍💻 Author

**Project:** PugWork — People Ops, Simplified

**Repository:** [PugArch Day 6 — Employee Hub](https://github.com/vaibhavirmehar16-lang/PugArch-Day-6-Employee-Hub)

**Live Demo:** [Open PugWork](https://pugarch-day-6-employee-hub.onrender.com/)

---

<p align="center">
  Built with React, TypeScript, and Vite.
</p>

<p align="center">
  If you find this project useful, consider giving the repository a ⭐ on GitHub.
</p>
