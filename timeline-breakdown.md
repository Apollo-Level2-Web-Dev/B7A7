
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
