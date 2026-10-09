# Chatbot AI

A modern AI-powered web application built with Next.js, designed for secure authentication, protected dashboards, and intelligent chatbot interactions. The app supports user login via credentials, Google, and Facebook, and includes a Gemini-powered chat experience with OCR support for uploaded document images.

## Features

- NextAuth authentication with:
  - Email/password login
  - Google OAuth
  - Facebook OAuth
- Protected user dashboard and admin routes
- Prisma + MySQL data model for user records and accounts
- AI chat interface using Google Generative AI
- OCR-based image processing using Tesseract.js
- Tailwind CSS + Chakra UI for responsive UI design
- Role-based access with admin support
- Modern Next.js 14 application structure

## Tech Stack

- Next.js 14
- TypeScript
- Tailwind CSS
- Chakra UI
- Prisma ORM
- MySQL
- NextAuth
- Google Generative AI
- Tesseract.js
- React Markdown

## Project Structure

```bash
chatbot-ai/
├── app/
│   ├── (auth)/
│   │   ├── auth/
│   │   ├── reset-password/
│   │   └── layout.tsx
│   ├── (landing)/
│   │   └── page.tsx
│   ├── admin/
│   │   ├── hooks/
│   │   └── page.tsx
│   ├── api/
│   │   └── auth/
│   ├── chat/
│   │   ├── App.css
│   │   ├── layout.tsx
│   │   └── page.tsx
│   ├── dashboard/
│   │   ├── App.css
│   │   ├── layout.tsx
│   │   └── page.tsx
│   ├── components/
│   │   └── ChatWithGemini.tsx
│   ├── hooks/
│   ├── libs/
│   ├── utils/
│   │   ├── authOptions.ts
│   │   └── ...
│   ├── config.ts
│   ├── globals.css
│   ├── layout.tsx
│   └── favicon.ico
├── components/
├── context/
├── lib/
├── prisma/
│   └── schema.prisma
├── public/
├── .env.example
├── .eslintrc.json
├── .gitignore
├── .prettierrc.json
├── components.json
├── next.config.js
├── package.json
├── postcss.config.js
├── readme.gif
├── tailwind.config.ts
├── tsconfig.json
├── LICENSE
└── README.md
```

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/syedhabibahmadg/chatbot-ai.git
   cd chatbot-ai
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure your environment variables:
   ```bash
   cp .env.example .env
   ```

4. Update the `.env` file with your values:
   ```env
   APP_URL="http://localhost:3000"

   DATABASE_URL="mysql://root:root@127.0.0.1:3306/testauth"
   SECRET="your-secret-key"

   GOOGLE_ID="your-google-id"
   GOOGLE_SECRET="your-google-secret"
   FACEBOOK_CLIENT_ID="your-facebook-client-id"
   FACEBOOK_CLIENT_SECRET="your-facebook-client-secret"

   EMAIL_USERNAME="your-email-username"
   EMAIL_FROM="your-email-from"
   EMAIL_PASSWORD="your-email-password"
   ```

5. Set up the database schema:
   ```bash
   npx prisma generate
   npx prisma db push
   ```

6. Run the application:
   ```bash
   npm run dev
   ```

7. Open:
   ```bash
   http://localhost:3000
   ```

## Available Scripts

```bash
npm run dev
npm run build
npm run start
npm run lint
npm run prisma:ui
```

## Authentication and Authorization

The project uses NextAuth with a Prisma adapter and includes:

- Credentials-based authentication
- Google and Facebook provider login
- JWT session strategy
- Role-based user access
- Email verification for credential users
- Protected admin and dashboard flows

## AI and OCR Capabilities

This project includes a chatbot interface with Gemini integration and supports image uploads for OCR processing. Uploaded images can be converted to text with Tesseract.js before being sent to the AI model for analysis.

## Screenshots

![Project preview](./readme.gif)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
