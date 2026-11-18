# Project case study evidence contract

**Status:** editorial specification for the planned site, not evidence that any projects have been published.
**Scope:** project-detail pages and project cards proposed in [PROJECT_AND_DESIGN_BRIEF.md](./PROJECT_AND_DESIGN_BRIEF.md).

## Why this exists

Architecture portfolios depend on accurate project metadata, image permissions, and credible descriptions of what a studio actually delivered. A striking render alone does not substantiate construction status, authorship, measurable outcomes, or a client testimonial. This contract gives writers, designers, developers, and reviewers a single acceptance standard **before** a case study enters a future CMS or site.

## Required content record

| Field | Type / example | Publication rule |
| --- | --- | --- |
| `slug` | Stable lowercase URL segment | Unique; redirect if renamed after publishing |
| `title` | Project's approved public name | Confirm spelling with project owner |
| `type` | Residential / commercial / interiors / other | Match project scope; do not imply services not provided |
| `location` | Publicly approved city or region | Never publish a private client's exact address without consent |
| `year` | Design year, completion year, or `undisclosed` | Label which year is shown; do not conflate stages |
| `status` | Concept / in design / built / photographed | Show the stage accurately, including unbuilt projects |
| `role` | Studio's actual deliverables | Attribute collaborators and external architects explicitly |
| `brief` | Client objective and context | Remove confidential identifying details |
| `constraints` | Site, budget, material, regulatory, or accessibility factors | Confirm sensitive details are approved |
| `approach` | Decisions and alternatives considered | Explain *why*, not only what the images show |
| `result` | Verified output and observable effect | Distinguish completed work from proposals |
| `media` | Asset, rights holder, photographer, caption, alt text | No asset ships without a rights and attribution check |
| `source` | Internal evidence URL or reference ID | Private source; do not expose protected documents publicly |
| `approved_by` | Owner/editor + review date | Required before publication |

Optional numeric outcomes must record **method, dates, baseline, and source**. If evidence is unavailable, omit the metric rather than inventing one.

## Page composition and behavior

1. **Header:** concise title, type, location granularity, role, and accurately labelled status.
2. **Overview:** objective, audience/client constraints, and scope of work in plain language.
3. **Process:** exploration and choices, with relevant sketches, plans, or iterations where permitted.
4. **Outcome:** delivered work and verified observations; clearly mark renders or proposals.
5. **Gallery:** ordered images with meaningful captions, dimensions or responsive aspect-ratio handling, and photographer/creator credits.
6. **Continuation:** related work, relevant services, and an accessible contact action.

A card must not make claims that disappear or contradict the detail page. Images that convey project details need meaningful alt text; decorative images may use empty alt text. Preserve readable overlay contrast and keyboard-visible gallery controls.

## Media provenance template

Use one entry for every image, video, or drawing:

```text
Asset ID:
Project slug:
Filename / canonical source:
Type (photo / render / drawing / plan):
Creator / copyright owner:
Usage permission, territory, term:
Required credit line:
Approved publication surfaces:
Public caption:
Alt text:
Approval date / reviewer:
```

A render cannot be labelled as a completed building photograph. Preserve a record of crop decisions when they change the apparent design.

## Editorial review and acceptance

- [ ] Names, role, location granularity, year and project stage have owner approval.
- [ ] Every public outcome/award/testimonial can be traced to evidence or has been removed.
- [ ] Every media asset has permission, caption/credit rules and accessible alternatives.
- [ ] Text explains decisions, constraints and result without fabricated client quotations.
- [ ] Mobile reading order, keyboard navigation, reduced-motion preferences and image loading are reviewed.
- [ ] Project card, detail page, social preview and metadata describe the same project.
- [ ] Contact path works and does not disclose private client information.
- [ ] A reviewer records approval date and any restrictions.

## Change control

Treat project naming, status, consent, credits and measurements as **editorial data** requiring reapproval after meaningful changes. If a rights holder withdraws permission, unpublish the asset and purge relevant cached previews; record the replacement or removal. Retain private evidence only in authorized systems, not in the public repository.

## Definition of done

This document is a **planning artifact**. It does not claim the future website, CMS, images, or checks already exist. Implementation is complete only when actual project records use the contract and a reviewer can reproduce the evidence and accessibility checks.
