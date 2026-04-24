# APAC Living Sector 2026 · Remarble Longform Essay

A longform essay on Asia-Pacific residential real estate investment, synthesizing 18 global research houses' 2026 outlooks with classical urban economics frameworks.

**Live URL**: [article.remarble.co](https://article.remarble.co)

---

## Files

| File | Description |
|---|---|
| `index.html` | English edition (main) |
| `index_ko.html` | Korean edition (한국어판) |
| `thumb.png` | Open Graph / social thumbnail (dark theme, 2400×1256) |
| `CNAME` | Custom domain: `article.remarble.co` |
| `README.md` | This file |

---

## Deployment

### 1. GitHub Pages Setup

1. Create a public GitHub repository
2. Upload all files to the repository root
3. Settings → Pages → Source: `main` branch, `(root)` folder
4. Save

### 2. Custom Domain (WordPress.com DNS)

Add CNAME record:
```
Type:   CNAME
Name:   article
Value:  YOUR-GITHUB-USERNAME.github.io
TTL:    3600
```

### 3. Enable HTTPS

After DNS propagation (10min–2hr):
- GitHub Settings → Pages → Check "Enforce HTTPS"

---

## Language Toggle

The header contains an EN/KO toggle allowing seamless switching between editions. Both files are stand-alone HTML documents with identical design, structure, and interactive elements (dark/light mode, charts, reveal animations).

### Link Structure

- **English** (main): `https://article.remarble.co` → `index.html`
- **Korean**: `https://article.remarble.co/index_ko.html`

---

## Structure (Both Editions)

- **Cover** — Why Now, Why Living?
- **Chapter I** — The Question
- **Chapter II** — The Three Shifts (Households · Supply · Capital)
- **Chapter III** — The Framework (Alonso · Marshall · Glaeser · Tiebout)
- **Chapter IV** — The Markets
  - Market Architecture (4 cards)
  - Tokyo · Developer-Led
  - Seoul · Informal Finance-Driven
  - Singapore · State-Led
  - Australia · Global Capital Competition
  - Other Markets (Hong Kong, China, India)
- **Chapter V** — Strategy (Core / Core+ / Value-Add / Opportunistic)
- **Chapter VI** — Risk (Macro · Policy · Execution)
- **Closing** — From "emerging" to "core"
- **Sources** — 21 institutional references

---

## Tech

- Pure HTML/CSS/JavaScript (no framework, no build step)
- Chart.js for embedded visualizations
- System fonts: Inter (sans), Playfair Display (display), JetBrains Mono (mono)
- Dark mode default, light mode toggle
- Self-contained (no external assets beyond CDN fonts)

---

## About Remarble

Remarble is an APAC-focused real estate intelligence firm, building Seoul-grade analytical frameworks for institutional Living sector investors across gateway markets.

[remarble.co](https://remarble.co)

---

*© 2026 Remarble. Published April 2026.*
