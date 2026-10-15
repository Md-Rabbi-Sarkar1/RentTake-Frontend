# Rental Property Management System (RPMS) - Frontend

This is the client-side user interface for the Rental Property Management System, built using **Next.js**, **Tailwind CSS**, and **TypeScript**. It delivers highly responsive, role-based dashboards tailored for Property Administrators, Landlords/Owners, and Tenants.

## 🛠️ Tech Stack & Architecture

* **Framework:** Next.js (App Router)
* **Styling:** Tailwind CSS / Shadcn UI
* **State Management:** TanStack Query (React Query) / Zustand
* **Authentication:** NextAuth.js (Session management)
* **Rendering Strategies:** 
  * **SSR (Server-Side Rendering):** Powers the secure dynamic dashboards for landlords and tenants to prevent layout shifts and flash-of-unauthenticated content.
  * **ISR (Incremental Static Regeneration):** Optimizes the public property search directory and individual property listing pages, regenerating them in the background when updates occur.
  * **CSR (Client-Side Rendering):** Manages interactive elements like property filters, dynamic map widgets, and payment forms.

## 🚀 Key Client Portals

* **Tenant Dashboard:** Browse available properties, submit rental applications, securely track upcoming rent dues, and file maintenance tickets.
* **Landlord Portal:** Upload property listings (images, pricing, rules), review tenant background applications, verify invoice balances, and update repair statuses.
* **Admin Control Center:** Global overview to verify newly uploaded properties, monitor user roles, and access automated system logs.

## ⚙️ Getting Started

### Prerequisites
* Node.js (v18.x or higher)
* npm, yarn, or pnpm

### Installation & Local Run

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install client dependencies:
   ```bash
   npm install
   ```

3. Setup environment configuration:
   Create a `.env.local` file in the root of this folder:
   ```env
   NEXT_PUBLIC_API_URL=http://localhost:5000/api/v1
   NEXTAUTH_SECRET=your_nextauth_secret_key_here
   ```

4. Run the development server:
   ```bash
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) to view the client-side app.
