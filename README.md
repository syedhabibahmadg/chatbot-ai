# AI Startup Dashboard

<div align="center">

  <img src="https://img.shields.io/badge/Next.js-14.2.4-000000?style=for-the-badge&logo=next.js" alt="Next.js" />
  <img src="https://img.shields.io/badge/TypeScript-5.5.2-3178C6?style=for-the-badge&logo=typescript" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Prisma-5.16.0-2D3748?style=for-the-badge&logo=prisma" alt="Prisma" />
  <img src="https://img.shields.io/badge/NextAuth-4.24.7-000000?style=for-the-badge&logo=nextauth" alt="NextAuth" />
  <img src="https://img.shields.io/badge/Google%20AI-GenAI-4285F4?style=for-the-badge&logo=google" alt="Google AI" />

  <h3>Smart AI dashboard for modern businesses, teams, and founders.</h3>
  <p>
    A polished startup-facing web app with authentication, AI chatbot workflows, protected dashboard access,
    and a clean interface designed to turn your product into a strong first impression.
  </p>

  <p>
    <a href="#features">Features</a> ·
    <a href="#tech-stack">Tech Stack</a> ·
    <a href="#setup">Quick Start</a> ·
    <a href="#project-structure">Project Structure</a>
  </p>

</div>

---

## Overview

This project is a modern AI-powered dashboard starter built with Next.js. It combines:

- Secure user authentication
- Protected dashboard routes
- AI assistant/chat interface
- Clean startup-style UI
- Ready-to-extend admin and product architecture

It is designed for founders, startups, SaaS teams, or AI products that want a premium-looking dashboard experience from day one.

---

## Why this project?

A startup product is not only about features — it is also about the first impression.

When someone lands on your dashboard, they should instantly feel:

- Professional
- Trustworthy
- Modern
- Product-ready
- Built for scale

This project gives you a strong foundation for that experience.

---

## Features

### 🚀 Dashboard Experience
- Clean, modern startup layout
- Responsive dashboard interface
- Protected pages for authenticated users
- Premium dark/blue visual theme

### 🤖 AI Chat Capabilities
- Integrated AI chatbot workflow
- Google Generative AI support
- Chat-style interaction ready for business use cases
- Extensible for customer support, internal agents, and productivity tools

### 🔐 Authentication System
- Email/password login
- Social login support
- Secure route protection using middleware
- User session management with NextAuth

### 📊 Startup-Ready Architecture
- Scalable Next.js app structure
- Prisma database integration
- Reusable UI patterns
- Easy expansion for analytics, reports, CRM, or admin panels

---

## Tech Stack

- Next.js 14
- React 18
- TypeScript
- Tailwind CSS
- Chakra UI
- Prisma ORM
- NextAuth
- Google Generative AI
- PostgreSQL / MongoDB compatible setup via Prisma

---

## Screenshots / Product Feel

This project is built to feel like a real startup dashboard experience.

The interface includes:

- premium hero/welcome sections
- dashboard orientation for logged-in users
- protected app flow
- AI-first product experience

> Add your real screenshots here:
>
> - `public/screenshots/dashboard-home.png`
> - `public/screenshots/ai-chat.png`
> - `public/screenshots/admin-panel.png`

---

## Project Structure

```bash
.
├── app/
│   ├── (auth)/
│   ├── (landing)/
│   ├── admin/
│   ├── dashboard/
│   └── profile/
├── components/
├── lib/
├── prisma/
├── public/
├── styles/
├── .env.example
├── middleware.ts
├── package.json
├── README.md
└── tsconfig.json
```

---

## Setup

### 1) Clone the repository

```bash
git clone https://github.com/syedhabibahmadg/chatbot-ai.git
cd chatbot-ai
```

### 2) Install dependencies

```bash
npm install
```

### 3) Configure environment variables

Create a `.env` file from the example file:

```bash
cp .env.example .env
```

Update it with your values such as:

```env
NEXTAUTH_SECRET=your_secret_key
NEXTAUTH_URL=http://localhost:3000
DATABASE_URL="your_database_url"
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GEMINI_API_KEY=your_gemini_api_key
```

### 4) Initialize Prisma

```bash
npx prisma generate
npx prisma db push
```

### 5) Run the app

```bash
npm run dev
```

Open:

```bash
http://localhost:3000
```

---

## Available Routes

- `/` – landing page
- `/auth` – login / sign up flow
- `/dashboard` – protected dashboard area
- `/admin` – admin access area
- `/profile` – user profile page

---

## Roadmap

- [ ] Add analytics dashboard widgets
- [ ] Add charts and KPIs
- [ ] Add team/user management
- [ ] Add AI workflow automation panel
- [ ] Add billing and subscriptions UI
- [ ] Add multi-role admin system
- [ ] Add dark/light mode toggle

---

## Contribution

Contributions are welcome.

If you want to improve the dashboard experience, add new sections, or extend AI features:

```bash
git checkout -b feature/my-improvement
```

Then make your changes and open a pull request.

---

## License

This project is currently configured for personal/development use.

If needed, you can update the license later for commercial startup use.

---

## Final Note

This app is a strong starting point for a modern AI startup dashboard. It is simple enough to understand, but polished enough to present as a real product experience.

If you want, the next step can be to turn this into:

- a SaaS admin panel
- a CRM dashboard
- an AI operations center
- a customer support portal
- a startup analytics dashboard

---

<p align="center">
  <b>Built for founders who want their product to look premium from the first click.</b>
</p>
