# Website Rebuild Prompt — Cornerstone Photography
## For Google AI Studio (Gemini)

---

## CONTEXT BLOCK

### Who You Are Building For
You are rebuilding the website for **Cornerstone Photography** (cornerstonephotography.com.au), an Australian real estate photography business. The client provides professional property photography services to real estate agents and property managers across Australia. This is a small, service-based business — not an enterprise. The website must function as both a portfolio showcase and a lead-generation tool that converts visiting real estate agents into paying clients.

### What the Current Website Offers (Content to Preserve)
The existing website at cornerstonephotography.com.au contains the following pages and content that must be carried across into the new build:

**Homepage:**
- Hero section introducing the business as a provider of residential and commercial photography
- Service overview tiles/cards covering: Interior Photography, Architectural Photography, Drone/Aerial Photography, 2D/3D Floor Plans, Virtual Furniture Staging, and 3D Virtual Tours
- Value proposition: "High quality professional photos that are professionally edited and processed, focusing on every detail to ensure each image is vibrant and crisp"
- Key selling point: Images delivered next business day, ready for uploading to any website
- Decluttering service mention: "We declutter inside and outside to maximise open space"

**Services Page — Full Service List:**
1. **Interior & Architectural Photography** — Professional photos of residential and commercial properties, professionally edited with editing software, vibrant and crisp
2. **Drone/Aerial Photography** — Bird's eye view of properties and their surroundings for prospective buyers
3. **2D/3D Floor Plans** — Showcase dimensions of rooms and property to help clients understand the entire property layout
4. **Virtual Furniture Staging** — Turn empty real estate properties into warm family living spaces; help prospective buyers visualise empty rooms with furniture
5. **3D Virtual Tours** — Immersive walk-through experiences of properties

**Pricing Page:**
- Packages structured by number of images:
  - $150 for 12 images
  - $200 for 20 images
  - $280 for 30 images
  - Up to $375 for premium 30-image packages
  - Video: $400 for 60-second HD video
- All prices inclusive of GST (as of January 2023 — prices subject to change). **NOTE TO AI: Display these prices as provided. Add a visible disclaimer on the pricing page: "Prices shown are indicative. Contact us for current pricing." This protects against outdated pricing.**
- Packages apply to both rental and sale properties

**Gallery/Portfolio Page:**
- Showcase of completed work across all service categories
- Before/after virtual staging examples
- Drone photography samples
- Interior photography samples across residential and commercial

**Contact Page:**
- Contact form for enquiries
- Invitation: "Do not hesitate to contact us should you have any special requirement"
- Location: Australia-based service

### What the New Website Must Achieve
The rebuild is NOT a content change — it is a **complete visual and experiential transformation**. All existing content, services, pricing, and business information must be preserved. The transformation is purely in how it looks, feels, and functions from a UX/UI perspective.

---

## DESIGN REFERENCE: LOGE Camps (logecamps.com)

The new Cornerstone Photography website must adopt the **look, feel, UX patterns, and UI design language** of the LOGE Camps website (logecamps.com/home). Here is a comprehensive breakdown of the LOGE design system that must be translated to the photography context:

### Visual Identity & Aesthetic
LOGE's design is a **retro-modern aesthetic** — inspired by 1970s surf, climbing, and camping culture blended with contemporary digital design. Key characteristics:

- **Warm, earthy colour palette**: Rich wood tones, teal/deep green accents, warm amber/gold highlights against dark backgrounds. The palette evokes warmth, adventure, and approachability — NOT corporate coldness
- **Dark, immersive backgrounds**: LOGE uses deep, dark sections (near-black or deep charcoal) as the dominant background, allowing full-bleed photography to breathe and glow against moody backdrops
- **Full-bleed, cinematic photography**: Images span edge-to-edge with no visible padding or borders. Hero images are massive, atmospheric, and feel like film stills rather than stock photos
- **Retro-modern typography**: A combination of a distinctive display/serif font for headlines (warm, characterful, slightly vintage feel) paired with a clean sans-serif for body text. Typography is generous in size, especially headlines
- **Textured, layered feel**: Subtle texture overlays, slight grain on images, and layered sections that create depth rather than flat, clinical layouts

### Layout & Structure Patterns
- **Full-width hero section**: Massive hero image or video that fills the viewport on load. Minimal text overlay — just a tagline and a single CTA button. The image does the talking
- **Scroll-driven storytelling**: The page is designed to be scrolled. Each section reveals a new "chapter" — a destination, a service, a value prop. Sections transition with generous whitespace or subtle parallax
- **Card-based content grids**: Services, destinations, or features displayed as image-forward cards with minimal text overlay. Cards have rounded corners, subtle hover animations, and consistent spacing
- **Asymmetric layouts**: Not everything is centred. Some sections use offset images with text beside them. This creates visual energy and avoids monotony
- **Generous whitespace**: Sections breathe. There is no cramming. Padding between sections is dramatic (80-120px+). This creates a premium, unhurried feel
- **Sticky/fixed navigation**: A compact, transparent navbar that sits over the hero image and becomes solid on scroll. Navigation items are minimal — no dropdown menus cluttering the experience

### Navigation & UX Patterns
- **Minimal top navigation**: Logo left, 3-5 primary nav items right, prominent CTA button (e.g., "Book Now") in a contrasting colour
- **Hamburger menu on mobile**: Clean slide-out menu with large touch targets
- **Explore/discovery-driven flow**: The homepage is designed to make visitors want to scroll and explore, not hunt for information. Content is seductive, not just informational
- **Single prominent CTA per section**: Each section has ONE clear action — not three competing buttons. This focuses user attention
- **Smooth scroll behaviour**: Anchor links and scroll animations that feel buttery, not jarring

### Interactive & Motion Design
- **Subtle hover states**: Cards lift with `transform: translateY(-4px)` and `box-shadow` increase over `transition: all 0.3s ease`. Buttons shift background colour over `transition: 0.25s ease`. Portfolio images zoom to `transform: scale(1.05)` within `overflow: hidden` containers over `transition: 0.5s ease`
- **Scroll-triggered animations**: Content fades in or slides up as users scroll into each section using `IntersectionObserver` API. Elements start at `opacity: 0; transform: translateY(30px)` and transition to `opacity: 1; transform: translateY(0)` over `0.6s ease-out` with staggered delays (0ms, 100ms, 200ms) for grouped elements. This is subtle — NOT flashy. Think "gentle reveal" not "PowerPoint transition"
- **Parallax on hero images**: The hero background uses `background-attachment: fixed` (or JS-based parallax for mobile compatibility) so the background image moves at a different speed to the foreground text, creating depth
- **Smooth page transitions**: Use `scroll-behavior: smooth` on the `html` element. All anchor links animate smoothly. Navigation clicks scroll with easing

### Footer Design
- **Rich footer**: Dark background, organised in columns. Includes: navigation links, contact info, social media icons, newsletter signup, and brand tagline. The footer feels like a complete section, not an afterthought
- **Social proof or community element**: LOGE includes community-driven content. For Cornerstone, this translates to testimonials, client logos, or a "trusted by X agents" element

### Mobile Experience
- **Mobile-first responsive**: The design compresses gracefully. Hero images still dominate. Cards stack vertically. Typography scales down but stays generous. Touch targets are large
- **Thumb-friendly navigation**: Bottom-accessible CTAs, large buttons, no tiny links
- **Fast loading**: Optimised images, lazy loading, minimal JavaScript bloat

---

## CRITICAL RULES FOR THE AI

### Code Quality & Architecture
- Generate a complete, production-ready website using **HTML, CSS, and JavaScript** (no frameworks required unless you determine one is necessary for a specific interaction)
- Use **semantic HTML5** elements throughout (header, nav, main, section, article, footer)
- CSS must use **CSS custom properties (variables)** for the colour palette, typography scale, and spacing system so the client can adjust branding later
- All CSS must be **responsive** using a mobile-first approach with media queries at standard breakpoints (480px, 768px, 1024px, 1280px)
- Include **accessibility** best practices: proper alt text placeholders, ARIA labels on interactive elements, sufficient colour contrast ratios (WCAG AA minimum), keyboard navigation support
- Use **placeholder images** from a service like Unsplash (real estate/architecture themed) with clear comments indicating where client photos should be swapped in
- Every image must have **lazy loading** enabled (`loading="lazy"`)

### Design Translation Rules
- The colour palette must be adapted from LOGE's outdoor/adventure palette to suit **real estate photography**. Use these CSS custom properties as your starting point (adjust if needed, but document why):
  ```css
  --color-bg-primary: #1a1a1a;       /* Deep charcoal — primary background */
  --color-bg-secondary: #2a2a2a;     /* Slightly lighter charcoal — section alternates */
  --color-bg-card: #333333;          /* Card backgrounds */
  --color-accent-primary: #c9954c;   /* Warm gold/amber — CTAs, highlights, accent borders */
  --color-accent-secondary: #2d6a6a; /* Deep teal — secondary accent for variety */
  --color-text-primary: #f5f0eb;     /* Warm white — primary text on dark backgrounds */
  --color-text-secondary: #a8a29e;   /* Muted warm grey — secondary/body text */
  --color-text-heading: #ffffff;     /* Pure white — headings for maximum contrast */
  --color-border: rgba(201, 149, 76, 0.2); /* Subtle gold border for cards */
  ```
- Typography must use **Google Fonts** — use these specific pairings:
  - **Headlines**: `'DM Serif Display', serif` — warm, editorial, premium feel (weight 400)
  - **Body text**: `'DM Sans', sans-serif` — clean, modern, highly readable (weights 400, 500, 700)
  - **Accent/labels**: `'DM Sans', sans-serif` at weight 500 with letter-spacing: 0.1em and text-transform: uppercase for service labels and navigation
  - **Type scale** (desktop): Hero headline 4.5rem, Section headings 2.5rem, Sub-headings 1.5rem, Body 1.125rem, Small/captions 0.875rem. Scale down proportionally for mobile (hero to 2.5rem, section headings to 1.75rem)
- Photography treatment: all portfolio images should be displayed with consistent aspect ratios, subtle hover zoom effects, and no visible borders — the LOGE "full-bleed, cinematic" approach
- The overall vibe must communicate: **"premium, professional, modern, warm, trustworthy"** — NOT "budget", "clip-art", or "template"

### Content Mapping (LOGE → Cornerstone)
Translate LOGE's content sections to Cornerstone's business as follows:

| LOGE Section | Cornerstone Equivalent |
|---|---|
| Hero: "The hotel that gets you outdoors" | Hero: Stunning full-bleed property photo with tagline about transforming how properties are presented |
| "Explore All Destinations" grid | "Our Services" grid — 6 service cards (Interior, Architectural, Drone, Floor Plans, Virtual Staging, 3D Tours) |
| Destination detail cards | Service detail cards with sample images and brief descriptions |
| "Plan by Activity" section | "Choose Your Package" section — pricing tiers displayed as elegant cards |
| FAFO (amenities) section | "Why Cornerstone" section — next-day delivery, professional editing, decluttering, GST-inclusive pricing |
| Journal/Stories section | "Our Work" portfolio gallery — filterable by service type |
| Community/About section | "About Cornerstone" — story, mission, the team's commitment to quality |
| Booking CTA | "Get a Quote" or "Book a Shoot" CTA — prominent throughout |
| Footer with newsletter | Footer with contact info, service areas, social links, quick enquiry form |

### What NOT to Do
- Do NOT create a generic real estate photography template. The design must feel like LOGE's website adapted for property photography — immersive, warm, scroll-driven, cinematic
- Do NOT use stock-looking icon sets for services. Use high-quality photography as the primary visual element for every service, with text overlays
- Do NOT create a flat, bright-white corporate website. The dark, moody, warm palette is essential to matching the LOGE feel
- Do NOT over-complicate the navigation. Keep it to: Home, Services, Pricing, Gallery, Contact — plus one CTA button
- Do NOT use popup modals, carousels with tiny dots, or any UX patterns that feel dated. LOGE's UX is modern, clean, and scroll-native
- Do NOT skip the mobile responsive design. The site must look intentionally designed on mobile, not just "squeezed down"
- Do NOT forget micro-interactions: hover states on every interactive element, scroll animations on section entries, smooth transitions on navigation

### Output Format
Deliver the website as follows:

1. **`index.html`** — Complete homepage with all sections, inline critical CSS in `<style>` tags within the head, and JavaScript at the bottom of the body
2. **`services.html`** — Detailed services page with individual sections for each service
3. **`pricing.html`** — Pricing page with the package tiers displayed as comparison cards
4. **`gallery.html`** — Portfolio/gallery page with a filterable masonry or grid layout
5. **`contact.html`** — Contact page with a styled form, map placeholder, and direct contact details
6. **`styles.css`** — Complete stylesheet with CSS custom properties, responsive breakpoints, animations, and all component styles
7. **`script.js`** — JavaScript for: mobile menu toggle, scroll-triggered animations, gallery filtering, smooth scroll, navbar background change on scroll, lazy image loading enhancement

For each file, include comments at the top explaining the file's purpose and any client-specific items that need updating (like placeholder images, phone numbers, email addresses, Google Maps embed codes).

### Handling Uncertainty
- If you are unsure about any specific detail of the Cornerstone Photography business (e.g., exact phone number, exact service area, team member names), use clearly marked placeholders like `[PHONE NUMBER]`, `[SERVICE AREA]`, `[TEAM MEMBER NAME]` and add a comment noting it needs client input
- If you cannot determine the exact LOGE colour hex codes from description alone, choose a cohesive palette that matches the described aesthetic (dark backgrounds, warm accents, clean whites) and document your colour choices in the CSS variables with comments explaining the rationale
- If any section requires content you don't have (e.g., testimonials, client logos), create realistic placeholder content clearly marked as `<!-- PLACEHOLDER: Replace with real testimonials -->`

### Quality Checklist (Self-Evaluate Before Delivering)
Before finalising your output, verify:
- [ ] Every page matches the LOGE aesthetic: dark, warm, immersive, scroll-driven
- [ ] All 6 Cornerstone services are represented with dedicated sections
- [ ] Pricing packages are accurately displayed ($150/12 images through to $400 video)
- [ ] Gallery page has filtering capability by service type
- [ ] Contact form is functional (front-end) with all necessary fields
- [ ] Mobile responsive at all breakpoints — test mentally at 375px, 768px, 1024px, 1440px
- [ ] CSS custom properties defined for: colours, fonts, spacing, border-radius
- [ ] All placeholder images have descriptive alt text and lazy loading
- [ ] Hover states exist on all interactive elements
- [ ] Scroll animations are defined and subtle
- [ ] Navigation is sticky/transparent-to-solid on scroll
- [ ] Footer is rich and complete
- [ ] Accessibility: ARIA labels, contrast ratios, keyboard nav
- [ ] No broken layout, no overlapping elements, no orphaned text
- [ ] Code is clean, commented, and production-ready

---

---

## IMPORTANT REMINDERS

- **Visit both reference websites BEFORE generating code.** Navigate to cornerstonephotography.com.au to verify current content, and logecamps.com/home to study the live design. If any content on the live site differs from what is described above, prioritise the live site content — it is more current.
- **Do not fabricate any business information.** If you cannot verify something (team names, phone numbers, exact service areas), use a placeholder. Never invent details that could mislead the business owner or their clients.
- **Label every assumption.** If you make a design choice that isn't explicitly specified above (e.g., choosing a specific animation curve, a particular grid column count), add a CSS/HTML comment explaining your reasoning so the client can adjust.
- **Test your output mentally at 375px width** (iPhone SE) before delivering. If any element would overflow, stack incorrectly, or become unreadable at that width, fix it before delivering.

---

*This prompt was built using the Goodside/Weng/Mollick Prompt Engineering Framework.*
