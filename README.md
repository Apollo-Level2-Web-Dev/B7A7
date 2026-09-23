# 🚀 B7A7 Frontend (Fullstack) Project Assignment

> 💡 **Note:** This is a **frontend/fullstack-focused** assignment. You will build a robust, scalable, and visually appealing user interface using **Next.js**. You must consume a backend API (either your own from B7A6 or a provided one) and demonstrate proper architecture, state management, role-based access, and modern UI/UX best practices.

---

## 🔍 Find Your Assignment 

> 💡 Check your Student ID by clicking your **profile image** on the [Programming Hero Website](https://web.programming-hero.com/profile). The project domain **must match** your B7A6 Backend Assignment (or a mutually agreed-upon alternative).

| Last Digit of Student ID | Assignment Domain |
|:------------------------:|:------------------|
| **1** | **Courier & Logistics Platform** 🚚 |
| **2** | **Blood Donation & Emergency Platform** 🩸 |
| **3** | **Load Shedding & Power Management** ⚡ |
| **4** | **Developer Assessment Platform** 💻 |
| **5** | **Emergency Ambulance Dispatch** 🚑 |
| **6** | **Housing & Roommate Platform** 🏠 |
| **7** | **Field Service Management** 🔧 |
| **8** | **Project Management SaaS** 📋 |
| **9** | **University Management System** 🎓 |
| **0** | **City Complaint & Service Platform** 🏙️ |

> 💡 **Note:** Regular e-commerce clones or overly simplistic CRUD dashboards are **not allowed**. The UI must reflect the complexity of the domain, featuring distinct workflows for **3 distinct user roles**.

---

## ⚠️ Mandatory Requirements

> [!CAUTION]
> **MANDATORY - READ CAREFULLY**
> 
> The following requirements are **strictly mandatory**. Failure to complete any of these may result in significant mark deductions or **0 marks** for the affected section:
> 
> 1. **Next.js App Router Architecture**: Strict and justified use of **Server Components** (default) and **Client Components** (`"use client"`). Proper use of `layout.tsx`, `page.tsx`, `error.tsx`, and `loading.tsx`.
> 2. **Better UI/UX & Responsiveness**: Mobile-first, accessible, and modern design. Must use a utility-first CSS framework (Tailwind CSS) and a component library (e.g., shadcn/ui, Radix UI, or Mantine).
> 3. **Authentication & Authorization**: Secure login flow, protected routes (middleware), and **role-based UI rendering** (hiding/showing elements based on the 3 distinct roles).
> 4. **API Implementation & State Management**: Proper data fetching (TanStack Query / SWR or native Next.js caching), global state management (Zustand / Redux Toolkit / Context), loading skeletons, and error boundaries.
> 5. **Form Handling & Validation**: Use **React Hook Form + Zod** for all forms, ensuring frontend validation matches backend rules.
> 6. **Commits**: Minimum **20 meaningful** frontend commits with descriptive messages (e.g., `feat: add role-based sidebar`, `fix: resolve hydration mismatch`).
> 7. **Admin Credentials**: Provide working demo admin email and password for evaluation.
> 8. **Deployment**: Provide a working live frontend URL (e.g., Vercel, Netlify).
> 9. **Video Explanation**: Submit a 5–10 minute UI/UX and fullstack integration walkthrough video.

---

## 📊 Marks Distribution

| # | Category | Weight | Details |
|:-:|:---------|:------:|:--------|
| 1 | UI/UX Design & Responsiveness | 20% | Modern design, accessibility, mobile responsiveness, consistent theming |
| 2 | Next.js Architecture | 15% | Proper Server/Client component split, App Router features, layouts, error boundaries |
| 3 | Authentication & Authorization | 15% | Secure auth flow, middleware protection, role-based UI rendering (3 roles) |
| 4 | API Integration & State Management | 15% | Data fetching strategy, caching, global state, optimistic updates, loading states |
| 5 | Form Handling & Validation | 10% | React Hook Form + Zod, user-friendly error messages, complex form workflows |
| 6 | Performance & Optimization | 10% | Image optimization, lazy loading, code splitting, URL state management (`useSearchParams`) |
| 7 | Code Quality & Reusability | 5% | Component modularity, custom hooks, clean code, proper typing (TypeScript) |
| 8 | Deployment | 5% | Working production URL, environment variable configuration, CI/CD (optional bonus) |
| 9 | Commit History | 2% | 20+ meaningful frontend commits |
| 10 | Video Explanation | 3% | 5–10 minute UI/UX and integration walkthrough |
| **Total** | | **100%** | |

---

## 📋 Project Requirements

### 🛠️ Tech Stack

| Category | Technology | Purpose |
|----------|------------|---------|
| **Framework** | Next.js (App Router), TypeScript | Server-side rendering, routing, and type safety |
| **Styling & UI** | Tailwind CSS, shadcn/ui, Framer Motion (optional) | Rapid, responsive, and accessible UI development |
| **State Management** | TanStack Query (React Query) + Zustand / Context | Server-state caching and global client-state management |
| **Forms & Validation** | React Hook Form + Zod | Type-safe form handling and client-side validation |
| **Authentication** | NextAuth.js (Auth.js) or Custom JWT Cookies | Secure session management and protected routes |
| **Icons & Media** | Lucide React, Next/Image | Optimized icons and image delivery |
| **Deployment** | Vercel | Seamless frontend deployment with edge network |

### 🎯 Core Project Rules

- **Role-Based UI**: The application must have distinct views or dashboards for **3 fixed primary roles** (e.g., Customer, Provider, Admin). A user must only see what their role permits.
- **API Integration**: You must connect to a real backend API. Mock data is **NOT** accepted for core workflows.
- **URL State Management**: Filtering, sorting, and pagination must be reflected in the URL (e.g., `?page=2&status=active`) using `useSearchParams`, allowing users to share links.
- **Performance**: Use `next/image` for all images, implement skeleton loaders (`loading.tsx`), and avoid unnecessary client-side re-renders.
- **Error Handling**: Graceful error handling using `error.tsx` and toast notifications (e.g., Sonner or React Hot Toast) for API failures.

---

## 📅 Timeline: 5-Day Work Breakdown

> ⏱️ **Recommended Workload:** 5–8 hours per day. Consistency is key to building a polished UI and maintaining a clean Git history.

### 🟢 Day 1 — Planning, Setup & Design System
- [ ] Define the UI/UX requirements and user flows for all 3 roles.
- [ ] Initialize Next.js (App Router) + TypeScript + Tailwind CSS project.
- [ ] Set up UI component library (e.g., shadcn/ui) and define theme/colors.
- [ ] Create base layouts (`layout.tsx`), responsive sidebars/navbars, and routing structure.
- [ ] Configure environment variables for API base URLs.

### 🔵 Day 2 — Authentication & Protected Routes
- [ ] Implement Login, Register, and Logout UI flows.
- [ ] Set up authentication state (NextAuth or custom JWT cookies).
- [ ] Create Next.js Middleware (`middleware.ts`) for route protection and role-based redirects.
- [ ] Build the foundational dashboards for all 3 roles (skeleton/wireframe stage).

### 🟡 Day 3 — Core Features & API Integration
- [ ] Integrate TanStack Query (or native fetching) for data retrieval.
- [ ] Build core CRUD UI views (e.g., listing resources, viewing details).
- [ ] Implement **Pagination, Filtering, and Search** with URL state synchronization.
- [ ] Add loading skeletons (`loading.tsx`) and empty states for all data views.

### 🟠 Day 4 — Forms, Complex Workflows & Optimization
- [ ] Implement complex forms using React Hook Form + Zod (e.g., multi-step forms, file uploads).
- [ ] Add optimistic updates for actions like "liking", "status changes", or "comments".
- [ ] Implement global state (Zustand) for UI-specific states (e.g., sidebar toggle, multi-step wizard data).
- [ ] Optimize performance: audit bundle size, ensure proper `next/image` usage, and fix any hydration warnings.

### 🔴 Day 5 — Polish, Deployment & Submission
- [ ] Conduct rigorous UI testing across desktop, tablet, and mobile viewports.
- [ ] Deploy to Vercel and verify all environment variables and API connections work in production.
- [ ] Review Git history to ensure **20+ meaningful commits**.
- [ ] Record the 5–10 minute video walkthrough.
- [ ] Submit all required links in the assignment portal.

---

## 📦 What to Submit

Please format your submission exactly like this example:

```text
Project Name    : Courier & Logistics Platform
Frontend Repo   : https://github.com/your-username/courier-frontend
Live URL        : https://courier-frontend.vercel.app
Backend API     : https://courier-api.vercel.app (Link to your B7A6 or provided API)
Demo Video      : https://drive.google.com/file/d/xyz/view
Admin Email     : admin@courier.com
Admin Password  : ********
```

> ⚠️ **Security Warning:** Never submit personal passwords or production secrets. Create dedicated, secure demo credentials specifically for evaluation.

---

## 🎥 Video Explanation Guide

**Duration:** 5–10 minutes  
**Language:** English or Bengali  

**What to Cover:**
1. **Project Overview & UI/UX Philosophy**: Briefly explain the project, the design system used, and how the UI solves the user's problem.
2. **Next.js Architecture**: Point out specific examples of where you used Server Components vs. Client Components and why. Show your `layout.tsx` and `loading.tsx` in action.
3. **Authentication & Role-Based UI**: Log in as **Role 1** (e.g., Customer) and show their dashboard. Log out, then log in as **Role 2** (e.g., Admin) and demonstrate how the UI, navigation, and accessible routes change dynamically.
4. **API Integration & State**: Demonstrate a data-heavy page. Show the loading skeleton, the populated data, and use browser DevTools (Network tab) to show efficient API calls (e.g., TanStack Query caching).
5. **Form Validation & Error Handling**: Intentionally submit a form with invalid data to show Zod/React Hook Form error messages. Then, trigger an API error (e.g., disconnect network or use bad data) to show the graceful `error.tsx` or toast notification.
6. **Responsive Design**: Resize the browser window or use DevTools device mode to prove the application is fully responsive and mobile-friendly.

**Recording Options:**
- **Loom**: Record and share the link directly.
- **OBS**: Record and upload to Google Drive (ensure sharing is set to "Anyone with the link" → Viewer).

---

## 🧭 Project Idea Hub Reference

Your frontend must bring the **B7A6 Backend Project Ideas** to life. Refer to the [B7A6 Idea Hub](https://github.com/Apollo-Level2-Web-Dev/B7A6/blob/main/idea-hub.md) for domain-specific workflows. 

**Frontend-Specific Challenges to Consider:**
- **Complex Dashboards**: Data visualization (charts/graphs) for Admin roles.
- **Real-time Feel**: Optimistic UI updates for status changes (e.g., marking a task as "Done" instantly before the server responds).
- **Multi-step Workflows**: Wizard-style forms for complex creations (e.g., "Create Shipment" with multiple steps).
- **Advanced Filtering**: Faceted search UI with URL synchronization (e.g., e-commerce style filters).

> 🚀 **Final Goal:** Build a frontend that is not just a "dumb" API consumer. Your project should demonstrate a deep understanding of **Next.js architecture, modern UI/UX principles, robust state management, and seamless fullstack integration**. Build an interface you would be proud to put in your professional portfolio!
