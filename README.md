# whosthatcorvid.co.uk

A simple web page to help you identify corvids!

Initially vibe coded in Google AI studio as part of a work training.

## Deploy to Cloudflare Workers

Cloudflare Workers Builds deploys the site automatically when changes are pushed to `main` on GitHub. The site uses Vite and Cloudflare Workers Static Assets; the custom domains are configured in `wrangler.jsonc`.

Connect the existing `whosthatcorvid` Worker to this GitHub repository from **Workers & Pages → whosthatcorvid → Settings → Builds → Connect**. Set the production branch to `main`, the build command to `npm run build`, and the deploy command to `npx wrangler deploy`. Leave the root directory at the repository root. Workers Builds does not use Wrangler's `build.command` setting.

After connecting, push commits to `main`; Cloudflare will build and deploy them. Local development still uses `npm run dev`.
