# 🏋️ Iron Forge — Elite Performance Gym Website

A full, single-file static gym website built with pure HTML, CSS, and vanilla JavaScript. Bold industrial design with smooth animations and a fully responsive layout.

---

## 📁 Project Structure

```
gym-website.html   # Complete website — all HTML, CSS, and JS in one file
README.md          # This file
```

---

## 🚀 Getting Started

No build tools, no dependencies, no npm. Just open the file.

```bash
# Clone or download the file, then:
open gym-website.html
```

Or serve it locally for best results:

```bash
# Python 3
python -m http.server 8000

# Node.js (npx)
npx serve .
```

Then visit `http://localhost:8000/gym-website.html` in your browser.

---

## 📐 Sections

| Section | Description |
|---|---|
| **Nav** | Fixed top bar with scroll-blur effect and CTA button |
| **Hero** | Full-viewport header with animated grid, stats, and call-to-action |
| **Marquee** | Infinite-scroll red banner with service tags |
| **About** | Two-column layout with image accent, badge overlay, and feature list |
| **Programs** | Hover-reveal 3-card program gallery |
| **Trainers** | 4-column team grid with color-reveal on hover |
| **Pricing** | 3-tier membership cards with a featured center plan |
| **Testimonials** | Member review cards with star ratings |
| **CTA Banner** | Full-width join prompt with phone link |
| **Footer** | 4-column footer with links, hours, and social icons |

---

## 🎨 Design System

### Fonts
- **Display:** [Bebas Neue](https://fonts.google.com/specimen/Bebas+Neue) — headings, logo, stats
- **Condensed UI:** [Barlow Condensed](https://fonts.google.com/specimen/Barlow+Condensed) — labels, nav, buttons
- **Body:** [Barlow](https://fonts.google.com/specimen/Barlow) — paragraphs, descriptions

### Color Palette

| Variable | Value | Usage |
|---|---|---|
| `--black` | `#0a0a0a` | Page background |
| `--deep` | `#111111` | Section backgrounds |
| `--charcoal` | `#1c1c1c` | Cards, trainer section |
| `--red` | `#e63329` | Primary accent, CTA |
| `--gold` | `#c9a84c` | Star ratings |
| `--white` | `#f5f5f0` | Primary text |
| `--smoke` | `#888888` | Muted/secondary text |

### Key CSS Features
- CSS custom properties (variables) for consistent theming
- `clip-path: polygon(...)` for diagonal-cut buttons
- `IntersectionObserver` for scroll-reveal animations
- CSS `@keyframes` for marquee loop and hero grid shift
- `backdrop-filter: blur()` on the navbar

---

## 📱 Responsive Breakpoints

| Breakpoint | Layout Changes |
|---|---|
| `> 900px` | Full multi-column layout |
| `≤ 900px` | Single-column about, 2-col programs/trainers/pricing, hidden nav links |
| `≤ 600px` | Single-column programs, trainers, pricing, and footer |

---

## ✏️ Customization

### Change the gym name
Search and replace `Iron Forge` / `IRONFORGE` throughout the file.

### Update colors
Edit the CSS variables at the top of the `<style>` block:
```css
:root {
  --red: #e63329;   /* swap for your brand color */
  --black: #0a0a0a;
}
```

### Swap hero/program images
Images are loaded from [Unsplash](https://unsplash.com). Replace the `src` URLs with your own hosted images:
```html
<div class="hero-image-area" style="background-image: url('your-image.jpg')"></div>
```

### Update pricing
Find the `.price-card` blocks in the Pricing section and edit the plan names, amounts, and feature list items directly.

### Add/remove nav links
Edit the `<ul class="nav-links">` block in the `<nav>` element.

---

## 🌐 Deployment

This is a plain static file — deploy anywhere:

- **GitHub Pages** — push to a repo, enable Pages in settings
- **Netlify** — drag and drop the file at [netlify.com/drop](https://netlify.com/drop)
- **Vercel** — `vercel --prod` from the project folder
- **Any web host** — upload via FTP/SFTP to your public directory

---

## 📦 Dependencies

All loaded via CDN — no local installation required.

| Resource | Source |
|---|---|
| Google Fonts | fonts.googleapis.com |
| Hero & card images | images.unsplash.com |

No JavaScript libraries. No CSS frameworks. No bundler.

---

## 📄 License

Free to use for personal and commercial projects. Attribution appreciated but not required.

---

> Built with pure HTML · CSS · Vanilla JS — no frameworks, no build step.
