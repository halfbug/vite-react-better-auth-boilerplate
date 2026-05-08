# Vite + React + TanStack + Better Auth Boilerplate

This project includes:

- React + TypeScript + Vite
- Tailwind CSS
- TanStack Router
- TanStack Table
- Better Auth with MongoDB adapter
- 3 pages:
  - `sign in`
  - `sign up`
  - protected `dashboard` with `header` and `footer`

## Setup

1. Copy env file:

```bash
cp .env.example .env
```

2. Fill in Google OAuth credentials in `.env`.
3. Make sure MongoDB is running locally (or update `MONGODB_URI`).
4. Install deps and run:

```bash
npm install
npm run dev
```

## Auth Routes

Better Auth runs on the Express server at:

- `http://localhost:3000/api/auth/*`

Vite proxies `/api` requests to that server.

## Pages

- `/sign-in` - email/password + Google
- `/sign-up` - email/password + Google
- `/dashboard` - protected page containing a sample TanStack table
