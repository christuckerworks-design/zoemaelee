# Zoemaelee

A pseudonymous wishlist. Share your list, keep your identity.

Live: https://zoemaelee.netlify.app

## What this is

A single static page (`index.html`) that talks directly to Supabase for
accounts and list storage. There is no build step and no server of our own.

- **Auth + database:** Supabase (project `gioxjlsgsjgwiqaeopxu`)
- **Hosting:** Netlify (free credit-based plan)
- **Build command:** none
- **Publish directory:** `.` (repo root)

## Cost discipline

Netlify's free plan gives **300 credits/month** and a **hard limit** — when
they run out, the site is paused with no warning.

| Action | Credits |
| --- | --- |
| Production deploy (push to `main`) | **15** |
| Deploy Preview (pull request) | **free** |
| Branch deploy | free |
| Bandwidth | 20 per GB |

**Never push straight to `main`.** Every change goes through a branch and a
pull request, so Netlify builds a free Deploy Preview you can test. Only merge
when it's right. That turns unlimited testing into exactly one 15-credit
publish.

## How to make a change

1. Open `index.html` on GitHub, click the pencil (Edit).
2. Scroll down and choose **Create a new branch for this commit and start a
   pull request**.
3. Commit, then open the pull request.
4. Netlify comments on the PR with a Deploy Preview URL — open it and test.
5. Still editing? Push to the same branch; the preview updates for free.
6. Happy? **Merge pull request** → that's the one paid production deploy.

## Not built yet

- Real link fetching (needs a Netlify Function — now possible since this site
  is Git-connected)
- Public list view (`?u=<handle>`)
- Affiliate disclosures, custom SMTP, responsive layout
