# Améza frontend

React storefront built with Vite. The API is maintained separately in
[AMEZA-Backend](https://github.com/shoaibkhan2015/AMEZA-Backend).

## Local development

Use Node.js 22.12 or newer.

```sh
npm ci
cp .env.example .env
npm run dev
```

In development, Vite forwards `/api` requests to `http://localhost:4000`.
Start the backend separately, or set `VITE_API_URL` to a running API origin.

## Environment

Set `VITE_API_URL` to the backend's public origin, without a trailing slash.
The app appends `/api` automatically. Set `VITE_SUPABASE_URL` and
`VITE_SUPABASE_ANON_KEY` for Supabase-backed admin sign-in, and optionally
`VITE_WHATSAPP_NUMBER`.

## Deployment

Deploy this repository as a Vite app (for example, on Vercel). The build
command is `npm run build`, with output in `dist`. Configure the environment
variables above in the hosting provider; `VITE_` values are embedded at build
time, so rebuild after changing them.
