# Next.js Invoice Dashboard

A learning implementation based on the [Next.js App Router course](https://nextjs.org/learn). It explores server-rendered financial views, invoice management, and credential-based authentication.

## What the code covers

- PostgreSQL-backed dashboard summaries, customers, and invoices.
- Invoice creation, editing, and deletion through server actions.
- Zod form validation, search, pagination, loading states, and error boundaries.
- NextAuth credential sign-in with bcrypt password verification.

Start with [server actions](app/lib/actions.ts), [data queries](app/lib/data.ts), and [authentication](auth.ts).

## Development prerequisites

Install dependencies with `npm ci`. Configure private `POSTGRES_URL` and `AUTH_SECRET` environment values for a development database and authentication. Database connections require SSL in the checked-in queries. Review [the seed route](app/seed/route.ts) before invoking it: seeding writes sample data and is appropriate only for a disposable development database.

Run `npm run dev` after preparing the database. This repository follows a course foundation; it is presented as learning work rather than an original commercial product.

## Current limits

The seed and query endpoints need review before public exposure. Runtime dependencies include unpinned `latest` versions, the lint script needs compatibility review, and no automated test suite is included. The documentation review did not run the application.
