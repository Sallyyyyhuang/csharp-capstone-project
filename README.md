# 🎓 MentorConnect — Mentorship Management Platform

> **Capstone Project** · Computer Information Systems (CIS) · Senior Year

A full-stack web application that connects mentees with mentors inside an organization. Mentees can browse and select mentors based on company reviews, while mentors can track and review their mentees' milestone progress — all from a single, role-based platform.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

MentorConnect was built as a capstone project to solve a real-world problem: making internal mentorship programs easier to manage. Instead of relying on emails or spreadsheets, both mentors and mentees get a dedicated dashboard tailored to their role.

- **Mentees** can explore available mentors, read reviews left by colleagues, and request a mentor that fits their goals.
- **Mentors** can monitor each mentee's milestone projects and leave feedback to guide their development.

---

## ✨ Features

### For Mentees
- 🔐 Secure login and registration
- 🔍 Browse a list of available mentors with company-sourced reviews
- ⭐ Select a mentor based on ratings and expertise
- 📌 View and manage personal milestone projects

### For Mentors
- 🔐 Secure login and role-based access
- 👥 View all assigned mentees from a single dashboard
- ✅ Check and evaluate mentee milestone submissions
- 💬 Provide feedback and track progress over time

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | C# (.NET) |
| Framework | ASP.NET (MVC / Web API) |
| IDE | Visual Studio 2017 |
| Frontend | HTML, CSS, JavaScript (Razor Views) |
| Database | SQL Server (`.mdf`) |
| Version Control | Git / GitHub |

---

## 🚀 Getting Started

### Prerequisites

- [Visual Studio 2017](https://visualstudio.microsoft.com/) or later (with ASP.NET workload)
- [.NET Framework](https://dotnet.microsoft.com/) (version matching the project target)
- SQL Server or SQL Server Express (LocalDB is fine for development)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/accountmanager.git
   cd accountmanager
   ```

2. **Open the solution in Visual Studio**
   ```
   accountmanager.sln
   ```

3. **Restore NuGet packages**
   - In Visual Studio: `Tools → NuGet Package Manager → Restore Packages`
   - Or via CLI: `dotnet restore`

4. **Configure the database connection**
   - Open `Web.config` (or `appsettings.json`)
   - Update the `ConnectionStrings` section to point to your local SQL Server instance

5. **Apply database migrations / seed data** *(if applicable)*
   ```
   Update-Database
   ```
   in the Package Manager Console.

6. **Run the project**
   - Press `F5` in Visual Studio, or run:
   ```bash
   dotnet run
   ```

---

## 🖥 Usage

| Role | Login | What You Can Do |
|------|-------|-----------------|
| **Mentee** | Use your mentee credentials | Browse mentors → Read reviews → Select a mentor → Track milestones |
| **Mentor** | Use your mentor credentials | View assigned mentees → Review milestone projects → Provide feedback |

> Accounts are role-based. A mentor account will not see the mentor-selection screen, and a mentee account will not see the milestone review panel.

---

## 📁 Project Structure

```
accountmanager/
├── accountmanager/          # Main ASP.NET project
│   ├── Controllers/         # MVC controllers (Auth, Mentor, Mentee, Milestone)
│   ├── Models/              # Data models and ViewModels
│   ├── Views/               # Razor (.cshtml) pages
│   ├── wwwroot/             # Static assets (CSS, JS, images)
│   └── Web.config           # App configuration
├── accountmanager.sln       # Visual Studio solution file
└── README.md
```

## 🤝 Contributing

This is a capstone project, but feedback is always welcome!

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

This project is for academic purposes. Feel free to use it as a reference with attribution.

---

> Built with ❤️ as a CIS Senior Capstone Project
