# SWORN

**Calm the Urge. Keep the Oath.**

SWORN is the daily discipline protocol for men who are done being controlled by their impulses. A clinically-dosed drink, a private AI coach, and a streak system — neurochemical support and structural accountability that willpower alone can't provide.

One scoop. One coach. One oath. Every day.

## How It Works

**The Drink** — A black powder mix containing NAC, KSM-66 Ashwagandha, L-Theanine, 5-HTP, L-Tryptophan, Vitamin B6, and Chasteberry. Taken when urges hit — the act of making it is the pattern interrupt.

**The Coach** — A private AI SMS system that learns when you're most vulnerable and reaches out first. Always on-call when you reach out. It knows your name, your goal, and your patterns.

**The Streak** — A daily scoreboard tracking consecutive days of discipline. Something worth protecting. A visible record that the man you're becoming is winning.

| Plan | Price | Details |
|------|-------|---------|
| Subscribe & Save | $79/month | Free shipping, cancel anytime |
| One-time Purchase | $99 | Single order |

---

## Repositories

| Repo | Purpose |
|------|---------|
| `website/` | Marketing website — Eleventy + Nunjucks + SCSS, deployed on Netlify |
| `marketing/` | Marketing content — social media assets, copywriting, Instagram HTML-to-PNG pipeline |
| `marketing-ops/` | Marketing operations — campaign tooling, automation, and analytics workflows |
| `ai-coach/` | AI accountability coach — SMS-based coaching system |
| `accounting/` | Financial operations and bookkeeping |

## Shared Configuration

### `CLAUDE.md`
Cross-project guidelines for Claude Code — design principles, reusable UI patterns, and brand voice rules. Automatically loaded by any Claude Code session in any subdirectory.

### `.agents/product-marketing-context.md`
Single source of truth for SWORN's product marketing context — brand voice, target audiences, IYKYK principle, two-layer marketing model, ingredient details, and competitive positioning. Used by the marketing-skills plugin across all repos.

Each repo symlinks to this file:

```
sworn/
├── .agents/product-marketing-context.md   ← source of truth
├── website/.agents/product-marketing-context.md → symlink
├── marketing/.agents/product-marketing-context.md → symlink
├── marketing-ops/.agents/product-marketing-context.md → symlink
├── ai-coach/.agents/product-marketing-context.md → symlink
└── accounting/.agents/product-marketing-context.md → symlink
```

To update the product marketing context, edit the root file — all repos pick up changes automatically:

```bash
vi .agents/product-marketing-context.md
```
