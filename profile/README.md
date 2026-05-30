# SWORN

**Calm the Urge. Keep the Oath.**

SWORN is a daily drink formula for men who struggle with sexual compulsivity — reverse-engineered from post-nut clarity, the neurochemical clarity that arrives *after* the act, delivered *before* it.

*Post-nut clarity before, not after.*

## How It Works

**The Formula** — A clinically-dosed black powder drink mix: NAC, KSM-66 Ashwagandha, L-Theanine, 5-HTP, L-Tryptophan, Vitamin B6, and Chasteberry (activated charcoal, blood orange). One scoop, 8oz water, no stimulants. Taken when the urge hits — making it is the pattern interrupt.

**The Coach** — A private AI coach over SMS that learns your patterns and checks in proactively when the urge is likely. Available 24/7 when you reach out.

**The Streak** — Consecutive days of discipline. Take the formula, resist the urge, build the streak.

| Plan | Price | Details |
|------|-------|---------|
| Subscribe & Save | $49/month | Free shipping · cancel, skip, or edit anytime |
| One-time | $69 | Single order |

---

## Engineering

Everything SWORN runs on lives in one consolidated monorepo — **`platform`**.

| Repo | What it is |
|------|------------|
| [`platform`](https://github.com/SwornCo/platform) | One Elixir/Phoenix app (`:sworn`) — accounting, the AI SMS coach, marketing automation, and the internal admin console — deployed to a single host on a single Postgres. Also home to the Shopify storefront theme and the content workspaces. |

> Formerly five side-by-side services (website, marketing, marketing-ops, ai-coach, accounting). Consolidated into `platform` in 2026 — one app, one deploy, one database.

## Brand & voice

`product-marketing-context.md` (in `platform`) is the single source of truth for SWORN's voice, audiences, and positioning — quiet conviction, direct about sexual compulsivity, the post-nut clarity origin, and the category-creating claim. Edit it once; every surface draws from it.
