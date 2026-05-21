# Test OM API Request Constructor

Static Cloudflare Pages site for manually constructing WagerWatch -> Worker -> OddsMarket API test requests.

## Cloudflare Pages settings

Use these settings when connecting this GitHub repo to Cloudflare Pages:

- Framework preset: None
- Build command: leave blank
- Build output directory: public
- Root directory: /

## Files

```text
public/
  index.html
README.md
```

## Important

This is only the website UI. It does not contain the OddsMarket API key.

The OddsMarket API key must be stored only in the Cloudflare Worker as the secret:

```text
ODDSMARKET_API_KEY
```

After deploying your Worker, enter its test endpoint in the UI:

```text
https://YOUR_WORKER.YOUR_SUBDOMAIN.workers.dev/om/test-lookup
```
