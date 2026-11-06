# 🎓 LearnHub — Enterprise Learning Management System (LMS)

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Online-00c853?style=for-the-badge&logo=googlechrome&logoColor=white)](https://abdulqader-alshihabi.github.io/LearningHub/)
[![React 18](https://img.shields.io/badge/React-18.3-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.6-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-5.4-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Supabase](https://img.shields.io/badge/Supabase-PostgreSQL-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)](https://supabase.com/)
[![TanStack Query](https://img.shields.io/badge/TanStack_Query-v5-FF4154?style=for-the-badge&logo=react-query&logoColor=white)](https://tanstack.com/query)

> 🌐 **Live Interactive Web Demo:** [https://abdulqader-alshihabi.github.io/LearningHub/](https://abdulqader-alshihabi.github.io/LearningHub/)  
> 💡 *Features pre-configured seed data & offline fallback so you can test all features live with zero setup.*

**LearnHub** is a modern, high-performance, enterprise-grade Learning Management System (LMS) engineered for scalable online education. It delivers a seamless, interactive experience for students, instructors, and administrators with course authoring, multimedia streaming, quizzes, and automated progress tracking.

---

## ⚡ Instant Demo Access (One-Click for Evaluators)

When testing the application live, click the **Instant Demo Access** pills on the Login screen, or use these pre-configured credentials:

| Role | Demo Email | Password | Access Capabilities |
| :--- | :--- | :--- | :--- |
| **Student** | `student@demo.com` | `demo123456` | Browse catalog, enroll in courses, stream video lessons, take quizzes, track progress |
| **Instructor** | `instructor@demo.com` | `demo123456` | Course creation studio, lesson curriculum management, student analytics & earnings |
| **Admin** | `admin@demo.com` | `demo123456` | Platform moderation, course approval, system KPIs, dispute resolution |

---

## ✨ Core Features & Functional Architecture

### 1. Multi-Role Ecosystem & Granular Access (RBAC)
- **Student Dashboard:** Enrolled courses overview, continuous learning tracker, certificate generator, and personalized recommendations.
- **Instructor Portal:** Multi-step course creation wizard, video asset uploader, lesson sequencer, and quiz authoring builder.
- **Admin Control Center:** Platform governance, catalog auditing, instructor verification, and complaints panel.

### 2. Multimedia Interactive Course Player
- High-definition video player with speed controls, timestamps, and fullscreen preview.
- Integrated PDF reader for supplementary handouts and coding cheat-sheets.
- Real-time lesson discussion forum directly beneath every lesson.
- Automated progress percentage calculation with persistent state.

### 3. Interactive Quiz & Assessment Engine
- Time-managed assessments with multiple-choice questions.
- Instant grading, passing score validation, and detailed review breakdowns.

### 4. Resilient Offline & Seed Data Architecture
- Comes complete with production-ready **`supabase/seed.sql`** script containing realistic tech courses, instructors, lessons, and reviews.
- Built-in graceful fallback layer that ensures full demo responsiveness even when external database endpoints are in standby.

---

## 🏗️ Architecture & Component Hierarchy

```
LearnHub/
├── src/
│   ├── components/         # Reusable atomic UI components (Shadcn UI & Radix)
│   │   ├── instructor/     # Course builder wizards & curriculum editors
│   │   ├── ui/             # Design system tokens (buttons, modals, cards, tabs)
│   │   ├── VideoPlayer.tsx # Custom HTML5 & embedded video streaming player
│   │   ├── QuizPlayer.tsx  # Dynamic quiz renderer & evaluation engine
│   │   └── Navbar.tsx      # Responsive header with role-based navigation
│   ├── contexts/           # Global AuthContext with demo authentication shortcuts
│   ├── data/               # Seed data & fallback providers (courses, lessons, reviews)
│   ├── hooks/              # TanStack Query custom hooks (useCourses, useCategories)
│   ├── pages/              # Route views (Catalog, CourseDetails, Player, Dashboards)
│   └── integrations/       # Supabase client instantiation & TypeScript database types
└── supabase/
    ├── migrations/         # PostgreSQL schema migrations (tables, RLS, functions)
    └── seed.sql            # Rich seed database script
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ or Bun
- npm or yarn

### Installation & Local Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Abdulqader-Alshihabi/LearningHub.git
   cd LearningHub
   ```

2. **Install project dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```
   Open [http://localhost:5173](http://localhost:5173) in your browser.

4. **Production Build:**
   ```bash
   npm run build
   ```

---

## 🗄️ Database Setup (Optional for Custom Supabase)

If deploying to your own Supabase project:
1. Copy `.env.example` to `.env` and set `VITE_SUPABASE_URL` and `VITE_SUPABASE_PUBLISHABLE_KEY`.
2. Execute the migrations located in `supabase/migrations/` in your Supabase SQL editor.
3. Run `supabase/seed.sql` to populate sample categories, instructors, courses, and lessons.

---

## 👨‍💻 Author

**Abdulqader Alshihabi**  
*Computer Science Graduate • Software & AI Engineer*  
- GitHub: [@Abdulqader-Alshihabi](https://github.com/Abdulqader-Alshihabi)  
- Email: [abdulqader.moh.2003@gmail.com](mailto:abdulqader.moh.2003@gmail.com)  
