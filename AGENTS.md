# Repository Instructions

## Current repository state

This repository is a design and planning scaffold for an architecture or interior-design website. It does not currently contain an application, package manifest, build system, deployment, or verified runtime screenshot.

Do not describe the repository as a completed website until real source files and a working deployment exist.

## Start here

Read these files in order:

1. `README.md`
2. `docs/PROJECT_AND_DESIGN_BRIEF.md`
3. `docs/assets/architecture-website-thumbnail.svg`

## Current commands

There are no installation, development, build, test, lint, or deployment commands yet because no application stack has been selected.

Do not invent commands or add placeholder scripts that do not execute real work.

## Implementation rules

When application development begins:

- choose the framework based on content-editing and deployment needs
- add a package manifest and lockfile together
- document the supported Node.js and package-manager versions
- add real lint, type-check, build, and test commands
- keep project content separate from layout components
- use typed project records or validated content collections
- preserve image dimensions, credits, rights, and captions
- keep route metadata centralized
- avoid introducing a CMS until a real editing workflow requires one
- keep contact-form secrets and private credentials server-side

## Product rules

The intended website should:

- prioritize project storytelling over decorative effects
- make services and process understandable
- give every major page a clear contact path
- explain project decisions, not only show galleries
- use real evidence for awards, statistics, locations, and experience
- distinguish concept work from completed client work

Do not publish fabricated projects, invented client outcomes, or unverified studio claims.

## Visual-design rules

- Use generous whitespace deliberately, not as a substitute for hierarchy.
- Keep body text comfortably readable.
- Let project photography carry most of the color.
- Use motion sparingly and support reduced-motion preferences.
- Avoid scroll hijacking, unnecessary parallax, and cursor gimmicks.
- Keep image crops intentional across desktop and mobile.
- Do not add unlicensed architectural photography or drawings.

## Accessibility

Future implementation must include:

- semantic landmarks and heading order
- keyboard-accessible navigation and controls
- visible focus states
- sufficient contrast
- meaningful image alt text and captions
- reduced-motion support
- form labels, errors, and confirmation messages
- zoom and reflow support
- no critical information communicated only through imagery

## Performance

- Use responsive images and modern formats.
- Reserve image dimensions to avoid layout shift.
- Lazy-load media below the fold.
- Avoid autoplay video on mobile without a strong reason.
- Minimize third-party scripts.
- Measure Core Web Vitals after deployment.
- Establish performance budgets before adding heavy animation.

## SEO and content

- Use unique titles and descriptions per route.
- Add canonical URLs, sitemap, and robots policy.
- Add accurate structured data only when supported by real business information.
- Keep project URLs descriptive and stable.
- Avoid thin location pages and keyword-stuffed copy.
- Record image credits and permissions.

## Testing and verification

Once source code exists, every meaningful change should include:

1. dependency installation from the committed lockfile
2. linting
3. type-checking
4. production build
5. unit or content-validation tests
6. keyboard and responsive testing
7. project-page image and metadata review
8. contact-form delivery testing
9. accessibility review
10. production deployment verification
11. real desktop and mobile screenshots

## Documentation rules

- Update the README when the repository state changes.
- Replace planning language only after implementation exists.
- Keep the project brief aligned with the chosen architecture.
- Add real setup instructions once commands exist.
- Clearly label concept thumbnails and generated presentation assets.

## Do not

- Do not claim the repository is deployed when it is not.
- Do not present the concept thumbnail as a browser screenshot.
- Do not invent performance scores, project counts, awards, or conversion metrics.
- Do not add fake package scripts merely to make the repository look active.
- Do not expose private enquiry-form credentials.
- Do not publish client material without rights and permission.
- Do not describe future functionality as implemented.