# Hypertrophy Training Hub

A professional strength and hypertrophy knowledge base built from 20 years of coaching experience by Coach Vladimir Brusov. Evidence-based, practically tested training, nutrition, and recovery guidance — no academic filler.

**Live site:** https://hypertrophy.brusovcoach.org

---

## What It Is

A static single-page knowledge base covering everything an athlete needs to understand and apply hypertrophy training — from foundational philosophy to advanced periodization. Built for competitive bodybuilders, powerlifters, and high-performance athletes who want actionable principles, not theory.

Core philosophy: progressive overload is the mechanism. Everything else — exercise selection, rep ranges, split structure — exists to support that one goal.

---

## Tech Stack

| Layer | Choice |
|-------|--------|
| Structure | HTML5 |
| Styling | CSS3 (custom properties, flexbox, grid) |
| Interactivity | Vanilla JS (ES6+, no frameworks) |
| Fonts | Barlow Condensed + DM Sans (Google Fonts) |
| Backend | None |
| Database | None |
| Build step | None |
| Dependencies | Zero |

Single file application. All HTML, CSS, and JavaScript live in `index.html`.

---

## File Structure

```
HypertrophyHub/
├── index.html      All HTML, embedded CSS, and inline JS (~2,340 lines)
├── robots.txt      Allows all crawlers, references sitemap
└── sitemap.xml     Primary page URL, monthly update frequency
```

---

## Content Sections

| # | Section | Category | Read Time |
|---|---------|----------|-----------|
| 1 | Philosophy | Start Here | — |
| 2 | Beginner Guide | Start Here | 6 min |
| 3 | Training Principles | Core Principles | 4 min |
| 4 | Volume | Core Principles | 4 min |
| 5 | Frequency | Core Principles | 3 min |
| 6 | Progressive Overload | Core Principles | 5 min |
| 7 | Intensity & Effort | Execution | 4 min |
| 8 | Exercise Selection | Execution | 6 min |
| 9 | Program Design | Execution | 4 min |
| 10 | Special Techniques | Execution | 4 min |
| 11 | Recovery | Support | 3 min |
| 12 | Nutrition | Support | 15 min |
| 13 | Advanced Concepts | Support | 5 min |
| 14 | Mindset & Application | Support | 3 min |
| 15 | Key Numbers Reference | Reference | 2 min |

---

## Key Reference Numbers

| Metric | Value |
|--------|-------|
| Minimum volume threshold | 5 sets / muscle / week |
| Productive volume range | 10–16 sets / muscle / week |
| Max effective volume per session | 10 sets / muscle |
| Optimal training frequency | 2x / week per muscle |
| Hypertrophy rep range | 6–12 reps |
| Strength rep range | 1–5 reps |
| Metabolic stress rep range | 13+ reps (to failure) |
| Effective effort range | RIR 0–3 |
| Upper body load increment | 2–2.5 kg |
| Lower body load increment | 5 kg |
| Eccentric tempo | 2–3 seconds |

---

## JavaScript Features

**Scroll progress bar** — 3px left-edge bar on the sidebar tracks reading progress via `window.scrollY`.

**Active nav link** — `IntersectionObserver` highlights the correct sidebar link as sections scroll into view (threshold: 20%, rootMargin: `-10% 0px -70% 0px`).

**Real-time search** — filters all 14 sections live on input, case-insensitive, searches full text content.

**Mobile menu** — slide-in drawer (85vw, max 320px) with backdrop overlay. Hamburger toggle, close button, backdrop click, and nav link click all close the menu.

**Auto copyright year** — footer year updates dynamically via `new Date().getFullYear()`.

---

## Layout

**Desktop:** sticky sidebar (left) with scroll progress bar + sticky filter/search bar below hero + main content area.

**Mobile:** sticky top bar with back button + hamburger menu toggle. Menu slides in from left with semi-transparent backdrop.

---

## Design System

Dark theme with orange accent.

| Variable | Value | Use |
|----------|-------|-----|
| `--bg` | `#0a0a0b` | Primary background |
| `--accent` | `#d4500a` | Primary orange accent |
| `--beginner` | `#1fa855` | Green — beginner badges |
| `--intermediate` | `#d4920a` | Amber — intermediate badges |
| `--advanced` | `#d43030` | Red — advanced badges |
| `--text` | `#e2e2e6` | Primary text |
| `--text-secondary` | `#a8a8b3` | Secondary text |

Content uses three knowledge tiers: **Foundation** (green) / **Deeper** (amber) / **Advanced** (red).

---

## Deployment

No build step. No environment variables. Push and it's live.

```bash
git add index.html
git commit -m "your message"
git push
```

Auto-deploys on push. The PAT is baked into the remote URL.

---

## Related Sites

- **Main site:** https://brusovcoach.org
- **Health & Longevity Hub:** https://health.brusovcoach.org
- **Contact:** vladimirbrusov83@gmail.com
