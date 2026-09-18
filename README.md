# Cape Town villas — 30 Dec 2026 to 25 Jan 2027

A single static page listing the villa options for the stay: name, rate, stay
total and details for each property, grouped by date window.

- `index.html` — the whole page (no build step, no dependencies)
- `images/` — one photo per property; see `images/README.md` for the file names

## Deploying to Vercel

The site is plain static HTML, so it needs no build configuration.

1. Go to https://vercel.com/new and import `deanwhitex/capetown`.
2. Framework preset: **Other**. Leave the build command and output directory empty.
3. Deploy.

Vercel then redeploys automatically on every push to the branch you connect.
