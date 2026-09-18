# Discovery and Strategy

Use this guide before visual design when the project lacks a verified evidence base, brand system, sitemap, or outcome definition.

## 1. Establish the Evidence Base

Inspect all available sources:

- the current and archived business website;
- supplied briefs, documents, emails, and prior design decisions;
- official business profiles and social accounts;
- public regulator, professional-body, and corporate-register records;
- relevant review platforms and local listings;
- the existing repository and downloaded assets.

Browse when facts or external sources must be current. Prefer first-party and authoritative sources. Record URLs and access dates for material claims.

Capture every relevant item without silently treating it as approved website copy:

- business name, history, positioning, and differentiators;
- services and their priority;
- staff, roles, bios, qualifications, and accreditations;
- offices, service areas, opening arrangements, phones, emails, and emergency contacts;
- testimonials, case outcomes, articles, FAQs, fees, policies, and compliance statements;
- logo variants, icons, photography, video, documents, and social media assets;
- existing navigation, routes, forms, integrations, and calls to action.

### Mandatory asset and visual-system capture

Before visual exploration or implementation, create or update both an asset inventory and a working brand-system record. This requirement applies even when the business has no formal brand guide.

For reusable assets, record:

- the local filename or stable reference;
- the original URL, supplied-file source, or page where it was found;
- dimensions, format, subject, and likely crop/use;
- whether ownership, license, or permission is confirmed, unknown, or client-supplied;
- the intended section and whether a production replacement is required.

For the existing visual system, record what can be verified from CSS, brand files, or the rendered site:

- logo variants, clear-space and light/dark behavior;
- sampled or declared colors with HEX/RGB values and their roles;
- actual font families, weights, and files or hosted sources;
- type scale, spacing rhythm, buttons, borders, radii, icons, image treatment, and recurring UI patterns.

Use the recorded assets and visual system as the starting point for the concept. Label every inferred token or proposed extension separately from confirmed brand facts. If no reusable asset or established visual system exists, record that absence and state the replacement/creation dependency before designing.

## 2. Classify Findings

Keep four categories distinct:

1. **Confirmed** — supported by a reliable current source.
2. **Proposal** — a design, content, or journey recommendation.
3. **Website issue** — something the build can correct using confirmed information.
4. **Material additional issue** — a conflict or missing internal fact that requires the client's confirmation or deliverable.

Write material issues neutrally. State the website claim, the conflicting record or uncertainty, why it matters, and the exact answer or asset required. Never imply misconduct from a discrepancy alone.

## 3. Create the Working Records

Use the filenames already present in the project. Otherwise create the smallest useful set:

### `info.md` or `business-research.md`

- verified business profile;
- complete service inventory;
- people and office information;
- trust, regulatory, and social-proof information;
- available copy, articles, links, and public resources;
- sources and unresolved gaps.

### `issues.md`

For each addressable issue record:

- location;
- evidence;
- user/business impact;
- recommended solution;
- priority.

### `material-additional-issues.md`

For each client-dependent issue record:

- conflicting or incomplete information;
- evidence sources;
- why verification matters;
- specific question;
- requested deliverable;
- status.

### `asset-inventory.md`

For every asset record:

- local filename;
- original source;
- subject and context;
- dimensions/type;
- permission or public-use note when known;
- suitability and intended section;
- replacement required, yes/no.

Do not stretch thumbnails or use repeated images merely because they are available. Identify where a commissioned or licensed replacement is necessary.

### `brand-system.md` or `colortheme.md`

Record:

- logo variants and clear-space/background rules;
- sampled and verified colors with HEX/RGB values;
- TailwindCSS token names, including foreground/background pairings;
- actual site fonts and available weights/files;
- proposed fallback fonts only when the actual font is unavailable;
- type scale, spacing, border, radius, icon, and image-treatment direction.

Do not identify a font by appearance alone if CSS, font files, or brand guidance can confirm it.

## 4. Define Outcomes Before Layouts

Document:

- primary and secondary audiences;
- their urgent, sensitive, research, and routine journeys;
- business-priority services;
- primary and secondary conversions;
- objections and trust requirements;
- homepage role versus inner-page roles;
- performance, accessibility, SEO, and content-maintenance expectations;
- what success and acceptance will look like.

Translate business priorities into information hierarchy. Percentages supplied by the client are planning inputs, not necessarily visitor-facing content.

## 5. Create the Homepage Concept Outline

When a homepage concept or redesign pitch is in scope, create `homepage-concept-outline.md` before making final visual directions. A broad website outline can link to this document, but it does not replace it.

The homepage outline must be a strategy artifact that a client can react to before design. Record:

- the concept objective, working positioning/promise, priority audiences, urgent journeys, primary CTA, secondary routes, and the homepage's role in the wider site;
- the narrative order and one clear job for every proposed section;
- for each section: audience state, content and provisional copy, conversion target, trust function, adjacent-section relationship, asset/brand dependency, desktop/mobile behavior, and unresolved input;
- an issue-to-section matrix: current issue, user/business impact, homepage or architecture response, evidence/asset needed, and whether the response is confirmed or proposed;
- the proof strategy and a claim gate for metrics, testimonials, client logos, credentials, outcomes, guarantees, regulated language, and any other material claim;
- SEO, accessibility, performance, language, and content-maintenance implications;
- measurable acceptance criteria and a short “not on this homepage” boundary list.

Keep confirmed facts, proposals, website fixes, and client-dependent gaps visibly separate. Use the outline to expose missing decisions before visual exploration; do not hide unresolved facts inside polished copy or mockups. The final visual direction should reference the approved or explicitly current working outline section by section.

## 6. Create the Website Outline

For every planned page specify:

- route and search intent;
- target audience;
- primary question answered;
- required sections;
- primary CTA and alternative CTA;
- responsible team/person;
- trust evidence;
- required internal links;
- missing content or assets.

For the homepage, give every section one clear job and define the narrative order. Avoid duplicating the same claim or CTA throughout the page without a journey reason.

## 7. SEO Foundation

Plan SEO around useful pages, not keyword stuffing:

- one clear intent and descriptive title per route;
- a semantic heading hierarchy;
- accurate location/service combinations;
- crawlable navigation and contextual internal links;
- descriptive image filenames and alt decisions;
- Organization/LocalBusiness/ProfessionalService or other applicable structured data only when supported;
- canonical, social-sharing, robots, and sitemap requirements;
- performance and mobile usability as acceptance criteria;
- compliance-safe wording for claims, outcomes, and reviews.

Do not fabricate location pages or thin service pages merely to target search terms.
