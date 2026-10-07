# paulgeo

Link page for Paul Georgoudis, served as static files by the Cloudflare Worker `paul`
(https://paul.cooper-577.workers.dev/). No build step: the files in this folder are the site.

- `index.html` is the whole page (styles are inline).
- `images/` holds the profile photo and the FundedNext logo.
- `_headers` sets the response headers; `.assetsignore` keeps repo files off the site.

Every push to `main` goes live once the Worker's Builds are connected to this repo
(deploy command `npx wrangler deploy`).
