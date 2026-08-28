# Context: bboscoe.github.io / bernieboscoe.com

This repo is Bernie Boscoe's personal site, served via GitHub Pages at
**bernieboscoe.com** (custom domain set via the `CNAME` file — currently
`www.bernieboscoe.com`).

## Related repo: boscoe-research-group

A **separate** repo, `bboscoe/boscoe-research-group` (also at
`~/boscoe-research-group` locally), holds a standalone research-group
one-pager (AquiLLM, Green Crossing AI, people, publications, funding, talks,
contact). It has its own `CNAME` file set to `boscoe.sou.edu`.

**Why two repos, not one page in this site:** GitHub Pages only supports one
custom domain per repo — the whole repo's Pages output answers to that
domain (GitHub even 301-redirects the default `github.io` URL to the custom
domain once set). Since this repo is already claimed by bernieboscoe.com,
the research-group page had to live in its own repo to get its own domain.

This site's nav bar has a "Research Group" link pointing out to
`https://boscoe.sou.edu` (added under Header nav, see `index.html`) so the
two feel like one integrated site even though they're separate repos/domains.

## Status as of 2026-08-28

- Nav link to the research group site: **added and pushed**.
- Title fixed here: was showing "Assistant Professor," corrected to
  **"Associate Professor"** (subtitle + About section) — Bernie was promoted.
- `boscoe-research-group` repo: created, pushed, GitHub Pages enabled,
  `CNAME` set to `boscoe.sou.edu`.
- **DNS confirmed propagated** (checked via `dig`, both 8.8.8.8 and 1.1.1.1):
  `boscoe.sou.edu` → CNAME → `bboscoe.github.io.` → GitHub Pages IPs.
  `http://boscoe.sou.edu` serves the site (200 OK).
- **Pending:** HTTPS. `https://boscoe.sou.edu` doesn't respond yet — cert not
  issued/provisioned yet. In that repo's GitHub Pages settings, the
  "Enforce HTTPS" checkbox is **disabled/grayed out** because GitHub is
  still verifying the DNS/checking domain status — this can lag behind DNS
  actually resolving. Re-check the Pages settings page in a bit; once
  GitHub finishes its check, the cert should issue and "Enforce HTTPS"
  should become available to enable.
- A prior attempt to host the research-group page as a Google Sites page
  (`sites.google.com/sou.edu/bboscoe/home`) was built, then **deleted** —
  superseded by the GitHub Pages approach above, which gives a real
  `sou.edu` subdomain rather than a `sites.google.com` URL.

## Housekeeping notes (not yet resolved)

- `images/site_I5_2023.jpg` — now tracked in the repo (a Southern Oregon
  I-5 corridor landscape photo, taken Oct 2023). Not used anywhere yet;
  keeping it in the repo for later, no placement decided.
- `Boscoe2026CV.pdf` and `Evidence of Instructor Qualifications for
  NVIDIA.pdf` are sitting in the repo root (added outside this session).
  Worth double-checking those are meant to be in a **public** repo before
  they go out with a future push, if they haven't already.
