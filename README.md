# 💼 Karma Sync

**Karma Sync** is a modern, lightweight **Agile Project Management Suite** designed for both individuals and teams. It empowers users to manage personal and collaborative projects, track issues using a Kanban board, and stay productive with a built-in daily to-do tracker — all from one streamlined dashboard.

> Frontend Repo: [karmasync_frontend](https://github.com/bsurajpatra/karmasync)  
> Backend Repo: [karmasync_backend](https://github.com/bsurajpatra/karmasync_backend)


---

## 🚀 Features

### 🧠 Project Management
- Create **Personal** and **Collaborative** projects
- Visual **Kanban Board** to manage tasks: To-Do → Doing → Done
- Add and assign issues within projects
- Roles in collaborative projects:
  - **Project Manager**: Full control over tasks and collaborators
  - **Developer**: Limited to viewing and updating assigned tasks
- Collaborator management: Add/Remove members, assign roles

### ✅ Personal Daily To-Dos
- Dedicated dashboard for managing personal daily tasks
- Add task name, priority, category, and due date
- Organize work, health, study, and custom routines
- Edit, delete, and mark tasks as done
- Search and filter your task list easily

### 🔐 Authentication & Security
- JWT-based secure login
- OTP validation for new account creation
- Forgot password recovery via email

### 📬 Mailing Service
- **Sending Mails (OTP verification, Forgot Password, etc.):**  
  Implemented using **Gmail SMTP** via the backend server. This handles system-generated emails securely.
- **Receiving Messages (Contact Us form submissions):**  
  Managed through **[EmailJS](https://www.emailjs.com/)** from the frontend, allowing direct message delivery without server-side handling.

#### 📄 `.env` Setup

**Backend (`.env`):**
```env
EMAIL_USER=yourgmail@gmail.com
EMAIL_PASS=your-app-password
PORT=
MONGODB_URI=
JWT_SECRET=
FRONTEND_URL=
```

**Frontend (`.env`):**
```env
REACT_APP_API_URL=
REACT_APP_EMAILJS_SERVICE_ID=
REACT_APP_EMAILJS_TEMPLATE_ID=
REACT_APP_EMAILJS_PUBLIC_API=
```

### 👤 Profile Management
- View and update user profile
- Manage credentials and preferences

### 📞 Contact & Support
- Integrated **Contact Us** section for feedback and help
- All user queries are routed via EmailJS to our support team

---

## 🛠️ Tech Stack

- **Frontend**: React + Vite
- **Backend**: Node.js + Express (MVC Pattern)
- **Database**: MongoDB Atlas (Free Tier)
- **Authentication**: JWT, Email OTP
- **Mailing**: Gmail SMTP (Send) + EmailJS (Receive)

---

## 📦 Installation Guide

### 🔧 Frontend Setup

```bash
git clone https://github.com/bsurajpatra/karmasync_frontend.git
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

---

## 🤝 Contributing

- Bug reports and suggestions are welcome via GitHub Issues
- Open to contributions — fork the repo and create a pull request

---

## 📫 Contact

📧 Email: [ankitsuraj1111@gmail.com](mailto:ankitsuraj1111@gmail.com)

---

## 📃 License

Licensed under the [MIT License](https://opensource.org/licenses/MIT) — use freely with attribution.
