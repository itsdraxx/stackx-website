# StackX — Professional Web Development at Unbeatable Costs

A modern, premium, conversion-focused SaaS agency website built for **StackX**, a software development company specializing in Web Development, Business Automation, and Advertising Technology solutions.

---

## 🚀 Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | [Next.js 16](https://nextjs.org/) (App Router, TypeScript) |
| Styling | [Tailwind CSS v4](https://tailwindcss.com/) |
| Animations | [Framer Motion](https://www.framer.com/motion/) |
| Icons | [React Icons](https://react-icons.github.io/react-icons/) (Heroicons, Font Awesome) |
| Fonts | [Poppins](https://fonts.google.com/specimen/Poppins) (headings) + [Inter](https://fonts.google.com/specimen/Inter) (body) via `next/font/google` |
| Deployment | Static export / Vercel-ready |

---

## 📁 Project Structure

```
src/
├── app/
│   ├── layout.tsx              # Root layout (fonts, metadata, navbar, footer)
│   ├── globals.css             # Design system (tokens, glassmorphism, animations)
│   ├── page.tsx                # Homepage
│   ├── services/
│   │   ├── layout.tsx          # SEO metadata
│   │   └── page.tsx            # Services page
│   ├── about/
│   │   ├── layout.tsx          # SEO metadata
│   │   └── page.tsx            # About Us page
│   ├── portfolio/
│   │   ├── layout.tsx          # SEO metadata
│   │   ├── page.tsx            # Portfolio grid
│   │   └── communize-vizag/
│   │       └── page.tsx        # Case study detail
│   ├── careers/
│   │   ├── layout.tsx          # SEO metadata
│   │   └── page.tsx            # Careers + application form
│   ├── testimonials/
│   │   ├── layout.tsx          # SEO metadata
│   │   └── page.tsx            # Testimonials grid
│   └── contact/
│       ├── layout.tsx          # SEO metadata
│       └── page.tsx            # Contact / consultation form
├── components/
│   ├── layout/
│   │   ├── Navbar.tsx          # Sticky navbar with blur + mobile menu
│   │   └── Footer.tsx          # Multi-column footer
│   └── ui/
│       └── index.tsx           # Reusable UI primitives
```

---

## 📄 Pages

### 1. Homepage (`/`)
- **Hero Section** — Headline "Professional Web Development at Unbeatable Costs", animated gradient background, floating shapes, two CTA buttons (Get Free Consultation, View Our Work)
- **Animated Stats** — Scroll-triggered counters: 150+ projects, 80+ clients, 99.9% uptime, 40% cost savings
- **Client Logos** — Marquee strip of trusted company names
- **Services Overview** — 3 glassmorphism cards with 3D tilt hover effect (Web Dev, Automation, Ad Tech)
- **Why StackX** — 4 value cards: Professionalism, Enthusiasm, Experience, Cost Efficiency
- **Testimonials Carousel** — Auto-play carousel with manual navigation and dot indicators
- **CTA Banner** — "Ready to Build Something Extraordinary?" with action buttons

### 2. Services (`/services`)
- Three category sections: **Web Development**, **Business Automation**, **Ad Tech Solutions**
- Each category includes:
  - Expandable accordion descriptions (4 sub-services each)
  - Technology stack badges
  - "Starting from" pricing transparency ($3,000 / $2,500 / $5,000)
  - Links to related case studies
  - "Get a Quote" CTA

### 3. About Us (`/about`)
- Company story narrative
- Team stats grid (25+ members, 8+ countries, 5+ years, 98% retention)
- Mission & Vision cards
- Core values section (Innovation, Client-Centric, Transparency, Team Excellence)
- Milestone timeline (2020–2025) with animated vertical line

### 4. Portfolio (`/portfolio`)
- Filterable project grid: All / Web Development / Automation / Ad Tech
- 6 case study cards with project thumbnail, category, description, tech stack, and measurable results
- Featured badge on highlight projects
- Animated layout transitions on filter change

### 5. Communize VIZAG Case Study (`/portfolio/communize-vizag`)
- Problem statement & solution provided
- Technologies used (Next.js, React, TypeScript, Node.js, PostgreSQL, AWS S3, Vercel, Tailwind CSS, Framer Motion)
- Measurable results: 3x engagement, 45% cost savings, 99.9% uptime, 2.1s page load
- Key features delivered checklist
- Client testimonial with star rating
- Project visuals section

### 6. Careers (`/careers`)
- Benefits overview (Remote-First, Growth & Learning, Flexible Hours, Competitive Pay)
- 4 open job listings with expand/collapse:
  - Senior Full-Stack Developer
  - Frontend Developer
  - Python Automation Engineer
  - UI/UX Designer
- Application form with validation:
  - Full Name, Email, Phone, Position, Resume Upload (.pdf, .doc, .docx), Portfolio Link, LinkedIn Profile, Cover Letter
  - Client-side validation with error messages
  - Success confirmation state

### 7. Testimonials (`/testimonials`)
- 8 testimonial cards in responsive 3-column grid
- Each card: client name, company, star rating (1–5), feedback quote, project type badge
- Average rating display (4.9/5 stars)

### 8. Contact (`/contact`)
- Consultation lead form with:
  - Name, Email, Phone, Company
  - Service Interest dropdown (6 options)
  - Project Budget Range dropdown (6 ranges)
  - Project Description textarea
  - Preferred Timeline
  - reCAPTCHA checkbox verification
  - Client-side validation with error/success states
- Contact info sidebar (email, phone, location, social links)
- Response time guarantee (2 business hours)

---

## 🎨 Design System

### Color Palette
| Token | Hex | Usage |
|-------|-----|-------|
| `primary` | `#8B5CF6` | Primary purple |
| `primary-light` | `#A78BFA` | Light purple accents |
| `primary-deep` | `#6D28D9` | Deep purple gradients |
| `accent` | `#06B6D4` | Cyan accent |
| `background` | `#0A0A0F` | Dark background |
| `surface` | `#13131A` | Card/section backgrounds |
| `foreground` | `#EDEDED` | Primary text |
| `muted` | `#9CA3AF` | Secondary text |

### UI Effects
- **Glassmorphism** — Semi-transparent cards with backdrop-blur and subtle borders
- **Gradient borders** — CSS mask-based gradient border technique
- **Gradient text** — Purple-to-cyan gradient text for highlights
- **3D tilt cards** — `rotateX`/`rotateY` hover transforms on service cards
- **Floating shapes** — CSS animated decorative shapes in hero sections
- **Marquee** — Infinite scroll logo strip
- **Animated counters** — Scroll-triggered count-up animation using `requestAnimationFrame`
- **Scroll reveal** — Framer Motion `whileInView` viewport-triggered animations
- **Pulse glow** — Subtle box-shadow animation on primary CTA

### Responsive Breakpoints
- **Mobile**: 375px+ (single column, hamburger menu)
- **Tablet**: 640px+ / 768px+ (2-column grids)
- **Desktop**: 1024px+ (full layout, side-by-side sections)
- **Wide**: 1280px+ (max-width container)

---

## 🧩 Reusable Components

| Component | Description |
|-----------|-------------|
| `SectionHeading` | Badge + title + subtitle with scroll animation |
| `GlassCard` | Glassmorphism card with optional hover effect |
| `Button` | 3 variants: `primary` (gradient), `secondary` (subtle), `outline` |
| `AnimatedCounter` | Scroll-triggered count-up with configurable duration |
| `TestimonialCard` | Star rating, quote, client info, project type badge |
| `Navbar` | Sticky with backdrop-blur, mobile hamburger menu (Framer Motion) |
| `Footer` | Multi-column with nav links, contact info, social icons |

---

## 🔧 Getting Started

### Prerequisites
- Node.js 18+
- npm

### Installation
```bash
npm install
```

### Development
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000)

### Production Build
```bash
npm run build
```

### Lint
```bash
npm run lint
```

---

## 📊 SEO

- Page-level `<title>` and `<meta description>` for every route via Next.js Metadata API
- OpenGraph tags on root layout
- Semantic HTML5 structure (`<nav>`, `<main>`, `<section>`, `<footer>`)
- Single `<h1>` per page with proper heading hierarchy
- Descriptive alt text and ARIA labels on interactive elements
- `next/font` for zero-layout-shift font loading

---

## ♿ Accessibility

- Focus-visible outlines on all interactive elements
- ARIA labels on icon-only buttons (menu toggle, social links, carousel controls)
- Semantic heading hierarchy (h1 → h2 → h3)
- Color contrast ratios meet WCAG 2.1 AA standards
- Keyboard navigable throughout

---

## ⚠️ Notes

- **Forms are frontend-only** — The contact and career forms perform client-side validation and show success/error states, but submissions are not connected to a backend API, database, or email service yet. To make them functional, you'll need to add Next.js API routes with an email service (e.g., Resend, SendGrid) or a form backend (e.g., Formspree).
- **reCAPTCHA** — Currently implemented as a checkbox placeholder. Replace with Google reCAPTCHA v2/v3 for production.
- **Client logos** — Text-based placeholders. Replace with actual SVG/PNG logos.
- **Project thumbnails** — Gradient placeholders. Replace with real screenshots or mockups.

---

## 📜 License

© 2025 StackX. All rights reserved.
