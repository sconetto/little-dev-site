# Little Development Tech

Corporate website for **Little Development Ltda** — a technology and consultancy company.

> **Focus on you, leave the little developments to us.**

Built with [Hugo](https://gohugo.io/) and the [HugoBlox](https://hugoblox.com/) framework. Bilingual: Portuguese (Brazil) and English.

**Production site:** [littledevelopment.tech](https://littledevelopment.tech)

---

## Prerequisites

- [Git](https://git-scm.com/)
- [Go](https://go.dev/dl/) 1.26+ (required by Hugo Modules)
- [asdf](https://asdf-vm.com/) — version manager (installed via [Homebrew](https://brew.sh/) on macOS)
  - macOS: `brew install asdf`
- [Hugo](https://gohugo.io/installation/) (extended edition) — **pinned to v0.162.0 via asdf** (see [.tool-versions](.tool-versions))
- [pnpm](https://pnpm.io/) v10.14.0 — package manager (install via `npm install -g pnpm` or `brew install pnpm`)

### Setting up asdf

After installing asdf, add the Hugo plugin and install the project's pinned version:

```bash
# From the project root
asdf plugin add hugo
asdf install
```

Verify the correct version is active:

```bash
hugo version
# Should show: hugo v0.162.0
```

> **Note:** Hugo version is pinned to v0.162.0 for HugoBlox v0.12.0 compatibility.

---

## Development

### 1. Clone the repository

```bash
git clone <repo-url>
cd little-dev
```

### 2. Install JS dependencies

```bash
pnpm install
```

### 3. Start the dev server

```bash
hugo server --disableFastRender
```

This starts a local development server with live reload at the displayed URL (default **http://localhost:1313**).

- The server watches content, config, layouts, and HugoBlox module files
- Hot reload applies changes without full rebuild

### Available languages

- **Portuguese (Brazil):** `http://localhost:1313/` (default)
- **English:** `http://localhost:1313/en/`

---

## Project Structure

```
little-dev/
├── .tool-versions               # Hugo v0.162.0 pinned via asdf
├── .gitignore                   # Hugo, Node.js, OS files
├── go.mod                       # Hugo Modules: blox v0.12.0 + netlify
├── hugoblox.yaml                # Build config (Hugo version, deploy target, template ID)
├── package.json                 # JS deps: Tailwind v4, Preact, Pagefind
├── config/
│   └── _default/
│       ├── hugo.yaml            # Core Hugo configuration (SaaS template)
│       ├── module.yaml          # Hugo Module imports + mounts
│       ├── params.yaml          # HugoBlox theme parameters (full config)
│       ├── languages.yaml       # Bilingual config + per-language menus (main + footer)
│       └── menus.yaml           # Footer menu definitions
├── content/
│   ├── pt/                      # Portuguese content (default language)
│   │   ├── _index.md            # SaaS-style landing page with blocks
│   │   ├── privacy.md           # Privacy policy
│   │   ├── terms.md             # Terms of service
│   │   └── blog/                # Blog listing
│   │       └── _index.md
│   └── en/                      # English content
│       ├── _index.md            # SaaS-style landing page with blocks
│       ├── privacy.md           # Privacy policy
│       ├── terms.md             # Terms of service
│       └── blog/                # Blog listing
│           └── _index.md
├── data/
│   └── authors/
│       └── sconetto.yaml        # Author profile
├── assets/
│   └── media/                   # Brand assets (images, SVGs)
├── layouts/                     # Custom template overrides (optional)
├── i18n/                        # Translation overrides (optional)
├── hugo-blox/                   # Local block overrides (optional)
├── public/                      # Build output (gitignored)
└── .opencode/
    └── memory-bank/             # Project context for AI-assisted dev
```

---

## Adding Content

### Landing page blocks

The homepage is built from YAML blocks defined in `content/{pt,en}/_index.md`. Available blocks (SaaS template):

| Block ID | Purpose |
|----------|---------|
| `hero` | Full-width hero with gradient, CTAs, announcements, trust signals |
| `logos` | Client logo marquee/grid |
| `stats` | Statistics/metrics display with gradient numbers |
| `steps` | "How we work" step-by-step horizontal layout |
| `features` | Services/benefits grid with icons (bento layout) |
| `comparison-table` | Competitor comparison table |
| `pricing` | Pricing tiers with monthly/yearly toggle |
| `cta-image-paragraph` | Alternating image + text sections with feature lists |
| `testimonials` | Customer testimonials with images |
| `faq` | Frequently asked questions accordion |
| `cta-card` | Gradient card with call-to-action |

### Adding a new page

For regular content pages (blog, privacy, etc.):

```bash
hugo new content/pt/blog/my-post/index.md
hugo new content/en/blog/my-post/index.md
```

### Important

- Always write content in **both languages** (PT in `content/pt/`, EN in `content/en/`)
- Set `draft: false` when ready to publish
- Images referenced in blocks go in `assets/media/`
- Blog posts should reference an author from `data/authors/`

---

## Building for Production

```bash
pnpm run build
```

This runs:
1. `hugo --minify` — builds the static site
2. `pnpm run pagefind` — generates search index (when search is enabled)

The output is written to `public/` — a fully static site.

---

## Deployment

The site is a collection of static files — no server-side runtime required. Deploy to any static hosting:

- **GitHub Pages** (default target in `hugoblox.yaml`)
- **Netlify**
- **Vercel**
- **Cloudflare Pages**

Connect your git repository to the hosting provider for automatic deployments.

---

## License

GNU General Public License v3.0 — see [LICENSE](LICENSE) for details.
