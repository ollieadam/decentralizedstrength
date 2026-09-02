# Decentralized Strength LLC Landing — Agent Context

## Project Overview

The company links landing page for Decentralized Strength LLC — the doorway to all sites/services. Hosted by Adam Oliver, CSCS.

**URL:** https://decentralizedstrength.com
**Repo:** `ollieadam/decentralizedstrength` (GitHub Pages, `main/root`)
**Deploy:** push to `main` → auto-deploys via GitHub Pages.

## Purpose
A **links portal** (not the podcast site). Links: Decentralized Strength Pod, Strength Club AI, Charleston Strength Club, social (`@decentralizedstrengthpod`), and email `decentralizedstrength@gmail.com`. Brand identity includes "self-directed positional trader/investor — blockchain & crypto."

## Structure
- `index.html` — links landing (hero + link cards, SEO meta, JSON-LD Organization). No branded hero images beyond the lockup.
- `blog/` — meta-refresh redirect stubs → `decentralizedstrengthpod.com/blog/<same>` (auto-redirect).
- `logo.png` / `logo-mark.png` / `logo-cover.png` — new Decentralized Strength brand (**evolved hexagon**, monochrome, landing-only).
- `favicon.png` / `apple-touch-icon.png` — hexagon mark icons.
- `CNAME`, `sitemap.xml`, `README.md`, GSC token.

## Brand rules
- Domain strings: **`decentralizedstrength.com`** (this site) and **`decentralizedstrengthpod.com`** (pod). Do NOT use the old `decentralizedpod.com`. Grep before shipping.
- The landing uses its **own** evolved-hexagon mark — the podcast mark belongs to the pod site and stays over there.
- `logo-cover.png` is the og:image at **1200×630, mark-only** (kept consistent with the pod + SCAI logo-only previews).

## Logo generator
- `decentralized.com/make_ds_logo.py` (in the `/home/ollie/Decentralized strength LLC/decentralized.com/` workspace, NOT committed here) regenerates all landing logo PNGs. After rerunning, copy the PNGs into this `site/` dir and push.

## Associated sites (hosting model)
| Site | Repo | Deploy |
|------|------|--------|
| `decentralizedstrengthpod.com` | `ollieadam/decentralizedstrengthpod` | GitHub Pages (podcast/blog) |
| `strengthclubai.com` | `ollieadam/strengthclubai` | Cloudflare tunnel → localhost:8082 |
| `chsstrengthclub.com` | `ollieadam/chsstrengthclub` | GitHub Pages |