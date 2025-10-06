# Drop/Hook — Next.js (TypeScript) for Vercel

## Deploy on Vercel
1) Push these files to a repo so that **app/** and **package.json** are in the **repo root**.
2) Vercel → New Project → Import Repo
   - Framework: Next.js
   - Root Directory: `/` (or the folder where app/ lives)
   - Node: 18.x
3) Environment Variables (Production):
   - `NEXT_PUBLIC_BLOB_READ_WRITE_TOKEN` — Create in Vercel: Storage → Blob → Tokens → Create (Read-Write)
   - `SMTP_HOST` = `smtp.gmail.com`
   - `SMTP_PORT` = `587` (or `465`)
   - `SMTP_USER` = your email
   - `SMTP_PASS` = app password (16 chars, no spaces)
   - `EMAIL_TO`  = recipient
   - `USE_SSL`   = `false` for 587, `true` for 465
4) Deploy.

