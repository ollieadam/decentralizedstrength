# Decentralized Strength LLC Landing — Agent Context

## Project Overview

The parent website for Decentralized Strength LLC — holdings doors plus the journal. Hosted by Adam Oliver, CSCS.

**URL:** https://decentralizedstrength.com
**Repo:** `ollieadam/decentralizedstrength` (GitHub Pages, `main/root`)
**Deploy:** push to `main` → auto-deploys via GitHub Pages.

## Purpose
The **parent website** (not the podcast site). Above the fold: one-line mark + holdings doors (Pod, Strength Club AI, Charleston Strength Club, YouTube, Reach the Coach, Barbie the Pug). Journal / philosophy lives **below the fold**. Essays are canonical on this domain. Brand identity includes "self-directed positional trader/investor — blockchain & crypto."

## Structure
- `index.html` — parent shell (one-line mark, holdings doors, journal list). SEO meta + JSON-LD Organization.
- `site.css` — cream paper `#f7f4ef`, ink `#000000`, wash `#efebe4`, mid `#6b6b6b`, line `#e5e5e5`. Georgia/Times + ui-monospace kickers. No red.
- `blog/` — essays that live here (`the-4-ps`, `robust-aging`, `pro-level-results-from-a-park`). Canonicals on `decentralizedstrength.com`.
- `philosophy.html` — short 4 P’s stack; links to the essay on this domain.
- `logo.png` — **same hex+barbell lockup as the podcast site** (`decentralizedstrengthpod.com/logo.png`). Used in header + JSON-LD.
- `logo-cover.png` — og:image at **1200×630, mark-only** (kept consistent with the pod + SCAI logo-only previews).
- `logo-mark.png` / `favicon.png` / `apple-touch-icon.png` — mark icons.
- `CNAME`, `sitemap.xml`, `README.md`, GSC token.

## Brand rules
- Domain strings: **`decentralizedstrength.com`** (this site) and **`decentralizedstrengthpod.com`** (pod). Do NOT use the old `decentralizedpod.com`. Grep before shipping.
- **Same logo on both sites:** parent `/logo.png` is the podcast hex+barbell lockup. Do not ship a second mark for the parent header.
- `logo-cover.png` is the og:image at **1200×630, mark-only** (kept consistent with the pod + SCAI logo-only previews).

## Logo generator
- `decentralized.com/make_ds_logo.py` (in the `/home/ollie/Decentralized strength LLC/decentralized.com/` workspace, NOT committed here) regenerates all landing logo PNGs. After rerunning, copy the PNGs into this `site/` dir and push.

## Associated sites (hosting model)
| Site | Repo | Deploy |
|------|------|--------|
| `decentralizedstrengthpod.com` | `ollieadam/decentralizedstrengthpod` | GitHub Pages (podcast/blog) |
| `strengthclubai.com` | `ollieadam/strengthclubai` | Cloudflare tunnel → localhost:8082 |
| `chsstrengthclub.com` | `ollieadam/chsstrengthclub` | GitHub Pages |