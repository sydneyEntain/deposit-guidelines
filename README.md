# Deposit Guidelines — review site

Single-page preview of the **Deposit** experience guidelines doc, hosted as a Render Static Site.

- `index.html` — the page (self-contained; no build step, no dependencies).
- `render.yaml` — Render blueprint (static site, publishes this folder).

## Deploy to Render

### Option A — Blueprint (recommended)
1. Push this folder to a Git repo (GitHub or GitLab).
2. In Render: **New → Blueprint**, pick the repo. Render reads `render.yaml` and creates the static site.
3. Every push to the default branch redeploys automatically.

### Option B — Manual static site
1. Push this folder to a Git repo.
2. In Render: **New → Static Site**, pick the repo.
3. Settings:
   - **Build Command:** *(leave empty)*
   - **Publish Directory:** `.`
4. Create. You get a `https://<name>.onrender.com` URL.

## Note on visibility
This documents an internal, in-build feature. The `X-Robots-Tag: noindex, nofollow` header keeps it out of search engines, but a Render static-site URL is still reachable by anyone who has the link. For access control, front it with Render's password protection / access rules or host behind internal SSO.
