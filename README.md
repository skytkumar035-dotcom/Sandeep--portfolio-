# Sandeep Kumawat — Portfolio Website
**Business Data Cleaning & CRM Optimization Specialist**

Live preview: open `index.html` in any browser.

---

## Folder Structure

```
sandeep-portfolio/
│
├── index.html               ← Home page
├── README.md                ← This file
│
├── css/
│   ├── style.css            ← Global styles (nav, footer, buttons, components)
│   └── home.css             ← Home page hero styles
│
├── js/
│   └── main.js              ← Nav scroll, counters, animations, mobile menu
│
└── pages/
    ├── services.html        ← Services + Pricing + FAQ
    ├── portfolio.html       ← Case Studies + Audit reports
    ├── about.html           ← Professional bio + toolset
    └── contact.html         ← Contact form + Fiverr integration
```

---

## Deployment — GitHub Pages (Free)

### Step 1: Create a GitHub account
Go to https://github.com and sign up (free).

### Step 2: Create a new repository
- Click **New Repository**
- Name it: `sandeep-portfolio` (or any name)
- Set to **Public**
- Click **Create Repository**

### Step 3: Upload files
- Click **uploading an existing file**
- Drag and drop the entire `sandeep-portfolio/` folder contents
- Commit with message: `Initial portfolio upload`

### Step 4: Enable GitHub Pages
- Go to your repo → **Settings** → **Pages**
- Source: **Deploy from a branch**
- Branch: `main` → folder: `/ (root)`
- Click **Save**

### Step 5: Live in ~2 minutes
Your site will be live at:
`https://YOUR-USERNAME.github.io/sandeep-portfolio/`

---

## Deployment — Replit (Alternative)

1. Go to https://replit.com → **Create Repl**
2. Choose **HTML, CSS, JS** template
3. Delete default files
4. Upload all files maintaining folder structure
5. Click **Run** — live URL provided instantly

---

## How to Edit Content

### Change your email
Search for `overlimits.data@gmail.com` across all files and replace.

### Change your Fiverr URL
Search for `fiverr.com/john_snow_10` across all files and replace with your actual Fiverr URL.

### Update statistics (Home page hero)
In `index.html`, find the `.hero-stats` section:
```html
<span class="stat-num" data-target="150">0</span>  ← Projects Done
<span class="stat-num" data-target="98">0</span>   ← Accuracy %
<span class="stat-num" data-target="50">0</span>   ← Happy Clients
<span class="stat-num" data-target="2">0</span>    ← Records (M+)
```
Change `data-target` values to update the animated counters.

### Add your real photo (About page)
In `pages/about.html`, find the `.about-photo` div and replace the placeholder with:
```html
<img src="../assets/sandeep.jpg" alt="Sandeep Kumawat" />
```
Then add your photo as `assets/sandeep.jpg`.

### Update testimonials
In `index.html`, find the `.testimonials-grid` section and edit the client quotes, names, and roles.

### Add/remove services
In `pages/services.html`, find `.services-full` and copy/paste an `.sf-card` block.

### Change brand colors
In `css/style.css`, update the CSS variables at the top:
```css
--navy: #0F172A;      /* Main dark color */
--blue: #2563EB;      /* Accent blue */
--blue-pale: #EFF6FF; /* Light blue backgrounds */
```

---

## Favicon Recommendation

Use **Favicon.io** (https://favicon.io/favicon-generator/):
- Text: `SK`
- Background: `#0F172A` (navy)
- Font color: `#FFFFFF`
- Font: **Inter Bold**

Download and add to root folder, then add to each HTML `<head>`:
```html
<link rel="icon" type="image/png" href="favicon.png"/>
```

---

## Icon Recommendations

All icons in this project are **inline SVG** — no dependencies needed.
For additional icons: **Lucide Icons** (https://lucide.dev) — same style, free, copy as SVG.

---

## Free Illustration Sources

- **Storyset** (https://storyset.com) — data/tech illustrations, free with attribution
- **unDraw** (https://undraw.co) — flat SVG illustrations, fully free
- **Humaaans** (https://humaaans.com) — people illustrations

---

## SEO Optimization

Each page has:
- Unique `<title>` tags
- `<meta name="description">` tags
- Semantic HTML structure (h1 → h2 → h3 hierarchy)
- Mobile-responsive viewport meta tag

To add more SEO, include in each `<head>`:
```html
<meta property="og:title" content="Sandeep Kumawat — Data Cleaning Specialist"/>
<meta property="og:description" content="Professional CRM cleanup and data management services."/>
<meta property="og:image" content="https://YOUR-SITE/assets/og-image.png"/>
```

---

## Responsive Breakpoints

| Breakpoint | Layout |
|---|---|
| `> 1024px` | Full desktop — 3-col grids, side-by-side panels |
| `768px – 1024px` | Tablet — 2-col grids, stacked audit section |
| `< 768px` | Mobile — single column, hamburger nav |

---

## Performance Tips

- All fonts loaded from Google Fonts with `preconnect`
- CSS is split (global + page-specific) for faster loads
- Animations use `IntersectionObserver` — only trigger when visible
- No external JS libraries — pure vanilla JS
- All SVG icons are inline — zero image requests

---

## Contact

**Email:** overlimits.data@gmail.com  
**Fiverr:** https://www.fiverr.com/john_snow_10?public_mode=true
