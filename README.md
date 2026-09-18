# Cape Town villas — 30 Dec 2026 to 25 Jan 2027

A single static page listing the villa options for the stay: villa, details,
per-night rate and stay total, grouped by date window.

- `index.html` — the whole page. No build step, no dependencies.
- `images/hero-cape-town.jpg` — the header background.

## Connecting Vercel (once)

1. Go to https://vercel.com/new and sign in with GitHub.
2. Import `deanwhitex/capetown`. If it isn't listed, use **Adjust GitHub App
   Permissions** and grant Vercel access to this repository.
3. Framework preset: **Other**. Leave Build Command, Output Directory and
   Install Command empty — the page is served straight from the repo root.
4. Click **Deploy**.

That's the only manual step. Vercel installs a webhook on the repository as
part of the import.

## What happens automatically afterwards

- **Production branch** is `claude/cape-town-villa-rentals-9zo3lw` — the
  repository's default branch, and the branch this page is developed on.
  Every push to it redeploys the live URL within about a minute. No action
  needed in Vercel, and none from you.
- **Any other branch** gets its own preview URL instead of touching the live
  site, so changes can be looked at before they go out.
- **Pull requests** get a preview URL posted as a comment on the PR.

Changing the hero image or a rate is therefore just a commit and a push — the
live page follows on its own.

## Changing the production branch

If the branch is ever renamed (to `main`, say), update it in Vercel under
**Project → Settings → Git → Production Branch**, or the live URL will keep
following the old branch.
