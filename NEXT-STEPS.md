# Brand + Website Build: Next Steps Process

## Repeatable workflow. Goal: 3 clients per week.

---

## Where We Are

The client has received brand directions and is picking their favorite. Once they confirm a direction, this is what happens next.

---

## Phase 1: Direction Lock + Logo Delivery

**Trigger:** Client picks a direction.
**Time:** 15 min

1. Move unchosen directions to `archives/`
2. Lock the brand DNA document (`brand-dna.md`) with final colors, fonts, voice, personality
3. Deliver logo assets:
   - Wordmark (SVG + PNG, light and dark backgrounds)
   - Favicon (SVG + ICO, 32x32 and 180x180)
   - Monogram/mark (if applicable)
   - Social avatar (circle crop, 400x400)
4. Confirm with client: "Your brand is locked. Moving to website."

---

## Phase 2: Competitive Research + SEO Strategy

**Time:** 1-2 hours (Claude Code does the heavy lifting)
**Reference:** [BuilderGrowth SEO Playbook, Phase 0](https://docs.google.com/document/d/1IbHuyCKnjPr9AxCm2YXGeCKsxWg3fHvPAX5aRwwCUAE/edit)

Run the SEO Playbook's Phase 0 (Building from Scratch) in Claude Code:

1. **Competitive Audit:** Top 8-10 competitors in the client's market. Site architecture, schema usage, content strategy, page counts, local SEO signals. Saved as `COMPETITOR-AUDIT.md`.

2. **Keyword Strategy:** Full keyword universe organized by money keywords, service keywords, local/neighborhood keywords, informational keywords. Saved as `KEYWORD-STRATEGY.md`.

3. **Site Architecture Blueprint:** Every page the site needs at launch with URL paths, keyword targets, schema types, internal linking strategy. Saved as `SITE-ARCHITECTURE.md`.

4. **Design + SEO Spec:** Above-the-fold requirements, page layout rules per page type, mobile-first specs, speed targets. Saved as `DESIGN-SEO-SPEC.md`.

This phase answers: what pages do we build, what keywords do we target, and how do we beat every competitor from day one.

---

## Phase 3: Two Website Directions (Lorem Copy)

**Time:** 1.5-2 hours
**This is the key deliverable the client sees next.**

Build 2 website directions as full HTML/CSS sites. Each direction uses the locked brand (colors, fonts, wordmark) but presents a different layout, structure, and feel.

### What each direction includes:
- Homepage (hero, services overview, about teaser, CTA, footer)
- 1 sample interior page (service page or about page)
- Navigation structure
- Mobile responsive
- All lorem ipsum / placeholder copy (no real content yet)
- Photo placeholders or client-provided photos

### Why two directions:
- Lets the client react to layout and structure without getting stuck on words
- Separates the "does this feel right" decision from the "is this copy right" decision
- Faster than building one perfect thing. Build two rough things, let the client pick.

### What differs between directions:
- Hero layout (full-bleed photo vs split, centered vs left-aligned)
- Navigation style (sticky top bar vs hamburger vs sidebar)
- Page rhythm (long scroll vs chunked sections)
- CTA placement and style
- Photo treatment (full-bleed vs contained, overlapping vs grid)

### What stays the same:
- Brand colors, fonts, wordmark (locked in Phase 1)
- Content structure from SEO spec (H1 placement, 50-word summary, FAQ sections, breadcrumbs)
- Schema markup (all SEO infrastructure baked into both directions)
- Mobile responsiveness

Deploy both to Vercel as separate URLs. Send to client with a walkthrough email.

---

## Phase 4: Client Approves Direction

**Trigger:** Client picks a website direction.
**Time:** 0 (waiting on client)

Operations lead follows up within 3 days if no response. Once approved:
- Archive the unchosen direction
- The chosen direction becomes the working build

---

## Phase 5: Real Copy + Brand Voice

**Time:** 1-1.5 hours

Using the locked brand DNA and the brand guide copy from the original brand directions:

1. Write all page copy in the client's brand voice
2. Apply the 50-word definitive answer rule on every service/landing page (from SEO Playbook)
3. Write all FAQ sections with real questions (informed by keyword strategy)
4. Write all meta titles and descriptions (unique per page)
5. Write CTA copy, navigation labels, footer content

Send the copy to the client for review. This is a separate approval from the design direction. Copy approval can happen async via Google Doc or directly in the site.

---

## Phase 6: Final Build + SEO Infrastructure

**Time:** 1-2 hours

Once copy is approved, execute the SEO Playbook Phases 1-3:

1. **Phase 1 (Foundation):** Meta tags, canonical URLs, Open Graph, schema markup (LocalBusiness, Breadcrumb, FAQ), sitemap.xml, robots.txt

2. **Phase 2 (Local SEO):** Neighborhood/location pages if applicable, SPA crawl fixes, competitive gap pages

3. **Phase 3 (Entity Dominance):** Most specific schema type, Person schema for the business owner, Service schema, programmatic service x location pages, internal linking, keyword scorecard

---

## Phase 7: Deploy + Handoff

**Time:** 30 min

1. Final build test (zero errors)
2. Schema validation on 5 representative pages
3. Deploy to production (Vercel or client's hosting)
4. Connect custom domain
5. Submit sitemap to Google Search Console
6. Send client a "your site is live" email with:
   - Live URL
   - Google Search Console access (if they want it)
   - Keyword scorecard
   - What to expect over the next 2-4 weeks

---

## Phase 8: Retainer Kickoff (if applicable)

If the client is on a monthly retainer ($500-2,000/mo), the ongoing work includes:

- Content publishing (blog posts, service pages) per SEO Playbook Phase 4
- Google Business Profile optimization
- Review generation system setup
- Directory submissions
- Monthly keyword ranking updates
- Quarterly page refreshes

---

## Total Timeline Per Client

| Phase | Time | Who |
|-------|------|-----|
| 1. Direction lock + logo | 15 min | Brand lead |
| 2. Competitive research + SEO strategy | 1-2 hours | Brand lead (Claude Code) |
| 3. Two website directions (lorem) | 1.5-2 hours | Brand lead (Claude Code) |
| 4. Client approves direction | 1-3 days (async) | Operations lead follows up |
| 5. Real copy + brand voice | 1-1.5 hours | Brand lead (Claude Code) |
| 6. Final build + SEO infrastructure | 1-2 hours | Brand lead (Claude Code) |
| 7. Deploy + handoff | 30 min | Brand lead |
| **Total build time** | **~6-8 hours** | |
| **Total calendar time** | **~1-2 weeks** | (includes client approval waits) |

---

## 3 Per Week Math

If each client takes ~6-8 hours of build time spread across 1-2 weeks:

- **Week 1 clients:** Start 3 new clients (brand directions intake + build)
- **Week 2:** Those 3 clients are in approval/copy phase. Start 3 new intakes.
- **Steady state:** 3 in build, 3 in approval, 3 in copy/deploy at any given time

The bottleneck is never the build (Claude Code handles that). The bottleneck is client response time between phases. Operations lead keeps the queue moving.

### Weekly capacity (brand lead):
- Monday: 2 brand direction intakes (2.5 hrs each = 5 hrs)
- Tuesday: 1 brand direction intake + 1 competitive research (2.5 + 2 = 4.5 hrs)
- Wednesday: 2 website direction builds (2 hrs each = 4 hrs)
- Thursday: 2 copy + SEO builds (2 hrs each = 4 hrs)
- Friday: Deploys, handoffs, retainer work

### Weekly capacity (operations lead):
- Scheduling intakes
- Following up on direction picks (3-day rule)
- Following up on copy approvals
- Logging projects in scoreboard
- Sending retainer invoices

---

## File Structure Per Client

```
~/Projects/[client-name]/
├── client-profile.md
├── brand-dna.md
├── landing-page-copy.md
├── COMPETITOR-AUDIT.md
├── KEYWORD-STRATEGY.md
├── SITE-ARCHITECTURE.md
├── DESIGN-SEO-SPEC.md
├── KEYWORD-SCORECARD.csv
├── lens-research/
│   ├── [creative-lens]-research.md
│   └── [strategy-lens]-research.md
├── drafts/
│   ├── brand-direction-A-[name].html
│   ├── brand-direction-B-[name].html
│   ├── brand-direction-C-[name].html
│   ├── brand-directions-presentation.html
│   ├── website-direction-A.html
│   ├── website-direction-B.html
│   └── photos/
├── site/                              (final production build)
│   ├── index.html
│   ├── services/
│   ├── about/
│   ├── neighborhoods/
│   ├── sitemap.xml
│   └── robots.txt
├── archives/
└── index.html
```

---

## Skills Used (in order)

1. `/onboard-client` — Client intake, generates profile + lens research
2. `/brand-development` — Brand directions, presentation deck, brand DNA
3. SEO Playbook Phase 0 prompt — Competitive research, keyword strategy, site architecture
4. `/landing-page` or `/copywriting` — Website copy in brand voice
5. SEO Playbook Phases 1-3 prompts — Technical SEO build
6. Manual deploy — Git, GitHub, Vercel, domain connection

---

*This is the full Brand + Website + SEO pipeline. Every client gets the same process. Every output is custom. The system scales because the skills do the work.*

*Last updated: March 4, 2026*
