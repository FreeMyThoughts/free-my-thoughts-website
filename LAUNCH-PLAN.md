# Free My Thoughts — Launch Plan (v2)

Updated now that we know the previous site exists at **freemythoughts.co.uk** (built in Webflow). Marie already has: the domain, `marie@freemythoughts.co.uk` email, a Calendly account, an Instagram (@mariefreemythoughtscoaching), Google Analytics (G-6ZYSHTFJ76) and a Google Search Console verification.

---

## 1. Hosting — moving off Webflow saves real money

Webflow site hosting costs roughly **£12–20/month (~£150–240/year)**. This new site is plain HTML/CSS and can be hosted **free**, so the only remaining cost is the domain renewal (~£10/year). **Net saving: ~£150–230/year.**

### Migration steps (do in this order)
1. **Find out where the domain is registered** and where email (MX records) is hosted — log into the domain registrar and check the DNS settings. ⚠️ **Do not change MX records** during migration or marie@ email will break.
2. **Create a free Cloudflare account**, add the freemythoughts.co.uk domain (Cloudflare copies existing DNS records automatically — verify MX records copied correctly).
3. **Deploy the site to Cloudflare Pages** (drag-and-drop upload of this folder, or connect a free GitHub repository for easy future updates).
4. **Point the domain** at the Pages site in the same dashboard. HTTPS is automatic and free.
5. **Test email still works**, then cancel the Webflow site plan.
- Equally good free alternatives: Netlify, GitHub Pages, Vercel.

### Email — £0 change needed
`marie@freemythoughts.co.uk` already exists. Just confirm which provider hosts it (step 1 above) and leave those DNS records alone. Nothing else to do.

### Contact form (one-time, free)
The old Webflow form will stop working off Webflow. Sign up at **formspree.io** (free, 50 submissions/month), create a form, and replace `YOUR_FORM_ID` in [get-in-touch.html](get-in-touch.html). Alternatives: Web3Forms, Tally.
- reCAPTCHA from the old form is no longer needed — Formspree includes spam filtering.

### Booking — already sorted
Calendly (calendly.com/marie-freemythoughts/freemythoughts) is already linked from every call-to-action button on the new site.

**Total running cost after migration: ~£10/year (domain renewal only).**

---

## 2. What the new site improves over the old one

- **Old bugs fixed**: Facebook icon linked to a yoga studio page (YOGAINBATH); the life-coaching page contained a leftover yoga booking slider and a `solpoweryoga.co.uk` contact email; testimonial sections rendered "No items found"; the disclaimer referenced "freemythoughts.com" (wrong domain).
- **Much faster**: no Webflow/jQuery/webfont-loader JavaScript, no cookie-consent scripts needed (see below), compressed single-size images.
- **Clearer copy**: the long question-lists are condensed into scannable cards; key info (pricing, process, contact) is easier to find.
- **Same URLs kept** (`/life-coaching`, `/for-business`, `/pricing`, `/meet-marie`, `/get-in-touch`) so existing Google rankings and links carry over.
- **Structured data** (schema.org ProfessionalService) added for local SEO.

### ⚠️ Decisions for Marie to review
- **Legal pages**: I rewrote the Terms and Privacy pages to remove irrelevant US-template clauses (California rights, "Marketplace Offerings", arbitration in Strasbourg, ad-network clauses). They are cleaner and UK-focused, **but they are not legal advice — Marie should read them and ideally have them checked**, and set the "Last updated" dates.
- **Analytics & cookies**: the old site used Google Analytics + a cookie consent banner. The new site currently has **no analytics and needs no cookie banner**. If Marie wants visitor stats, add **Cloudflare Web Analytics or Plausible** (privacy-friendly, no cookies, no banner needed) rather than re-adding Google Analytics.
- **Old pages dropped**: coming-soon, 401, and the empty detail_ pages weren't worth keeping. A custom 404 page can be added on request.
- **"Depression"/"Addiction" areas**: kept from the old site but reworded slightly with a clear signpost to GP/Samaritans, since coaching marketing around clinical-sounding areas needs care.

---

## 3. SEO strategy

The niche is local + specific: own searches like "life coach Bristol", "business coach Bristol", "NLP coach Bristol".

### Already done in the new site
- Bristol-targeted titles and meta descriptions on every page
- Schema.org structured data with real contact details
- One page per topic, semantic headings, fast Core Web Vitals
- Old URL slugs preserved

### To do at/after launch
1. **Google Business Profile** (free — the single highest-impact action). Register at business.google.com as a service-area business in Bristol. This puts Marie on Google Maps and in local results.
2. **Google Search Console** — the site verification meta tag from the old site can be re-added if needed; submit a sitemap.xml (create once live).
3. **Reviews**: after every successful engagement, ask clients for a Google review. 10+ reviews beats almost any other local SEO tactic. The three site testimonials (Emma, Jacob, Daniel) are a good start — Google reviews carry more weight.
4. **One blog post a month** targeting real questions: "Coaching vs therapy — which do I need?", "How NLP coaching works", "Overcoming imposter syndrome at work". Share each on Instagram/LinkedIn.
5. **Local citations**: Life Coach Directory, Bark, EMCC/ICF directories (if accredited), Bristol Life, Bristol Creative Industries, chamber of commerce. Keep name/address/phone identical everywhere.

---

## 4. Outreach strategy (first 90 days)

### Weeks 1–2: Foundations
- Announce the relaunched site on Instagram and to the personal network — referrals are the #1 source of coaching clients.
- Set up **LinkedIn** properly (business coaching clients live there, not Instagram): headline "Life & Business Coach | Bristol", link to the site, republish the best testimonials.
- Ask past clients (Emma, Jacob, Daniel and others) for **Google reviews** once the Business Profile is live.

### Weeks 3–6: Local presence
- **Partnerships**: introduce the practice to complementary Bristol businesses — therapists, HR consultants, co-working spaces (Origin Workspace, Runway East, Desklodge), gyms/yoga studios. Offer a free taster workshop or referral arrangement.
- The **business coaching packages** (£1,600–£6,200) are where the revenue is: identify 20 Bristol SMEs/charities that fit, and send a short, personal outreach note offering a free consultation. Marie's charity-sector background is a genuine differentiator — lead with it.

### Weeks 7–12: Authority building
- **Free workshop** ("Free your thinking: a 45-minute reset for busy professionals") at a co-working space — collects warm leads.
- **LinkedIn rhythm**: 2 posts/week (one coaching insight, one story), 15 minutes/day of genuine commenting.
- **Email list** (MailerLite free tier): monthly "one idea to free your thoughts" note.

### Don't spend money on
- Paid ads before reviews are in place; premium directory listings; rebranding. The swallow brand is distinctive — keep it.

---

## 5. Pre-launch checklist

- [ ] Marie reviews all copy — especially [pricing.html](pricing.html), the reworded coaching-area cards on [life-coaching.html](life-coaching.html), and the legal pages
- [ ] Set real "Last updated" dates on Terms & Privacy
- [ ] Create Formspree form and paste ID into [get-in-touch.html](get-in-touch.html)
- [ ] Confirm domain registrar + email host; migrate DNS carefully (keep MX)
- [ ] Deploy to Cloudflare Pages, connect domain, test on mobile
- [ ] Test: Calendly links, email links, phone link, Instagram link, form submission
- [ ] Google Business Profile + Search Console + sitemap.xml
- [ ] Cancel Webflow subscription (only after the new site is live and tested!)
