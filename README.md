# Phase Wheel

A self-contained, single-file interactive timer dial. No build step, no external
dependencies — everything (HTML, CSS, JS) lives in `public/index.html`.

## Deploy to Cloudflare Pages (free tier)

### Option A — from the command line (Wrangler)

```sh
npm install                 # installs wrangler locally
npx wrangler login          # one-time browser auth to your Cloudflare account
npm run deploy              # uploads ./public to a Pages project named "phase-wheel"
```

The first deploy creates the project and prints a `*.pages.dev` URL. Re-running
`npm run deploy` publishes a new version to the same URL.

### Option B — from the Cloudflare dashboard (no CLI)

1. Go to **Cloudflare Dashboard → Workers & Pages → Create → Pages**.
2. Either connect a Git repo or choose **Upload assets** and drop the `public/`
   folder.
3. Build command: *(leave empty)*. Build output directory: `public`.
4. Deploy — you'll get a `https://phase-wheel.pages.dev` URL.

## Local preview

```sh
npm run dev                 # serves public/ locally via wrangler
```

Or just open `public/index.html` directly in a browser — it works standalone.
