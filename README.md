# 💼 Karma Sync

**Karma Sync** is a modern, lightweight **Agile Project Management Suite** designed for both individuals and teams. It empowers users to manage personal and collaborative projects, track issues using a Kanban board, and stay productive with a built-in daily to-do tracker — all from one streamlined dashboard.

> Frontend Repo: [karmasync_frontend](https://github.com/bsurajpatra/karmasync)  
> Backend Repo: [karmasync_backend](https://github.com/bsurajpatra/karmasync_backend)

---

## 🌟 Key Highlights

- Manage **personal and collaborative projects**
- Visual **Kanban board** for issue tracking
- **Sprint & User Story management**
- Built-in **daily to-do tracker**
- **Project Activity Log** for transparency
- **@Mentions in issue comments** for collaboration
- Secure authentication with email workflows

---

## 🧠 Project Management

### Projects
- Create **Personal** and **Collaborative** projects
- Role-based access:
  - **Project Manager** – Full control
  - **Developer** – Assigned-task access
- Add / remove collaborators
- Assign roles dynamically

### Kanban Board
- Issue workflow:
  - **To-Do → Doing → Done**
- Drag-and-drop task movement
- Status updates tracked automatically

---

## 🏃 Sprint Management

- Organize work into **Sprints**
- Sprint statuses:
  - Planned
  - Active
  - Completed
  - Cancelled

### Sprint Rules
- Create/edit sprints only in **Planned** state
- Add/remove tasks in **Planned** and **Active** states
- Automatic cleanup when sprint is **Completed** or **Cancelled**
- Clear sprint lifecycle visibility

---

## 📘 User Stories

User Stories bridge planning and execution.

### Story Structure
- Title & description
- Status:
  - Draft
  - Ready
  - In Progress
  - Done
- Optional sprint assignment
- Multiple associated tasks

### Automatic Progress Tracking
- Progress bar calculated from task completion
- Tasks inherit sprint context from their parent story

---

## ✅ Issues & Tasks

- Create and assign issues/tasks
- Independent task creation
- Optional linking to user stories
- Task tagging for:
  - Priority
  - Technology
  - Workflow
- Advanced filtering & search

---

## 💬 Issue Comments & @Mentions

- Comment on issues for collaboration
- Tag project members using `@username`
- Mentions are:
  - Parsed and validated on backend
  - Highlighted in the UI
  - Stored explicitly (no fragile text-only parsing)

> 🔔 Mentions are notification-ready, but **do not trigger notifications yet** (by design).

---

## 🧾 Project Activity Log

A centralized **Activity Log** tracks **who did what and when** within a project.

### Logged Events Include
- Task status changes
- Kanban movements
- Sprint lifecycle updates
- Story updates
- Member additions / role changes
- Issue comments (event-level only)

### Design Principles
- Service-level logging (not controller-based)
- Human-readable descriptions
- No activity spam
- No full content snapshots

### Project Overview Activity Widget
- Displays recent project activity (last 5–10 events)
- Same view for all project members
- Lightweight, read-only widget
- Optional "View all activity" modal

> 📌 This is **project-wide activity**, not user-specific notifications.

---

## ✅ Personal Daily To-Dos

- Dedicated dashboard for personal productivity
- Add:
  - Task name
  - Priority
  - Category
  - Due date
- Organize:
  - Work
  - Health
  - Study
  - Custom routines
- Edit, delete, mark complete
- Search & filter tasks easily

---

## 🔐 Authentication & Security

- JWT-based authentication
- OTP verification during signup
- Forgot password recovery via email
- Secure credential handling

---

## 📬 Mailing System (Intentionally Limited)

Emails are sent **only for critical events**:

- New account creation (OTP)
- Welcome email
- Forgot password
- Added to a project

❌ No emails for:
- Task updates
- Comments
- Activity
- Notifications

This avoids inbox fatigue and keeps communication intentional.

---

## 👤 Profile Management

- View and update user profile
- Manage credentials and preferences

---

## 📞 Contact & Support

- Integrated **Contact Us** form
- Messages handled via **EmailJS** from frontend
- No server-side inbox exposure

---

## 🛠️ Tech Stack

### Frontend
- React

### Backend
- Node.js
- Express.js (MVC architecture)

### Database
- MongoDB Atlas (Free Tier)

### Authentication & Security
- JWT
- Email OTP verification

### Mailing
- Gmail SMTP (system emails)
- EmailJS (contact form)

---

## 📦 Installation Guide

### 🔧 Frontend Setup

```bash
git clone https://github.com/bsurajpatra/karmasync.git
cd karmasync_frontend
npm install
npm run dev
```

### 🔧 Backend Setup

```bash
git clone https://github.com/bsurajpatra/karmasync_backend.git
cd karmasync_backend
npm install
npm start
```

### 🔑 Environment Configuration

#### Backend (`.env`)

```env
EMAIL_USER=yourgmail@gmail.com
EMAIL_PASS=your-app-password
PORT=5000
MONGODB_URI=your-mongodb-connection-string
JWT_SECRET=your-secret-key
FRONTEND_URL=http://localhost:3000
```

#### Frontend (`.env`)

```env
REACT_APP_API_URL=http://localhost:5000
REACT_APP_EMAILJS_SERVICE_ID=your-service-id
REACT_APP_EMAILJS_TEMPLATE_ID=your-template-id
REACT_APP_EMAILJS_PUBLIC_API=your-public-key
```

---

## 🤝 Contributing

- Bug reports and suggestions are welcome via GitHub Issues
- Open to contributions — fork the repo and create a pull request

---

## 📫 Contact

📧 Email: [ankitsuraj1111@gmail.com](mailto:ankitsuraj1111@gmail.com)

---

## 📃 License

Licensed under the [MIT License](https://github.com/bsurajpatra/KarmaSync_Info/blob/main/LICENSE) — use freely with attribution.
