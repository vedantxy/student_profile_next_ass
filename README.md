# Student Profile Directory

A Next.js web app for browsing student profiles, departments, and academic details.

## Features

- **Student listing** — Browse all enrolled students on the home page
- **Student detail page** — View individual student profiles with academic info, enrolled subjects, and contact details
- **Department listing** — Browse all departments and their specializations
- **Department detail page** — View students filtered by department/specialization track
- **404 page** — Custom not-found page with navigation links

## Tech Stack

- [Next.js 16](https://nextjs.org/) — App Router
- [React 19](https://react.dev/)
- [TypeScript](https://www.typescriptlang.org/)
- [Tailwind CSS v4](https://tailwindcss.com/)

## Project Structure

```
app/
  page.tsx                         # Home — student listing
  layout.tsx                       # Root layout with nav
  globals.css                      # Global styles
  not-found.tsx                    # 404 page
  department/
    page.tsx                       # Department listing
    [department]/page.tsx          # Department detail by ID
  studentData/
    [student]/page.tsx             # Student detail by ID
data/
  studentData.js                   # Student records array
  departmentData.js                # Department/specialization records
```

## Getting Started

Install dependencies:

```bash
npm install
```

Run the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Available Scripts

| Script | Description |
|--------|-------------|
| `npm run dev` | Start the dev server |
| `npm run build` | Build for production |
| `npm run start` | Start the production server |
| `npm run lint` | Run ESLint |

## Data

Student and department data lives in the `data/` directory as plain JS arrays. To add or modify records, edit:

- `data/studentData.js` — student profiles (id, name, department, subjects, etc.)
- `data/departmentData.js` — department specializations and enrolled student IDs
