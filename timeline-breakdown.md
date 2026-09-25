## 📅 Timeline: 5-Day Work Breakdown

> ⏱️ **Recommended Workload:** 5–8 hours per day. Consistency is key to building a polished UI, avoiding last-minute bugs, and maintaining a clean, meaningful Git history.  
> 💡 **Pro Tip:** Commit your code at the end of *every* day with descriptive messages to naturally hit the 20+ meaningful commits requirement.

### 🟢 Day 1 — Planning, Setup & Design System
- [ ] Review your B7A6 Backend API Documentation (Postman/Swagger) and map out UI/UX user flows for all **3 distinct roles**.
- [ ] Initialize Next.js (App Router) + TypeScript + Tailwind CSS project.
- [ ] Set up your UI component library (e.g., `shadcn/ui`) and define the global theme, typography, and color palette.
- [ ] Create base layouts (`layout.tsx`), responsive sidebars/navbars, and the foundational routing structure.
- [ ] Configure environment variables (`.env.local`) for backend API base URLs and payment gateway test keys.

### 🔵 Day 2 — Authentication & Protected Routes
- [ ] Implement Login, Register, and Logout UI flows.
- [ ] Set up authentication state management (NextAuth.js or custom JWT via HTTP-only cookies).
- [ ] Create Next.js Middleware (`proxy.ts` or `middleware.ts`) for route protection and role-based redirects.
- [ ] **Mandatory:** Implement the **One-Click Demo Login** buttons on the login page for all 3 roles (e.g., "Login as Admin", "Login as User").
- [ ] Build the foundational wireframe/skeleton dashboards for all 3 roles to establish the layout.

### 🟡 Day 3 — Core Features, API Integration & Dashboards
- [ ] Integrate TanStack Query (React Query) or native Next.js fetching for efficient data retrieval and caching.
- [ ] Build core CRUD UI views (e.g., listing resources, viewing detailed modals/pages).
- [ ] Implement **Pagination, Filtering, and Search** with strict URL state synchronization (`useSearchParams`).
- [ ] Add loading skeletons (`loading.tsx`), empty states, and global error boundaries (`error.tsx`) with toast notifications for all data views.
- [ ] Implement at least one **Data Visualization** component (e.g., Recharts/Chart.js) for the Admin/Manager dashboard.

### 🟠 Day 4 — Complex Workflows, Payments & Optimization
- [ ] Implement complex forms using **React Hook Form or `@tanstack/react-form` + Zod** (e.g., multi-step wizards, file/image uploads to Cloudinary).
- [ ] Add **Optimistic UI updates** for instant feedback actions (e.g., toggling a status, adding to cart, or upvoting).
- [ ] Implement global client state (Zustand/Context) for UI-specific states (e.g., sidebar toggle, multi-step form data persistence).
- [ ] **Mandatory:** Integrate the frontend flow for **Stripe or SSLCommerz** (Test Mode), including proper success/cancel redirect handling.
- [ ] Optimize performance: audit bundle size, ensure proper `next/image` usage, and resolve any React hydration warnings.

### 🔴 Day 5 — Polish, Deployment & Submission
- [ ] Conduct rigorous cross-device testing (desktop, tablet, mobile) and fix any responsive layout breaks.
- [ ] Deploy to Vercel (or Netlify) and verify all environment variables, CORS settings, and API connections work flawlessly in production.
- [ ] **Crucial Check:** Test the **One-Click Demo Login** and Payment flow in the live production environment.
- [ ] Review Git history to ensure **20+ meaningful, conventional commits** (rewrite/squash messy commits if necessary).
- [ ] Record the **5–10 minute video walkthrough**, strictly following the provided video guide checklist.
- [ ] Finalize and submit the exact required text template with all links in the assignment portal.

---
