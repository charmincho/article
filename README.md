# Remarble Research · Longform Essays

A collection of longform essays on Asia-Pacific residential real estate investment, synthesizing institutional research with classical urban economics frameworks.

**Live URL**: [article.remarble.co](https://article.remarble.co)

---

## Site Structure

```
article.remarble.co/
├── index.html              ← Landing page
├── apac/
│   └── index.html          ← "Why Now, Why Living?"
├── seoul/
│   └── index.html          ← "Demand, Supply, Capital"
└── macro-policy/
    └── macro-policy.html   ← "The Macro Holds, The Policy Doesn't"
```

| URL | Article |
|---|---|
| `/` | Landing — Article Index |
| `/apac/` | Why Now, Why Living? |
| `/seoul/` | Demand, Supply, Capital |
| `/macro-policy/macro-policy.html` | The Macro Holds, The Policy Doesn't |

---

## Articles

### 1. Why Now, Why Living? · April 2026 · 18 min
APAC overview synthesizing 18 leading global research houses' 2026 outlooks through the classical frameworks of Alonso, Marshall, Glaeser, and Tiebout. Covers Tokyo, Seoul, Singapore, Sydney, and other gateway markets.

### 2. Demand, Supply, Capital · May 2026 · 12 min
The first of three essays on Seoul's rental market. Reads the structural shift through three forces: rising demand (1-person households, tourism, foreign students), tightening supply (housing permits down 70% from peak, low supply elasticity), and rotating capital (jeonse cracking, monthly rent at 74.5%).

### 3. The Macro Holds, The Policy Doesn't · May 2026 · 13 min
The second of three essays on Seoul's rental market. Reads the macro and policy environment around the structural case: where Korea sits in the APAC cost-of-capital stack (a −1.25% rate inversion running past 40 months), the buffer that absorbs the currency pressure (record current-account surplus, ~$427B reserves, export strength), and the constraint that household debt at 89.4% of GDP forces onto housing policy — closing both institutional entry routes.

*Forthcoming:*
- Essay 3 · Where Opportunities Sit — Operator partnerships and entry pathways

---

## Adding a New Article

1. Create a new folder at the repo root, e.g., `/macro/`
2. Add `index.html` using the same design system
3. Copy `Remarble-Primary.png` and `Remarble-White.png` into the folder
4. Update the landing page (`/index.html`) — add a new `<a class="article-card">` block in the `.article-grid` section
5. Commit and push

The design tokens are consistent across files:
- Fonts: Newsreader, Playfair Display, Inter, Noto Serif KR, JetBrains Mono
- Accent green: `#0FC76F` (warm) and `#05342C` (deep, light theme) / `#4FDB9A` (dark theme)
- Dark theme is the default; light theme is toggleable

---

## Deployment

### 1. GitHub Pages Setup
1. Push to a public GitHub repository
2. Settings → Pages → Source: `main` branch, `(root)` folder
3. Save

### 2. Custom Domain
The `CNAME` file is already configured for `article.remarble.co`.

Required DNS record (at your DNS provider — WordPress.com / Cloudflare / etc.):
```
Type:   CNAME
Name:   article
Value:  YOUR-GITHUB-USERNAME.github.io
TTL:    3600
```

### 3. Enable HTTPS
After DNS propagation (10 min – 2 hours):
- GitHub Settings → Pages → Check "Enforce HTTPS"

---

## Design System

Every page (landing + articles) shares the same design tokens:

| Token | Value |
|---|---|
| Default theme | Dark |
| Background (dark) | `#14130F` |
| Background (light) | `#FAF7F0` |
| Accent warm | `#0FC76F` |
| Accent deep (light) | `#05342C` |
| Accent green (dark) | `#4FDB9A` |
| Accent gold | `#C9A55F` |
| Display font | Playfair Display |
| Body serif | Newsreader |
| Sans-serif | Inter |
| Mono | JetBrains Mono |

Each article has:
- Sticky masthead with logo, brand label, in-page nav, EN/KO toggle, theme toggle
- Reading-progress bar
- Reveal-on-scroll animations
- Mobile-responsive layout (twin charts and grids collapse to single column at narrow widths)

---

## Tech

- Pure HTML/CSS/JavaScript — no framework, no build step
- Chart.js (loaded from CDN) for embedded visualizations in articles
- Fonts loaded from Google Fonts CDN
- Self-contained (no other external dependencies)

---

## About Remarble

Remarble is an APAC-focused real estate intelligence firm, building Seoul-grade analytical frameworks for institutional Living sector investors across gateway markets.

[remarble.co](https://remarble.co)

---

*© 2026 Remarble · APAC Real Estate Intelligence*
