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
