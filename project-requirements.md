## 📋 Project Requirements

> 💡 **Note:** Read these carefully. While not every single point is strictly fixed, you must follow this general guideline to ensure your project meets expectations.

## 🛠️ Tech Stack

| Category | Technology | Purpose |
|----------|------------|---------|
| **Framework** | Next.js (App Router), TypeScript | Server-side rendering, routing, and type safety |
| **Styling & UI** | Tailwind CSS, shadcn/ui | Responsive, accessible, and modern UI development |
| **State Management** | TanStack Query + Zustand / Context *(if needed)*  | Server-state caching and global client-state management |
| **Forms & Validation** | React Hook Form / `@tanstack/react-form` + Zod | Type-safe form handling and client-side validation |
| **Authentication** | NextAuth.js / Custom JWT + Middleware | Secure session management and protected routes |
| **Payment Integration** | Stripe / SSLCommerz (Test Mode) | Real payment processing with success/cancel flows |
| **Data Visualization** | Recharts / Chart.js | Admin dashboard charts and analytics |
| **Media & Icons** | `next/image`, Lucide React | Optimized image delivery and consistent iconography |
| **Notifications** | Sonner / React Hot Toast | User-friendly toast notifications |
| **Deployment** | Vercel / Netlify / Cloudflare | Production frontend deployment with edge network |

> **Note:** You do not need to use every technology in every project. Choose technologies based on the actual requirements of your specific project.

--- 

## 🎯 Core Project Rules

- **Roles**: Each project must have **3 fixed primary roles** (e.g., Customer, Provider, Admin). Role permissions must be strictly enforced at both route level (Middleware) and UI level (conditional rendering).
- **Payment Integration**: This is **MANDATORY**. You must integrate **Stripe or SSLCommerz** (Test Mode). Your frontend must handle payment initiation, success redirect, and cancellation redirect. *Cash on Delivery, Pay Later, or fake manual status updates are NOT accepted.*
- **Real API Only**: You must connect to a real backend API (your B7A6 project or a provided one). Mock data, hardcoded JSON, or placeholder content is **NOT accepted** for any core workflow.
- **One-Click Demo Login**: Your login page must feature distinct, one-click "Demo Login" buttons for each of the 3 roles (e.g., Admin, User, Provider) to allow evaluators to quickly test role-based UI.
- **URL State Synchronization**: All filtering, sorting, searching, and pagination must be reflected in the URL (e.g., `?page=2&status=active`) using `useSearchParams`, allowing users to bookmark or share specific views.
- **No Placeholder Content**: All UI elements must be fully implemented and populated with real data. The use of "Lorem ipsum" text, placeholder images, or incomplete demo components is strictly prohibited.
- **Performance & Loading States**: Use `next/image` for all images, implement skeleton loaders (`loading.tsx`) for every data-fetching page, and avoid unnecessary client-side re-renders. Use Server Components by default.
- **Error Handling**: Implement graceful error handling using `error.tsx` boundaries and toast notifications (e.g., Sonner or React Hot Toast) for API failures. Never show a blank screen or unhandled crash to the user.

---

### 🔐 Mandatory UI Requirement: One-Click Demo Login

The login page must feature a clear, structured layout with separate, easily accessible **Demo Login** buttons for each of the 3 roles. This allows evaluators to quickly test role-based UI without manually typing credentials.

```text
┌─────────────────────────────────────────────┐
│                                             │
│              Welcome Back 👋                │
│                                             │
│        Login to your account                │
│                                             │
│  ┌───────────────────────────────────────┐  │
│  │ Email                                 │  │
│  │ [_______________________________]     │  │
│  │                                       │  │
│  │ Password                              │  │
│  │ [_______________________________]     │  │
│  │                                       │  │
│  │          [ 🔐 Login ]                 │  │
│  └───────────────────────────────────────┘  │
│                                             │
│              ─── OR ───                     │
│                                             │
│           🚀 Quick Demo Login               │
│                                             │
│  ┌──────────────┐ ┌──────────────┐          │
│  │ 👨‍💼 Admin     │ │ 👤 User      │          │
│  │              │ │              │          │
│  │ [Demo Login] │ │ [Demo Login] │          │
│  └──────────────┘ └──────────────┘          │
│                                             │
│          ┌──────────────────┐               │
│          │ 🛠️ Provider      │               │
│          │                  │               │
│          │  [Demo Login]    │               │
│          └──────────────────┘               │
│                                             │
└─────────────────────────────────────────────┘
```
*Note: Each **Demo Login** button should automatically authenticate the user with the corresponding demo account and redirect them to the appropriate role-specific dashboard.*

---

## 📄 Minimum 15 Pages Requirement

Each project must implement and deploy **at least 18 fully functional pages**. 

These pages must represent the actual functionality of your selected project. You should not create empty, duplicate, or dummy pages just to fulfill the page count.

### Page Technical Requirements

- **Responsive Design**: Mobile-first approach. Every page must work flawlessly on mobile, tablet, and desktop. Test using DevTools Device Toolbar.
- **Loading States**: Every data-fetching page must have a **skeleton loader** (`loading.tsx`). Full-page spinners or blank screens are not acceptable.
- **Empty States**: Every list/table view must show a meaningful empty state (e.g., "No orders found" with an illustration or icon) when there is no data.
- **Error States**: API failures must show toast notifications (Sonner / React Hot Toast). Page-level crashes must be caught by `error.tsx` boundaries.
- **Consistent Theming**: Use a unified color palette, typography scale, and spacing system across all pages. All components must look like they belong to the same application.
- **Accessibility (a11y) (Optional)**: Keyboard navigation, proper ARIA labels, focus management in modals/dropdowns, and sufficient color contrast (WCAG AA minimum).
- **Form Standards**: All forms must use **React Hook Form** or **`@tanstack/react-form`** with **Zod** or any other schema validation. Show real-time validation with human-readable error messages.
- **Complex Workflows**: At least one multi-step (wizard-style) form is expected for complex creations (e.g., "Create Shipment", "Post a Service").
- **File Uploads**: If your domain requires image/file uploads, integrate with Cloudinary or a similar service. Show upload progress and preview.
- **Component Splitting**: Use Server Components by default. Only add `"use client"` when you need interactivity (state, effects, event handlers).
- **TypeScript Strictness**: No `any` types. Define proper interfaces/types for all API responses, props, and form data.
- **Reusable Components**: Create shared, reusable UI components (e.g., `DataTable`, `StatCard`, `StatusBadge`, `SearchInput`). Do not copy-paste the same UI code across pages.
- **Custom Hooks**: Extract repeated logic into custom hooks (e.g., `useDebounce`, `useAuth`, `usePagination`).
- **SEO & Metadata**: All public pages must have proper **Metadata** (title, description, Open Graph tags) using the Next.js App Router Metadata API.

### Minimum Page Coverage

Your 15+ pages should cover most of the following areas:

| Category | Pages | Requirement |
|----------|:-----:|---|
| **Public Pages** | 5 | Home, About, Services, Contact, Domain-Specific (Pricing/FAQ/Blog) |
| **Authentication** | 2 | Login (with One-Click Demo), Register |
| **Admin Dashboard** | 3 | Overview/Analytics (with charts), Resource Management (CRUD + filters), Reports/Settings |
| **User Dashboard** | 3 | My Activity, Profile & Settings, Payments/History |
| **Provider Dashboard** | 3 | My Tasks/Listings, Earnings/Analytics, Profile & Availability |
| **Shared/Utility** | 2 | Custom 404 (`not-found.tsx`), Global Error Boundary (`error.tsx`) |
| **Payment** | 2 | Success redirect, Cancel redirect |
| **Total** | **18+** | |

### Example Route Structure

A complete project will contain routes structured similar to this:

```
# Public Pages (Server Components by default)
/                    → Home / Landing
/about               → About
/services            → Services / Features
/contact             → Contact
/pricing             → Domain-Specific Page (e.g., Pricing, FAQ, Blog)

# Authentication
/login               → Login (with One-Click Demo Login buttons)
/register            → Register

# Admin Dashboard (Protected — Admin Only)
/admin               → Overview / Analytics (Charts & Stats)
/admin/manage        → Resource Management (CRUD Table + Pagination/Filters)
/admin/reports       → Reports / Audit Logs / Settings

# User / Customer Dashboard (Protected — User Only)
/dashboard           → My Activity / Orders / Bookings
/dashboard/profile   → Profile & Settings (Form with Validation)
/dashboard/payments  → Payment History / Notifications

# Provider / Worker Dashboard (Protected — Provider Only)
/provider            → My Tasks / Listings (Status Updates)
/provider/earnings   → Earnings / Analytics
/provider/profile    → Profile & Availability Settings

# Shared / Utility
/not-found           → Custom 404 Page
/error               → Global Error Boundary

# Payment Integration
/payment/success     → Payment Success Redirect
/payment/cancel      → Payment Cancel Redirect
```
