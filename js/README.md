# Simplisite — Simple Websites for Small Businesses

A working marketing + portfolio site for selling **AI-generated, human-edited websites** to small businesses.

The live site is in `index.html` — open it in any browser. It's a self-contained static site (no build step, no backend).

---

## 1. The Concept

**The pitch:** *"AI builds it. I polish it. You get a site that looks like you paid a lot — without paying a lot."*

Everyone who runs a small business (bakery, salon, contractor, clinic, boutique, café) knows they need a website but most can't afford a $5,000 agency build or the week of evenings it takes to DIY it.

The core insight of the business is the **division of labour between AI and human**:

| Step | Who does it | Why |
|------|-------------|-----|
| Structure + first-pass copy | **AI** | Fast, cheap, tailored to the industry, kills the blank-page problem |
| Rewriting, redesign, polish | **You (human)** | Fixes the awkward phrasing and flat layouts AI leaves behind |
| Hosting, domain, launch | **You** | Removes the technical friction entirely for the client |

The selling point is not "AI" and it's not "hand-made" — it's **the combination**: AI speed with human quality control.

### The guardrail
You must be honest about the AI involvement. The differentiation is the *editing* — you are a designer who uses AI as a tool, not a reseller of raw AI output. That's the entire value proposition and the reason clients will pay more than a $10/mo DIY builder.

---

## 2. Target Audience

- **Business type:** local, owner-operated, 1–20 staff
- **Pain point:** has no website, a bad one, or one they can't update
- **Budget:** $100–$1,000 one-off, plus maybe a small monthly retainer
- **Decision-maker:** the owner (needs it simple and fast, not "an agency relationship")
- **Examples:** restaurants, salons, contractors, clinics, boutiques, cafés, studios, trades

---

## 3. The Offer

Four products, each a clear level of buy-in. They ladder from a cheap entry point (template) to a full build (business site) with a recurring upsell (care plan).

| Product | Price | What they get | Delivery |
|---------|-------|---------------|----------|
| **Template Pack** | $79 one-time | A finished template, re-skinned to their brand, set up on their domain | 2–3 days |
| **Starter Site** | $299 one-time | A custom 1-page site, AI-drafted then hand-edited copy, booking/contact form, SEO essentials | 3 days |
| **Business Site** | $699 one-time | Up to 5 pages, full SEO, analytics, gallery, 3 revision rounds | up to 1 week |
| **Care Plan** | $39/month | Hosting, SSL, weekly backups, ~1 hr of edits/month, priority support | ongoing |

### Pricing rationale
- **Anchor low ($79)** so a hesitant small business owner can start and you build trust for the upsell.
- **Center the eye on $299** — the "Most Popular" tier. It's the product most small businesses actually need, and the featured dark card draws the eye there.
- **The $39/mo Care Plan** is the real engine of recurring revenue and the product that turns one-off buyers into subscribers.

### Optional add-ons / upsells
- Rush delivery (+25%)
- Additional page ($50–$100 each)
- Copywriting / content pack (write all the text for them) (+$150)
- Logo or brand refresh (+$100)
- Google Business / local SEO setup (+$80)

---

## 4. Platform: Where to build & sell

There are **two separate platforms** to consider — one for *building the sites you sell*, one for *selling/processing payments*.

### For building the sites you deliver
| Platform | Best for | Notes |
|----------|----------|-------|
| **Framer** | Fastest for AI-assisted design; gorgeous defaults | Great if you want to iterate quickly and hand off a link. |
| **Webflow** | Most business-grade; client editing, CMS, strong SEO | Best if you want clients to self-edit and you need e-commerce. |
| **Squarespace** | Easiest for non-tech clients | Fine, but less "designer" control than Framer/Webflow. |
| **Custom (React/Vite)** | Full control, zero platform fees | What this demo site is built on. More work to maintain. |
| **AI + code (v0, Lovable, etc.)** | Speeds up your own build process | Use as a tool *for you*, not as the deliverable platform. |

**My recommendation:** Build the client sites in **Framer or Webflow**. They are fast, polish-friendly, and (importantly) let you hand the client a link and an editable canvas — which reinforces the "you own it, you can edit it" promise. Host client projects there and charge a monthly Care Plan for hosting and edits.

### For selling & taking payment
| Platform | Best for | Fees |
|----------|----------|------|
| **Gumroad** | Selling standalone templates as digital products | ~10% per sale |
| **Lemon Squeezy** | Same as Gumroad but handles VAT/global tax for you | ~5% + $0.50 |
| **Stripe Payment Links / Checkout** | Direct, clean, low fee | ~2.9% + $0.30 |
| **Webflow E-commerce** | Only if you're fully in Webflow | platform pricing |

**For templates (digital downloads):** **Gumroad** or **Lemon Squeezy** — they handle delivery, and Lemon Squeezy handles global sales tax/VAT automatically, which is a huge time-saver for a solo seller.

**For custom builds:** Just invoice via **Stripe** (or Stripe Payment Links). Keep it simple — a quote, a 50% deposit, payment link, done.

### For hosting the Simplisite site itself (this demo)
This is a static site, so deploy it for free on:
- **Vercel** (easiest, auto-serves from a Git repo)
- **Netlify** (drag-and-drop or Git)
- **GitHub Pages** (free, but needs a repo)
- Or hand this exact HTML/CSS to **Framer/Webflow** if you'd rather edit visually later.

---

## 5. What's on the site (what I built)

A single-page marketing site with the editorial design system. Sections:

1. **Nav** — logo, links, sticky CTA, mobile hamburger menu
2. **Hero** — headline, value prop, stats, animated browser mockup
3. **Trust strip** — "Built for the businesses that run your town"
4. **How It Works** — 4-step AI + human process
5. **The Work** — 4 template cards with mockups (Bakery, Salon, Contractor, Clinic)
6. **Pricing** — 4 tiers, "Starter Site" featured
7. **Testimonials** — 3 social-proof quotes
8. **FAQ** — accordion (native `<details>`)
9. **Contact** — form that composes a mailto (no backend required)
10. **Footer** — brand, links, copyright year auto-generated

### Design notes
- **Style:** Editorial — warm off-white, deep forest green, terracotta accent, serif display (Fraunces) + clean sans (Inter)
- **Fully responsive** (breakpoints at 980px, 720px, 480px)
- **Icons** throughout are inline SVG (no emoji)
- **Accessible:** semantic headings, ARIA labels, keyboard-friendly accordion

### Files
```
simplisite/
├── index.html          # Full single-page site
├── css/styles.css      # Editorial design system
├── js/main.js          # Nav toggle, form validation + mailto, footer year
├── assets/favicon.svg  # Logo mark
└── README.md           # This document
```

---

## 6. Next steps to launch

1. **Replace the placeholder email** `hello@simplisite.studio` with your real one (in `index.html` contact section and `js/main.js`).
2. **Swap in real template images/screenshots** in the Work section if you have them (the current mockups are CSS skeletons).
3. **Connect a checkout** — add Gumroad/Lemon Squeezy links to the template buttons, or a Stripe Payment Link per pricing tier.
4. **Deploy** to Vercel/Netlify, or migrate the design into Framer/Webflow.
5. **Add your own name/"About"** — the testimonials and voice are placeholders; write them in your own words.
