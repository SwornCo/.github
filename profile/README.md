# SWORN

> Calm the urge. Keep the oath.

SWORN is the first daily discipline protocol built specifically for men who are done being controlled by their impulses. It combines a clinically-dosed drink mix, an AI-powered SMS accountability coach, and a daily streak tracker into one system — giving men the neurochemical support and structural accountability that willpower alone can't provide.

**One scoop. One coach. One oath. Every day.**

## How It Works

1. **The Drink** — A black powder mix (activated charcoal, blood orange) containing NAC, KSM-66 Ashwagandha, L-Theanine, 5-HTP, L-Tryptophan, Vitamin B6, and Chasteberry. Taken when urges hit — the act of making it is the pattern interrupt.
2. **The Coach** — A private AI SMS system that learns when you need it most and reaches out first. Always available when you reach out. It knows your name, your goal, and your patterns.
3. **The Streak** — A daily scoreboard that tracks consecutive days of adherence, giving discipline a visible, protectable record.

| Plan | Price | Details |
|------|-------|---------|
| Subscribe & Save | $79/month | Free shipping, cancel anytime |
| One-time Purchase | $99 | Single order |

## Repository Structure

```
sworn/
├── ai-coach/            # SMS coaching backend (TypeScript/Express/Claude)
├── ingredients-video/   # Remotion video generator for ingredient animations
├── marketing/           # Brand, content, press, social — all marketing assets
└── website/             # Eleventy marketing site (auto-deploys to Netlify)
```

Each directory is an independent git repository with its own remote.

---

## AI Coach — [`ai-coach/`](https://github.com/SwornCo/ai-coach)

TypeScript/Express backend that connects Shopify orders to a personalized SMS coaching experience powered by Claude. Handles the full user lifecycle: order → onboarding → daily check-ins → coaching → streak milestones → retention.

**Stack:** TypeScript · Express · PostgreSQL · Twilio · Anthropic Claude · node-cron
**GitHub:** [SwornCo/ai-coach](https://github.com/SwornCo/ai-coach)

```bash
cd ai-coach && cp .env.example .env && npm install && npm run dev
```

---

## Website — [`website/`](https://github.com/SwornCo/website)

The sworn.co marketing site. A responsive landing page built with Eleventy and SCSS, auto-deployed to Netlify on every push to `main`.

**Stack:** Eleventy (11ty) v3 · Nunjucks · SCSS/BEM · Vanilla JS · Swiper.js
**GitHub:** [SwornCo/website](https://github.com/SwornCo/website)

```bash
cd website && npm install && npm start
```

---

## Marketing — [`marketing/`](https://github.com/SwornCo/marketing)

The single home for all brand, content, and campaign assets. Houses the product marketing context document (the source of truth read before any marketing task), approved copywriting, press releases, social media templates, science research, and strategic planning.

**Key areas:** Brand guidelines · Copywriting · Press releases · Instagram pipeline · Google My Business · Science research · Strategy docs

```bash
cd marketing
# Content is mostly markdown/PDF — no build step
# For Instagram post generation:
cd social/instagram && node capture.mjs
```

---

## Ingredients Video — [`ingredients-video/`](https://github.com/SwornCo/ingredients-video/)

Remotion-based video generator that creates ingredient breakdown animations for the website and social media channels.

**Stack:** Remotion · React · TypeScript

```bash
cd ingredients-video && npm install && npx remotion studio
```

---

## Links

- **Website:** [sworn.co](https://sworn.co)
- **Design:** [Figma — SWORN Website](https://www.figma.com/design/pJ9Cdg0QcSqldJ0a3mElYB/Sworn-Website-Figma)

---

**Built for the man you've sworn to become.**
