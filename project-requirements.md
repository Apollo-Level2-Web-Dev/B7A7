## 📋 Project Requirements

### 🛠️ Tech Stack

| Category | Technology | Purpose |
|----------|------------|---------|
| **Framework** | Next.js (App Router), TypeScript | Server-side rendering, routing, and type safety |
| **Styling & UI** | Tailwind CSS / StyleX, shadcn/ui, Framer Motion (optional) | Rapid, responsive, and accessible UI development |
| **State Management** | TanStack Query (React Query) + Zustand / Context (if needed) | Server-state caching and global client-state management |
| **Forms & Validation** | React Hook Form + Zod | Type-safe form handling and client-side validation |
| **Payment Integration** | Stripe (Checkout/Elements) or SSLCommerz (Test Mode) | Secure, real payment gateway integration (No fake "Cash on Delivery" workflows) |
| **Authentication** | NextAuth.js (Auth.js) or Custom JWT (Cookies + Middleware) | Secure session management, HTTP-only cookies, and protected route enforcement |
| **Media** | Next/Image | Optimized icons and image delivery |
| **Deployment** | Vercel, Netlify, or Cloudflare | Seamless frontend deployment with global edge network and preview URLs |

### 🎯 Core Project Rules

- **Role-Based UI**: The application must have distinct views or dashboards for **3 fixed primary roles** (e.g., Customer, Provider, Admin). A user must only see what their role permits.
- **API Integration**: You must connect to a real backend API. Mock data is **NOT** accepted for core workflows.
- **URL State Management**: Filtering, sorting, and pagination must be reflected in the URL (e.g., `?page=2&status=active`) using `useSearchParams`, allowing users to share links.
- **Visualize Dashboards**: Data visualization (charts/graphs) for Admin roles.
- **Advanced Filtering**: Faceted search UI with URL synchronization (e.g., e-commerce style filters).
- **Performance**: Use `next/image` for all images, implement skeleton loaders (`loading.tsx`), and avoid unnecessary client-side re-renders.
- **Error Handling**: Graceful error handling using `error.tsx` and toast notifications (e.g., Sonner or React Hot Toast) for API failures.

---

**Frontend-Specific Challenges to Consider (Optional):**
- **Real-time Feel**: Optimistic UI updates for status changes (e.g., marking a task as "Done" instantly before the server responds), you can use tools like tanstack query.
- **Multi-step Workflows**: Wizard-style forms for complex creations (e.g., "Create Shipment" with multiple steps).
- **Dark Mode Support**: Implement a seamless light/dark mode toggle using next-themes and Tailwind CSS, ensuring all custom components and charts adapt gracefully.
- **SEO & Metadata**: Utilize Next.js App Router Metadata API to generate dynamic Open Graph (OG) images, titles, and descriptions for public-facing pages (e.g., individual product or service detail pages).
- **Accessibility (a11y) First**: Ensure full keyboard navigation, proper ARIA labels, focus management in modals, and sufficient color contrast. Treat accessibility as a requirement, not an afterthought.

---
