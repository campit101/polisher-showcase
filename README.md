# Polisher

**[aipolisher.app](https://aipolisher.app)** is a live subscription web app that rewrites a draft in the user's own voice.

I designed and built it end to end. The source code is private, so this repository is an overview of what it does and how it is built.

## What it does

- Rewrites a draft so it sounds like the person who wrote it, using their own writing samples
- UK or US spelling settings
- Accounts and sign-in
- Usage limits and monthly subscription billing through Stripe
- Landing page and waitlist
- Admin dashboard for tracking launch results against set thresholds

## Stack

| Area | Tools |
| --- | --- |
| Front end and server | TypeScript, Next.js, React |
| Database and auth | Supabase (PostgreSQL) with row level security |
| Payments | Stripe subscriptions and webhooks |
| Hosting | Vercel |
| Testing | Vitest, Playwright end-to-end tests, axe accessibility checks |
| Delivery | GitHub Actions CI, secret scanning |

## Engineering practices

- Row level security on database tables, with integration tests for the access rules
- End-to-end browser tests and automated accessibility checks on every page, in light and dark themes
- Rate limiting and usage allowances to control cost
- Automated checks that run before each change is merged

## Contact

Cameron Pittaway, Aberdeen, Scotland. [LinkedIn](https://www.linkedin.com/in/campittaway/) | [Polisher](https://aipolisher.app)
