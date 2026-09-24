## 📋 Project Requirements

### 🛠️ Recommended Tech Stack

| Category | Technology | Purpose |
|----------|------------|---------|
| **Framework** | Next.js (App Router), TypeScript | Server-side rendering, advanced routing, and strict type safety |
| **Styling & UI** | Tailwind CSS / StyleX, shadcn/ui, Framer Motion *(optional)* | Rapid, responsive, accessible, and animated UI development |
| **State Management** | TanStack Query + Zustand / Context *(if needed)* | Server-state caching, optimistic updates, and global client-state |
| **Forms & Validation** | React Hook Form + Zod | Type-safe, performant form handling with schema-based validation |
| **Payment Integration** | Stripe (Checkout/Elements) or SSLCommerz (Test Mode) | Secure, real payment gateway integration (No fake "Cash on Delivery") |
| **Authentication** | NextAuth.js (Auth.js) or Custom JWT (Cookies + Middleware) | Secure session management, HTTP-only cookies, and protected routes |
| **Media & Icons** | `next/image`, Lucide React | Optimized image delivery and consistent, accessible iconography |
| **Deployment** | Vercel, Netlify, or Cloudflare | Seamless frontend deployment with global edge network and preview URLs |

---

### 🎯 Core Project Rules

> [!IMPORTANT]
> These rules define the baseline quality of your application. Deviating from these will result in mark deductions.

- **Strict Role-Based UI (RBAC)**: The application must have distinct views or dashboards for **3 fixed primary roles** (e.g., Customer, Provider, Admin). A user must only see and interact with what their role permits.
- **Real API Integration**: You must connect to a real backend API. Mock data or hardcoded JSON is **NOT** accepted for core workflows.
- **URL State Synchronization**: Filtering, sorting, and pagination must be reflected in the URL (e.g., `?page=2&status=active`) using `useSearchParams`, allowing users to bookmark or share specific views.
- **No Placeholder Content**: All UI elements must be fully implemented and populated with real data. The use of "Lorem ipsum" text, placeholder images, or incomplete demo components is strictly prohibited.
- **Skeleton Loaders & Partial Rendering**: Implement skeleton loaders (`loading.tsx`) and partial rendering techniques to provide immediate visual feedback during data fetching, avoiding full-page spinners or blank screens.
- **Data Visualization**: Admin or Manager dashboards must include at least one data visualization component (e.g., charts/graphs using Recharts or Chart.js).
- **Advanced Filtering**: Implement faceted search UIs (e.g., e-commerce style sidebar filters) with URL synchronization.
- **Performance Optimization**: Use `next/image` for all images and avoid unnecessary client-side re-renders.
- **Robust Error Handling**: Graceful error handling using `error.tsx` boundaries and toast notifications (e.g., Sonner or React Hot Toast) for API failures.

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

### 🚀 Frontend-Specific Challenges (Optional but Recommended)

> 💡 **Go the extra mile:** Implementing these features will not only secure maximum marks but will also make your project stand out in professional job interviews.

- **Real-time Feel (Optimistic UI)**: Use TanStack Query to instantly update the UI for status changes (e.g., marking a task as "Done" or adding to cart) *before* the server responds, rolling back gracefully only if the API fails.
- **Multi-step Workflows**: Build wizard-style forms for complex creations (e.g., "Create Shipment" or "Register Patient") with step-by-step validation and progress indicators.
- **Dark Mode Support**: Implement a seamless light/dark mode toggle using `next-themes` and Tailwind CSS, ensuring all custom components and charts adapt gracefully.
- **SEO & Metadata**: Utilize the Next.js App Router Metadata API to generate dynamic Open Graph (OG) images, titles, and descriptions for public-facing pages.
- **Accessibility (a11y) First**: Ensure full keyboard navigation, proper ARIA labels, focus management in modals, and sufficient color contrast. Treat accessibility as a core requirement, not an afterthought.
