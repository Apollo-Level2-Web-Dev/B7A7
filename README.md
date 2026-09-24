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
> 2. **Modern UI/UX & Responsiveness**: Mobile-first, accessible, and modern design. Must use a utility-first CSS framework (Tailwind CSS/StyleX) and a component library (e.g., shadcn/ui, Radix UI, or Mantine).
> 3. **Authentication & Authorization**: Secure login flow, protected routes (middleware), and **role-based UI rendering** (hiding/showing elements based on the 3 distinct roles).
> 4. **One-Click Role Login**: Your login page must implement a clear, structured layout featuring distinct, one-click "Demo Login" buttons for each of the 3 roles (e.g., Admin, User, Provider).
> 5. **API Integration & State Management**: Proper data fetching (TanStack Query / SWR or native Next.js caching), global state management (Zustand / Redux Toolkit / Context), loading skeletons, and error boundaries.
> 6. **Form Handling & Validation**: Use **React Hook Form or `@tanstack/react-form` + Zod** for all forms, ensuring frontend validation matches backend rules.
> 7. **Payment Integration**: Must integrate the frontend flow for **Stripe** or **SSLCommerz** (Test Mode). Simulated/fake payments (e.g., "Cash on Delivery") are **NOT accepted**.
> 8. **Meaningful Commits**: Minimum **20 meaningful** frontend commits with descriptive messages (e.g., `feat: add role-based sidebar`, `fix: resolve hydration mismatch`).
> 9. **Demo Credentials**: Provide working demo email and password for the Admin role (and others, if 1-click login is not fully functional) for evaluation.
> 10. **Deployment**: Provide a working live frontend URL (e.g., Vercel, Netlify, Cloudflare).
> 11. **Video Explanation**: Submit a 5–10 minute UI/UX and fullstack integration walkthrough video.

---

## 📊 Marks Distribution

| # | Category | Weight | Details |
|:-:|:---------|:------:|:--------|
| 1 | UI/UX Design & Responsiveness | 20% | Modern design, accessibility, mobile responsiveness, consistent theming |
| 2 | Next.js Architecture | 15% | Proper Server/Client component split, App Router features, layouts, error boundaries |
| 3 | Authentication & Authorization | 15% | Secure auth flow, middleware protection, role-based UI rendering (3 roles) |
| 4 | API Integration & State Management | 15% | Data fetching strategy, caching, global state, optimistic updates, loading states |
| 5 | Form Handling & Validation | 10% | React Hook Form / `@tanstack/react-form` + Zod, user-friendly errors, complex workflows |
| 6 | Performance & Optimization | 10% | Image optimization, lazy loading, code splitting, URL state management (`useSearchParams`) |
| 7 | Code Quality & Reusability | 5% | Component modularity, custom hooks, clean code, proper typing (TypeScript) |
| 8 | Deployment | 5% | Working production URL, environment variable configuration, CI/CD (optional bonus) |
| 9 | Commit History | 2% | 20+ meaningful frontend commits |
| 10 | Video Explanation | 3% | 5–10 minute UI/UX and integration walkthrough |
| **Total** | | **100%** | |

---

## 📋 Project Requirements

> ⏱️ **Detailed Guidelines:** Please read the complete project requirements, tech stack, and API rules here:  
> 👉 [Project Requirements & API Guidelines](https://github.com/Apollo-Level2-Web-Dev/B7A7/blob/main/project-requirements.md)

---

## 📅 Timeline: 5-Day Work Breakdown

> ⏱️ **Recommended Schedule:** Maintain steady progress to avoid last-minute stress and ensure a clean Git history.  
> 👉 [View the 5-Day Work Breakdown](https://github.com/Apollo-Level2-Web-Dev/B7A7/blob/main/timeline-breakdown.md)

---

## 🗓️ Submission Deadlines

| Deadline | Maximum Marks |
|:---------|:-------------:|
| **October 10, 2026, 11:59 PM** | 60 Marks |

> [!IMPORTANT]
> **Note:** There will be **no 50-mark or 30-mark extended deadlines**. To ensure your eligibility and participation in **Job Placement Support** and **Reward Courses**, you must submit your assignment strictly within this deadline. Late submissions will not be accepted or graded.

---

## 📦 What to Submit

Please format your submission exactly like this example:

```text
Project Name            : Courier & Logistics Platform
Backend Repo            : https://github.com/your-username/courier-backend
Frontend Repo           : https://github.com/your-username/courier-frontend
Live Backend URL        : https://courier-api.vercel.app
Live Frontend URL       : https://courier-frontend.vercel.app
API Documentation       : https://courier-api.vercel.app/docs (Link to your B7A6 or provided API docs)
Demo Video              : https://drive.google.com/file/d/xyz/view
Demo Admin Email        : admin@courier.com
Demo Admin Password     : ********
```

> ⚠️ **Security Warning:** Never submit personal passwords or production secrets. Create dedicated, secure demo credentials specifically for evaluation.

---

## 🎥 Video Explanation Guide

**Duration:** 5–10 minutes  
**Language:** English or Bengali  

**What to Cover:**
1. **Project Overview & UI/UX Philosophy**: Briefly explain the project, the design system used, and how the UI solves the user's problem.
2. **Next.js Architecture**: Point out specific examples of where you used Server Components vs. Client Components and why. Show your `layout.tsx` and `loading.tsx` in action.
3. **Authentication & Role-Based UI**: Use the **One-Click Demo Login** to log in as **Role 1** (e.g., User) and show their dashboard. Log out, then log in as **Role 2** (e.g., Admin) and demonstrate how the UI, navigation, and accessible routes change dynamically.
4. **API Integration & State**: Demonstrate a data-heavy page. Show the loading skeleton, the populated data, and use browser DevTools (Network tab) to show efficient API calls (e.g., TanStack Query caching).
5. **Form Validation & Error Handling**: Intentionally submit a form with invalid data to show Zod error messages. Then, trigger an API error (e.g., disconnect network or use bad data) to show the graceful `error.tsx` or toast notification.
6. **Responsive Design**: Resize the browser window or use DevTools device mode to prove the application is fully responsive and mobile-friendly.

**Recording Options:**
- **Loom**: Record and share the link directly *(Recommended)*.
- **OBS**: Record and upload to Google Drive (ensure sharing is set to "Anyone with the link" → Viewer).

---

## 🧭 Project Idea Hub Reference

Your frontend must bring the **B7A6 Backend Project Ideas** to life. Refer to the [B7A6 Idea Hub](https://github.com/Apollo-Level2-Web-Dev/B7A6/blob/main/idea-hub.md) for domain-specific workflows. 

> 🚀 **Final Goal:** Build a frontend that is not just a "dumb" API consumer. Your project should demonstrate a deep understanding of **Next.js architecture, modern UI/UX principles, robust state management, and seamless fullstack integration**. Build an interface you would be proud to put in your professional portfolio!

---
