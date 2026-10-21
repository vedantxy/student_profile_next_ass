<div align="center">

# 🎓 Student Profile

### A modern student directory built with Next.js 16 & TypeScript

[![Next.js](https://img.shields.io/badge/Next.js-16.4.0-black?style=for-the-badge&logo=next.js&logoColor=white)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.3.0-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-4.x-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)

</div>

---

## 📌 About

**Student Profile** is a Next.js web application that lets you browse, filter, and view detailed profiles of students — organized by department and year. Built as a Next.js assignment showcasing file-based routing, dynamic segments, and component-driven UI.

---

## ✨ Features

- 📋 **Student Listing** — View all students in a clean card grid
- 🏛️ **Department Filter** — Browse students by their department
- 👤 **Student Detail Page** — Dedicated profile page for each student
- 🔗 **Dynamic Routing** — Uses Next.js App Router with `[department]` and `[student]` dynamic segments
- ⚡ **Fast & Lightweight** — Static data, no database needed

---

## 🗂️ Project Structure

```
student_profile_next_ass/
├── app/
│   ├── page.tsx                        # Home — all students listing
│   ├── layout.tsx                      # Root layout & metadata
│   ├── globals.css                     # Global styles
│   ├── not-found.tsx                   # Custom 404 page
│   ├── department/
│   │   ├── page.tsx                    # All departments listing
│   │   └── [department]/
│   │       └── page.tsx                # Students filtered by department
│   └── studentData/
│       └── [student]/
│           └── page.tsx                # Individual student profile
├── data/
│   ├── studentData.js                  # Student records
│   └── departmentData.js               # Department records
├── public/                             # Static assets
└── package.json
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have **Node.js 18+** installed.

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/vedantxy/student_profile_next_ass.git

# 2. Move into the project folder
cd student_profile_next_ass

# 3. Install dependencies
npm install
```

### Run Locally

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser. 🎉

---

## 📄 Pages Overview

| Route | Description |
|---|---|
| `/` | Home page — lists all students |
| `/department` | All departments |
| `/department/[id]` | Students filtered by department |
| `/studentData/[id]` | Individual student profile |

---

## 🛠️ Tech Stack

| Technology | Version | Purpose |
|---|---|---|
| Next.js | 16.4.0 | React framework & routing |
| React | 19.3.0 | UI library |
| TypeScript | 5.x | Type safety |
| Tailwind CSS | 4.x | Utility-first styling |
| ESLint | 9.x | Code linting |

---

## 📦 Scripts

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run start    # Start production server
npm run lint     # Run ESLint
```

---

<div align="center">

Made with ❤️ by **Vedant**

</div>
