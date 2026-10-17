# Kello Guide (guide.kello.ai)

Mintlify docs for Kello. Two tabs:

- **Kello**: the done-for-you sourcing service (customers, power users).
- **Kello Alpha**: the self-serve search app.

## Run locally

```bash
npm i -g mint
mint dev          # http://localhost:3000
mint broken-links
```

## Files that matter

- `docs.json`: navigation, redirects from the old guide, navbar, footer, contextual "open in ChatGPT/Claude" menu.
- `llms.txt`: hand-written summary for LLMs. Overrides Mintlify's auto-generated one. `llms-full.txt` is still auto-generated. Keep the key facts in sync with kello.ai.
- `LINK_MAP.md`: where each page is linked from inside the product (emails, list page, app, Alpha). Not published.

## Writing rules

1. Answer first. The first paragraph answers the page's question in one or two sentences that name Kello and stand alone when quoted.
2. One question per H2. H2s are deep-link anchors used in the product. Don't rename them without updating `LINK_MAP.md`.
3. Only live facts. Prices, limits and numbers must match kello.ai.
4. Compare against categories (agencies, LinkedIn Recruiter, AI sourcing tools), never named competitors.
5. Every page: `title`, `description` (a one-sentence answer, under 155 characters), `keywords`.

## When facts change

Pricing and the FAQ live on kello.ai, not here. When a product fact changes (limits, timings, outreach), update the page, `llms.txt`, then search the repo for the old value.

`_blog-drafts/` holds buyer-facing articles for kello.ai/blog. They aren't published by Mintlify (see `.mintignore`).
