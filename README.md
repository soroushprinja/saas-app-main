SaaS LMS with Voice AI (Next.js + Supabase + Clerk)

A fully functional SaaS-style Learning Management System featuring voice-enabled tutoring, subscription-based access, and real-time interactions — built with a scalable and modern full-stack architecture.

🚀 Features

✅ User Authentication & Authorization (Clerk)

💳 Subscription Billing & Access Control

🎙 Voice AI Tutor Integration (Real-time conversational agents)

🔍 Search & Filters for Tutors / Subjects

📌 Bookmarking & Activity History

⚡ Modern UI with Tailwind + shadcn/ui

📱 Fully Responsive Across Devices

🛠 Modular Architecture for Easy Expansion

🧠 Tech Stack
Layer	Technology
Frontend Framework	Next.js (App Router)
Auth & Billing	Clerk
Database & APIs	Supabase
Voice AI	Vapi
UI Components	shadcn/ui + Tailwind CSS
Validation	Zod
Monitoring	Sentry
📦 Installation
git clone https://github.com/soroushprinja/saas-app-main.git
cd saas-app-main
npm install

🔐 Environment Variables

Create a .env file in the root with:

# Sentry
SENTRY_AUTH_TOKEN=

# Vapi
NEXT_PUBLIC_VAPI_WEB_TOKEN=

# Clerk
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_IN_FALLBACK_REDIRECT_URL=/
NEXT_PUBLIC_CLERK_SIGN_UP_FALLBACK_REDIRECT_URL=/

# Supabase
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=

▶️ Run Locally
npm run dev


Then open:

http://localhost:3000

📁 Project Structure
/
├── app/                    # Next.js routes and logic
├── components/             # Reusable UI blocks
├── constants/              # Static configs & enums
├── lib/                    # Utilities, hooks, API wrappers
├── public/                 # Static assets
├── middleware.js
├── next.config.mjs
└── ...

🛠 Customization Ideas
Want to Add	How to Do It
New Subscription Tiers	Define plans in Clerk
Additional AI Tutor Types	Extend voice agent config
Progress Tracking	Add user-specific history tables
Leaderboards / Gamification	Supabase realtime tables
📤 Deployment

Compatible with Vercel, Netlify, or any platform supporting Next.js + Edge functions.
Just ensure all environment variables are set in production.
