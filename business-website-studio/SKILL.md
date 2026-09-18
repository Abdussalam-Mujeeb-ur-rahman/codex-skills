---
name: business-website-studio
description: Research, plan, visually explore, implement, and quality-assure a credible business website from an existing site, public business information, supplied materials, or a brief. Use for client website concepts, redesign pitches, complete business sites, industry-specific web design, three-option section exploration, selected-design implementation, responsive QA, SEO planning, or when continuing an existing website project without repeating the full workflow.
---

# Business Website Studio

Run a business website project as an evidence-led design studio. Preserve approved work, use authentic business information, and move from research to visual selection to implementation without treating the site like a generic template.

## Begin Every Run

1. Inspect the workspace, existing site, supplied files, current build, and previous decisions.
2. Determine the current phase: discovery, strategy, visual exploration, implementation, QA, or handoff.
3. Resume from the latest approved state. Do not restart research, replace selected designs, rewrite supplied copy, or redesign completed sections without a reason.
4. State which phase is being handled and what will be produced.
5. If the user requests the complete project, progress through the phases in order. If they request one phase or section, stay within that scope.

## Core Rules

- Treat verified business information and approved decisions as the source of truth.
- Never invent people, credentials, accreditations, reviews, outcomes, fees, phone numbers, addresses, opening hours, company details, or regulatory claims.
- Separate confirmed facts, reasonable design proposals, unresolved inconsistencies, and information that only the client can provide.
- Use authoritative current sources for regulated, legal, financial, medical, corporate-registration, or other material claims.
- Before visual exploration or implementation, explicitly capture the business's reusable visual assets and existing visual system. Inventory the logo variants, photography, illustrations, icons, video, documents, and other supplied or current-site assets; record each source, dimensions/type, permission status, intended use, and replacement need. Extract the observable color palette, typography and available weights, logo treatment, spacing, borders, radii, icon style, image treatment, and recurring UI patterns into `brand-system.md` or `colortheme.md`. Treat inferred or proposed tokens as proposed, not confirmed brand facts.
- Use suitable authorized public or supplied brand assets in concepts and implementation when they support the approved direction; do not replace authentic business assets with generic stock or silently reuse public-site assets without recording the source and rights/permission status.
- Use inspiration to learn patterns, not to copy a layout, brand, wording, or distinctive composition.
- Keep desktop and mobile behavior visible during design, but also design and test the widths between them.
- Do not claim a concept is a production-ready full website. Do not publish or deploy unless requested.

## Workflow

### 1. Discovery and Evidence

Read [discovery-and-strategy.md](references/discovery-and-strategy.md) when starting a project, auditing an existing site, collecting assets, extracting a brand system, verifying business facts, planning pages, or defining SEO and outcomes.

Do not begin visual exploration until the reusable-asset inventory and current visual-system extraction have been completed, or the records explicitly state that no usable assets or established system were found. This is a discovery gate, not an optional polish step.

Produce or update the relevant project records rather than relying on chat history alone. Typical records include:

- `business-research.md` or `info.md`
- `issues.md`
- `material-additional-issues.md`
- `asset-inventory.md` and an `assets/` directory
- `brand-system.md` or `colortheme.md`
- `website-outline.md`
- `seo-plan.md`

Material additional issues are researched inconsistencies or missing inputs that cannot safely be resolved from outside the business. Present them neutrally for client verification and list the exact deliverable needed.

### 2. Homepage Concept Outline

For a homepage concept, redesign pitch, or homepage-first project, create or update `homepage-concept-outline.md` before visual exploration. A general sitemap or website outline is not a substitute for this record.

The outline must turn the research into a pitchable homepage narrative and make the reasoning inspectable. Include:

- the concept objective, working positioning/promise, primary audiences, urgent journeys, primary CTA, and secondary routes;
- the proposed section order, with one clear job for each section and its audience state, content, conversion target, trust function, and relationship to adjacent sections;
- an explicit mapping from every material website issue to the homepage section or architecture change that addresses it, including the evidence, asset, or client input required;
- the confirmed facts and reusable assets each section may use, plus proposed copy, proposed tokens, and unresolved client-dependent inputs clearly labeled;
- the proof strategy, claim/content gates, mobile and desktop narrative behavior, SEO/accessibility implications, and measurable acceptance criteria;
- a short list of what the homepage deliberately will not claim or attempt to explain.

Do not begin final visual design until this outline exists and the current working direction is accepted for exploration. Missing facts may remain provisional, but they must be visible in the outline and must not be converted into invented copy, metrics, credentials, testimonials, or promises. The outline is a strategy artifact, not a claim that the final copy or production design has been approved.

### 3. Strategy and Architecture

Define the site's audiences, urgent and routine user journeys, business priorities, desired conversions, sitemap, page intent, content hierarchy, trust signals, SEO targets, accessibility expectations, and measurable acceptance criteria.

Derive the visual language from the industry and the specific business. A law firm should feel dependable and precise; real estate should prioritize place, property, and aspiration; fintech should prioritize clarity, control, and security. Do not reduce an industry to clichés.

### 4. Section Design Exploration

Read [design-and-selection.md](references/design-and-selection.md) whenever the user asks to design, explore, or choose a section.

Unless the user specifies another order, begin with the navbar and hero. Then proceed through the approved homepage outline one section at a time.

For each section:

1. Confirm its job, content, conversion target, trust function, and relationship to adjacent sections.
2. Research several relevant references across sources such as Dribbble, Figma Community/templates, high-quality live sites, editorial layouts, and sector-specific examples.
3. Generate three materially distinct original options—not three color variations.
4. Show desktop and mobile together for every option. Explain the structural idea and any asset dependency.
5. Wait for selection or requested revision before implementing that section.

### 5. Faithful Implementation

Read [implementation-and-qa.md](references/implementation-and-qa.md) after an option is selected or when working in code.

Treat the approved visual as the primary visual specification and the verified content/brand files as the factual specification. Implement it faithfully in the project's existing stack. Preserve the composition, crop, typography, hierarchy, geometry, spacing, and responsive intent—not merely the general theme.

Use semantic structure, accessible interactions, optimized media, useful metadata, clear internal links, and stable responsive behavior. Implement real routes and interaction states when they are in scope; do not leave important controls as decorative elements.

### 6. QA and Handoff

Compare the implementation against the approved design at matching viewport sizes. Test the full responsive transition, interactions, keyboard behavior, visible focus, contrast, overflow, media loading, links, console, build, and reduced motion where applicable.

Use the project-defined breakpoints. If none exist, start with 320, 375, 390, 640, 768, 1024, 1025, 1279, 1280, and 1440 pixels, adding any widths where the composition changes. Record evidence in `design-qa.md` and leave failures open until resolved.

At handoff, distinguish clearly among:

- designed but not implemented;
- implemented but not fully verified;
- verified local concept;
- published concept;
- production-ready full site.

## Communication Pattern

Lead with the current outcome and decision needed. During exploration, make the three options easy to compare. After selection, treat the choice as locked unless the user changes it. When blocked by missing internal information, continue all safe work and present a precise content/asset request instead of guessing.
