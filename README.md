# Grey One Constructions — Website

A single-page, glassmorphism-style marketing site for **Grey One Constructions**, a design-build construction studio serving The Nilgiris & Coimbatore.

Built as one static HTML file — no build step, no dependencies to install. Open it and it works.

## Live preview

Open `index.html` in any modern browser, or serve the repo with GitHub Pages (see below).

## Tech stack

- **HTML5** — semantic markup (`header`, `nav`, `section`, `footer`)
- **CSS3** — custom properties (design tokens), Grid/Flexbox layout, `backdrop-filter` glass effects, keyframe animations
- **Vanilla JavaScript** — no frameworks or libraries
- **Google Fonts** — [Big Shoulders Display](https://fonts.google.com/specimen/Big+Shoulders+Display), [Manrope](https://fonts.google.com/specimen/Manrope), [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono), loaded via CDN

Everything (HTML, CSS, JS) lives in `index.html` — nothing to compile or bundle.

## Sections

| Section | What it contains |
|---|---|
| Nav | Glassy floating nav bar, logo mark, mobile hamburger menu |
| Hero | Headline, subtitle, CTAs, animated glass version of the brand mark |
| Stats | Projects delivered, years in practice, sq ft built, on-time rate (count-up on scroll) |
| Services | Six service cards (residential, commercial, renovation, architecture, project management, sustainable building) |
| Work | Project showcase grid with abstract isometric illustrations |
| Clients | Testimonial cards |
| Pricing | Three project tiers — Foundation / Structure / Penthouse |
| Contact | Contact details + inquiry form (client-side only, no backend) |
| Footer | Sitemap, social links, copyright |

## Features

- Fully responsive (desktop → tablet → mobile)
- Scroll-triggered reveal animations via `IntersectionObserver`
- Count-up number animation on the stats strip
- Mouse-parallax tilt on the hero's glass shapes
- Glossy shine sweep on card hover
- Respects `prefers-reduced-motion`
- Keyboard-visible focus states

## Customizing content

Open `index.html` and search for these sections — all copy is plain text in the markup, no CMS or data file:

- **Contact details** — `id="contact"` section
- **Stats** — `data-count` / `data-suffix` attributes in the `.go-stats` section
- **Services** — `.go-feature-card` blocks
- **Projects** — `.go-project-card` blocks
- **Testimonials** — `.go-test-card` blocks
- **Pricing** — `.go-price-card` blocks
- **Colors / fonts** — CSS custom properties at the top of the `<style>` block (`:root`)

## ⚠️ Still placeholder

A few things were left as reasonable placeholders and should be reviewed before this goes fully live:

- On-Time Rate stat (currently 98%)
- Business hours (currently Mon–Fri, 7:00 AM – 5:00 PM)
- Project names, testimonial quotes, and client names in the **Work** and **Clients** sections
- Pricing tier amounts
- Social links in the footer (currently point to `#`)

## Deploying with GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Source**, select the branch (e.g. `main`) and root folder.
4. Save — your site will be live at `https://<username>.github.io/<repo-name>/`.

## License

Site code: free to use and modify for Grey One Constructions. Fonts are served under their respective open licenses via Google Fonts.
