# whosthatcorvid.co.uk

A simple web page to help you identify corvids!

Initially vibe coded in Google AI studio as part of a work AI training thing.

## Deploy to Cloudflare Workers

Cloudflare Workers Builds deploys the site automatically when changes are pushed to `main` on GitHub. The site uses Vite and Cloudflare Workers Static Assets; the custom domains are configured in `wrangler.jsonc`.

Connect the existing `whosthatcorvid` Worker to this GitHub repository from **Workers & Pages → whosthatcorvid → Settings → Builds → Connect**. Set the production branch to `main`, the build command to `npm run build`, and the deploy command to `npx wrangler deploy`. Leave the root directory at the repository root. Workers Builds does not use Wrangler's `build.command` setting.

After connecting, push commits to `main`; Cloudflare will build and deploy them. Local development still uses `npm run dev`.

## To Do

- Fix the AI slop SVG corvid for a nicer outline.
- Can probably just be a static site, not on cloudflare workers.
- Pull some images off wikipedia or elsewhere so it's not just all text.
- Make the styling look less shit.
- Lil burger menu with an about and mention charlie the crow and his my Grannie's TikTok (@jaxmadhouse)
- Actually fact check all the stuff I just let Gemini write it all.
- Lil footer
- Do a pass for code quality and stuff, it took quite a few prompts in AI Studio to get to the minimal web page so there's probably lots of useless crap there.
