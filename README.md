# PlacementIQ — AI-Powered Placement & Interview Platform

> **Tagline:** Prepare smarter. Practice better. Get placement-ready.

PlacementIQ is a production-quality, SaaS web application built with **React, TypeScript, Vite, Tailwind CSS, and Recharts**. It connects the complete student placement workflow into one unified, data-driven journey:

```
Profile → Resume Analysis → Skill Analysis → Skill Gap → Learning Roadmap → AI Mock Interview → Interview Feedback → Job Matching → Applications → Placement Readiness
```

---

## 🌟 Key Features

### 1. Student Placement Preparation Suite
- **Interactive Dashboard (`/dashboard`):** 
  - Placement Readiness Composite Score (81/100, +8% trend).
  - 5-Pillar Competency Radar Chart (Recharts).
  - Upcoming tasks with interactive completion toggles.
  - Recommended job opportunities matched by verified skill overlap.
  - Recent activity timeline.
- **My Profile (`/profile`):**
  - Personal Information, Education (CGPA, Degree, Graduation), and Target Role selector.
  - Interactive skill chips with proficiency indicators and dynamic skill additions.
- **AI Resume Analyzer (`/resume`):**
  - Drag-and-drop PDF upload with 5MB validation.
  - Multi-stage simulated AI parsing: skills extraction, ATS scoring, keyword density, and formatting.
  - ATS Score Gauge (86/100 Excellent) with 7-section breakdown bars.
  - Detailed Strengths, Actionable Improvements, and interactive Google X-Y-Z rewrite modal.
- **Skill Gap Benchmarking (`/skill-gap`):**
  - Compare verified skills against industry benchmarks for target roles (React Developer, Full Stack, etc.).
  - Qualified, Developing, and Missing indicators with gap percentage calculation.
- **Personalized Learning Roadmap (`/roadmap`):**
  - Multi-week curriculum tracking with progress bar.
  - Curated resources (docs, video tutorials, practice problems).
  - Interactive status controls (*Start Week*, *Mark Complete*, *Reset*).
- **AI Mock Interview (`/interview`, `/interview/session`, `/interview/report`):**
  - Configurable setup: Role, Type (Technical, HR, Behavioral, Resume-based), Difficulty (Easy/Medium/Hard), Question counts.
  - Live AI interviewer session with timer, progress bar, large answer area, and simulated voice input.
  - Instant AI evaluation: Technical Accuracy, Relevance, Completeness, Communication, What You Did Well, Improve This, and Suggested Answer Structure.
  - Final Celebration Report with Recharts horizontal bar chart, strong areas, and recommended topics.
  - **Interview History (`/interview-history`):** Historical logs linking directly back to performance reports.
- **Smart Job Matches & Details (`/jobs`, `/jobs/:id`):**
  - Job search, workplace mode tabs (Remote, Hybrid, On-site), and sort filters.
  - Transparent match calculations (Skills, Experience, Education) with matched/missing skill chips.
  - 1-Click application submission.
- **Applications Kanban Tracker (`/applications`):**
  - 7-Stage drag-and-drop Kanban board: *Saved, Applied, Assessment, Interview, Shortlisted, Offer, Archived*.
  - Alternate table list view.
- **Notification Center (`/notifications`):**
  - Dropdown badge & full notification log with category icons and direct actions.
- **Settings & Preferences (`/settings`):**
  - Appearance (Light / Dark / System mode persisted in localStorage).
  - Notification toggles, recruiter privacy controls, and danger zone account reset modal.

---

### 2. Institutional Admin Portal (`/admin`, `/admin/students`, `/admin/jobs`, `/admin/analytics`)
- **Admin Command Center:** High-level metrics (Total Students, ATS Ready, Interview Ready, Offers).
- **Interactive Visualizations:** Student readiness distribution bar chart, applications-to-offers trend line chart, and corporate skill demand.
- **Student Directory:** Searchable, filterable student table with individual diagnostic candidate cards.
- **Placement Drives Manager:** View, create, and manage campus drives and company openings.

---

### 3. Recruiter Portal (`/recruiter`, `/recruiter/jobs/create`, `/recruiter/applicants`)
- **Recruiter Dashboard:** Active jobs, received applications, shortlisted count, and scheduled rounds.
- **Applicant Pipeline:** Candidate cards showcasing Resume ATS score, Mock Interview score, and Skill Match percentage with 1-click shortlisting.
- **Job Drive Creator:** Structured posting form with React Hook Form + Zod schema validation.

---

## 🛠️ Tech Stack & Architecture

- **Framework:** React 18 + TypeScript + Vite
- **Routing:** React Router DOM v6 with lazy loading and protected route abstractions
- **Styling:** Tailwind CSS with custom Indigo/Navy (`primary`) and Violet AI (`ai`) palette
- **Charts & Data Viz:** Recharts (RadarChart, BarChart, LineChart, AreaChart)
- **Forms & Validation:** React Hook Form + Zod resolvers
- **Icons:** Lucide React
- **Mock Data & Services:** Centralized data models in `src/data/` and asynchronous service layer in `src/services/` ready for real REST/GraphQL APIs.
- **Context State:** `AuthContext`, `ThemeContext`, `NotificationContext`, `ToastContext`.

---

## 🚀 Getting Started

### 1. Install Dependencies
```bash
npm install
```

### 2. Start Development Server
```bash
npm run dev
```

### 3. Production Build
```bash
npm run build
```

---

## 👤 Demo Evaluator Profiles
The application features a 1-click profile switcher on the Login page and in the top-right user menu:
- **Kanika Sharma (Student):** `kanika.sharma@example.com` / `password123`
- **Priya Patel (Recruiter):** `priya.patel@nexuswave.io` / `recruiter123`
- **Dr. Arvind Varma (Admin / Dean):** `arvind.varma@univ-placement.edu` / `admin1234`
"# PLACEMENTIQ" 
