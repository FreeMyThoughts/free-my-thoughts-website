# Free My Thoughts — website project

Website for **Free My Thoughts**, the coaching practice of **Marie Stoner**, Bristol (freemythoughts.co.uk). Static HTML/CSS, no build step, designed for free hosting (Cloudflare Pages or similar).

## Business context
- Marie is a life & business coach in Bristol; works UK & Europe, online and in person.
- **Positioning (current)**: premium, targeted at personal & professional growth. **Signature focus: imposter syndrome and breaking through professional blocks.** Avoid presenting a long menu of problem areas — the offer is deliberately narrow: Personal Coaching + Business & Executive Coaching.
- Method language she uses: NLP (Neuro-Linguistic Programming), mindfulness, somatic/ontological coaching, "internal work creates external change", working "at identity level". Brand symbol: the swallow (new life, fresh starts, renewal, growth). Brand phrase: "free your thinking / free my thoughts".
- Real details in use: marie@freemythoughts.co.uk · 07932 675 945 · Instagram @mariefreemythoughtscoaching · Calendly: calendly.com/marie-freemythoughts/freemythoughts
- Pricing: complimentary 30-min discovery consultation; personal coaching £60/50-min (min 6 sessions); combined life+business from £90/60-min; business engagements from £1,600/£1,700/£1,800 and £6,200 (6-month "shoulder-to-shoulder"). Charity/voluntary sector tailored.
- Testimonials in use: Emma, Jacob, Daniel (from the previous site).

## History
- v1: generic placeholder site built from a brief.
- v2: rebuilt using content from Marie's previous Webflow site (an export lives in `C:\Users\marie\OneDrive\website\` — photos, old copy, legal pages). Old URL slugs kept for SEO: `/life-coaching`, `/for-business`, `/pricing`, `/meet-marie`, `/get-in-touch`.
- v3 (current): premium redesign + repositioning around imposter syndrome / professional blocks. Nav labels: Personal Coaching, Business Coaching, Investment, Meet Marie, Book a Consultation.

## Design system (styles.css)
- Palette: deep forest green `#1f3a33` / `#2c524a`, ivory `#faf8f3`, bronze accent `#a07c48`, hairline borders `#e6e0d3`.
- Type: Fraunces (headings, serif) + Inter (body) via Google Fonts. Uppercase letter-spaced eyebrows/buttons/kickers. No emoji icons — use `.kicker` labels on cards.
- Components: `.focus-band` (dark signature section), `.quote-band`, `.testimonial` (serif quotes with bronze “ mark), `.steps` (01/02/03 numbered), `.card` (bronze top border), `.area-grid`.

## Files
- Pages: index, life-coaching, for-business, pricing, meet-marie, get-in-touch, terms-and-conditions, privacy, disclaimer (all .html)
- `images/` — Marie's photos (renamed marie-*.jpg), swallow.png logo, favicon
- `LAUNCH-PLAN.md` — hosting migration (Webflow → Cloudflare Pages, saves ~£150-230/yr), SEO strategy, 90-day outreach plan, pre-launch checklist

## Outstanding / decisions pending
- Contact form needs a Formspree form ID in `get-in-touch.html` (search `YOUR_FORM_ID`).
- Legal pages reviewed with Marie (July 2026): sole trader identity added, bank-transfer payment, 48-hour cancellation + 14-day cooling-off, no-cookies privacy policy naming Calendly/Formspree, 6-year financial record retention, US waiver legalese replaced with plain UK disclaimer. Dates set to 19 July 2026. Still open: Marie to check ICO data protection fee applies (ico.org.uk self-assessment); consider a signed client coaching agreement.
- No analytics currently; if wanted, use Cloudflare Web Analytics or Plausible (cookie-free, no banner needed).
- sitemap.xml + robots.txt to create at deploy time; custom 404 page optional.
- Domain/DNS: keep MX records untouched during migration (marie@ email must not break). Cancel Webflow only after new site is live and tested.

## Conventions
- Plain HTML/CSS only — no frameworks, no build step. Header/footer are duplicated per page; keep them in sync when editing nav.
- Keep existing URL slugs. British English. Tone: assured, warm, unhurried — premium but human; no hype, no exclamation-mark salesiness.
