# Khojo Marketplace

A Vite + React + TypeScript storefront and admin experience for a neighbourhood social-commerce marketplace.

## Overview

Khojo is designed to support:
- buyer browsing and product discovery
- seller applications and approval workflows
- admin review queues and member insights
- member feedback and public review experiences
- Supabase-powered authentication, storage, and database logic

This project is intended for local development and deployment configuration, not for exposing private credentials or internal operational secrets in the repository.

## Tech Stack

- React 19
- TypeScript
- Vite
- Tailwind CSS
- Supabase
- Framer Motion
- Lucide React

## Getting Started

1. Clone the repository
   ```bash
   git clone https://github.com/tajtarun/khojo.git
   cd khojo
   ```
2. Install dependencies
   ```bash
   npm install
   ```
3. Create a local environment file from the example
   ```bash
   cp .env.example .env.local
   ```
4. Fill in the required Supabase values in `.env.local`
5. Start the app
   ```bash
   npm run dev
   ```
6. Build for production
   ```bash
   npm run build
   ```

## Environment Variables

Use the sample file `.env.example` as the template. Do not commit real secrets, service-role keys, SMTP credentials, payment credentials, or courier tokens.

Example variables:
```dotenv
VITE_SUPABASE_URL=
VITE_SUPABASE_PUBLISHABLE_KEY=
VITE_WEB3FORMS_ACCESS_KEY=
VITE_PUBLIC_APP_URL=
```

## Project Notes

- Keep secrets in server-only configuration such as Supabase Edge Function secrets or deployment environment variables.
- Never commit `.env.local` or any private credential file.
- Treat any third-party reference code or local setup notes as untrusted until reviewed.
- Use `npm run build` before shipping changes to verify the app still compiles.

## Security

Please review `SECURITY.md` before reporting vulnerabilities or sensitive issues.

## License

This project is licensed under the MIT License. See `LICENSE` for details.
