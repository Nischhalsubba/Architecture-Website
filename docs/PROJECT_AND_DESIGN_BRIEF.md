# Architecture Website — Project and Design Brief

> A product, content, UX, visual-design, technical-planning, accessibility, SEO, and launch brief for turning this repository into a real architecture or interior-design website.

## 1. Current state

This repository is currently a planning scaffold. It contains documentation and a concept thumbnail, but no application source, package manifest, build configuration, automated tests, or deployment.

That status is intentional and should remain visible until implementation begins.

## 2. Product objective

Create a premium architecture-studio website that communicates:

- design quality
- project credibility
- sector expertise
- process clarity
- studio personality
- confidence to enquire

The website should function as both a portfolio and a lead-generation surface without turning every page into a sales brochure wearing black-and-white photography.

## 3. Target users

### Primary

- prospective residential clients
- commercial clients
- developers and property owners
- collaborators and consultants
- design-conscious visitors evaluating the studio

### Secondary

- future hires
- press and award reviewers
- students and researchers
- suppliers and project partners

## 4. Core user journeys

### Explore projects

1. Land on the homepage.
2. Understand the studio positioning.
3. Browse selected work.
4. Open a project detail page.
5. Review scope, constraints, process, and outcome.
6. Continue to a related project or contact path.

### Evaluate the studio

1. Read the studio philosophy.
2. Review sectors and services.
3. Understand the process.
4. See team credibility and selected recognition.
5. Contact the studio.

### Make an enquiry

1. Reach the contact section from any major page.
2. Understand what information is useful.
3. Submit project type, location, stage, budget range, and timeline.
4. Receive a clear confirmation and response expectation.

## 5. Recommended information architecture

```text
/
├── /projects
│   └── /projects/[slug]
├── /studio
├── /services
├── /process
├── /journal
│   └── /journal/[slug]
├── /contact
├── /privacy
└── /404
```

A smaller first release may combine studio, services, and process into the homepage while preserving dedicated project pages.

## 6. Homepage structure

1. **Header**
   - restrained wordmark
   - Projects, Studio, Services, Journal, Contact
   - optional location or availability note

2. **Hero**
   - one strong project image or motion sequence
   - concise positioning statement
   - selected-project or enquiry link

3. **Selected projects**
   - three to six projects
   - location, type, year, status
   - avoid decorative cards that obscure the images

4. **Studio statement**
   - one clear paragraph
   - avoid generic claims such as “we create timeless spaces” unless supported by real evidence

5. **Services or sectors**
   - architecture
   - interiors
   - master planning
   - renovation
   - consultation

6. **Process**
   - discovery
   - concept
   - design development
   - documentation
   - delivery

7. **Recognition or proof**
   - awards
   - publications
   - years of experience
   - completed projects
   - client references

8. **Contact CTA**
   - clear invitation
   - expected response time
   - location and working regions

## 7. Project detail template

Each project page should include:

- project title
- location
- year
- status
- type or sector
- area when appropriate
- services delivered
- client or confidentiality note
- concise challenge
- design response
- material or spatial strategy
- image sequence with captions
- plans, sections, or diagrams where licensed
- project team and collaborators
- related projects

A project page should explain decisions, not merely display twelve photographs and expect visitors to infer the thinking through telepathy.

## 8. Content model

### Project

```text
slug
title
summary
location
year
status
sector
services
area
client_name_or_confidentiality
hero_image
image_gallery
challenge
approach
outcome
materials
team
collaborators
featured
seo_title
seo_description
```

### Journal entry

```text
slug
title
summary
published_at
author
cover_image
body
tags
seo_title
seo_description
```

### Team member

```text
name
role
biography
portrait
credentials
social_links
```

## 9. Visual direction

### Tone

- editorial
- calm
- precise
- tactile
- image-led
- contemporary without chasing fashion

### Typography

Use a deliberate pairing such as:

- editorial serif for display with neutral sans-serif for body
- high-quality grotesk throughout
- restrained mono only for project metadata

Typography should remain readable before it becomes “architectural.” Tiny uppercase labels are not sophistication if nobody can read them.

### Color

Recommended base:

- warm off-white
- charcoal or near-black
- concrete grey
- one restrained material-inspired accent

Project photography should carry most of the color.

### Layout

- generous whitespace
- wide image frames
- asymmetric editorial moments
- stable reading widths
- clear project metadata
- responsive image crops

### Motion

- subtle image reveals
- calm page transitions
- hover states that do not block access
- reduced-motion alternative

Avoid excessive parallax, scroll hijacking, and cursor experiments that turn portfolio review into an obstacle course.

## 10. Image strategy

Architecture websites are image-heavy, so the implementation should support:

- responsive formats
- width and height metadata
- lazy loading below the fold
- high-priority hero image
- blur or neutral placeholders
- art direction for mobile crops
- meaningful alt text
- captions for plans and diagrams
- rights and credit metadata

Do not publish client work, drawings, or photography without permission.

## 11. Accessibility

Minimum requirements:

- semantic headings
- keyboard-accessible navigation
- visible focus states
- sufficient contrast
- descriptive link labels
- alt text that describes spatial content when meaningful
- reduced-motion support
- no information communicated by image alone
- accessible enquiry form errors and confirmation
- zoom and reflow support

Large photographs do not excuse small text.

## 12. Performance

Recommended budgets for the first release:

- initial page JavaScript below 180 KB compressed where practical
- responsive hero image below 350 KB for common desktop delivery
- no autoplay video on mobile without a strong reason
- minimal third-party scripts
- preloaded primary font only when needed
- self-hosted fonts where licensing allows
- Core Web Vitals monitored in production

## 13. SEO

Implement:

- unique metadata per route
- canonical URLs
- sitemap
- robots policy
- Open Graph images
- Organization or LocalBusiness structured data where accurate
- Project or CreativeWork structured data where appropriate
- image alt text and captions
- descriptive project URLs
- location and sector content based on real services

Do not create dozens of thin location pages unless the studio genuinely operates there.

## 14. Recommended implementation

A sensible first implementation:

- Next.js or Astro
- TypeScript
- CSS Modules, Tailwind CSS, or a small token-based CSS system
- local typed content or MDX for the first release
- image optimization built into the framework
- form provider or server action with spam protection
- Vercel, Cloudflare, or Netlify deployment

A CMS becomes useful when non-developers need to add projects or journal entries regularly. It should not be introduced merely because the acronym looks expensive.

## 15. Suggested repository structure

```text
src/
├── app-or-pages/
├── components/
├── content/
│   ├── projects/
│   └── journal/
├── data/
├── lib/
├── styles/
└── types/

public/
├── images/
└── fonts/

docs/
├── PROJECT_AND_DESIGN_BRIEF.md
└── assets/
```

## 16. Testing strategy

### Unit

- content validation
- project sorting and filtering
- metadata helpers
- form validation

### Component

- navigation
- project cards
- image gallery
- enquiry form
- filters if added

### End-to-end

- homepage to project detail
- project navigation
- mobile menu
- contact submission
- keyboard flow
- 404 handling

### Visual

- homepage desktop and mobile
- project detail templates
- long and short titles
- image aspect-ratio variations
- reduced-motion state

## 17. Deployment checklist

- application builds successfully
- production URL resolves
- metadata and canonical URLs are correct
- sitemap and robots files load
- forms deliver successfully
- image credits are accurate
- mobile navigation works
- accessibility review completed
- performance measured
- real browser screenshots captured
- analytics and cookie behavior documented

## 18. Repository statistics

The README should use live GitHub badges for stars, forks, issues, and latest commit activity rather than frozen numbers.

The repository currently contains planning documentation only. Product metrics, page counts, performance scores, and deployment statistics should not be claimed until they exist.

## 19. Roadmap

### Phase 1: Foundation

- choose framework
- add package and lockfile
- establish tokens and typography
- implement base layout
- add lint, typecheck, and build scripts

### Phase 2: Core pages

- homepage
- project index
- project detail
- studio
- contact

### Phase 3: Content quality

- real project data
- image rights and credits
- process and service content
- SEO metadata

### Phase 4: Reliability

- automated tests
- CI
- accessibility review
- performance budgets

### Phase 5: Launch

- deployment
- verified forms
- analytics
- browser screenshots
- README update with real runtime evidence

## 20. Portfolio framing

A truthful current summary is:

> Defined the product direction, information architecture, visual principles, content model, implementation plan, accessibility requirements, and launch checklist for a premium architecture-studio website concept.

Do not claim that the repository contains a completed website, deployed product, client project, or measured outcome.

## 21. Disclaimer

The repository thumbnail is an original concept presentation asset. It is not a browser screenshot, completed client website, or representation of an existing architecture studio. Any future project imagery must be licensed and credited appropriately.