# OM API Request Constructor

This is a single-page static HTML tool for manually constructing WagerWatch -> Worker -> OddsMarket requests.

## Files

- `public/index.html` - the static web app.
- `wrangler.toml` - only needed if deploying as Cloudflare Worker static assets with `wrangler deploy`.
- `package.json` - optional local deploy scripts.

## Deploy to Cloudflare Pages via dashboard / Git

Use these build settings:

- Build command: leave blank, or use `echo "No build step"`
- Build output directory: `public`
- Do not use `npx wrangler deploy` as the Pages build command.

## Deploy to Cloudflare Pages via Wrangler

```bash
npx wrangler pages deploy public --project-name om-api-request-constructor
```

## Deploy as Worker static assets

```bash
npx wrangler deploy
```

This uses `wrangler.toml` and the `assets = { directory = "./public" }` setting.
