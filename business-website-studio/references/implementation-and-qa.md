# Implementation and QA

Use this guide after a visual option is selected or when assessing an existing build against an approved design.

## 1. Establish the Implementation Contract

Before editing:

- inspect the existing stack, routes, components, tokens, assets, and uncommitted work;
- locate the approved design and written amendments;
- identify content that is confirmed versus provisional;
- list required interactions and responsive transformations;
- preserve user changes and already approved sections.

Use the existing stack unless the user requests a change. Do not replace the application with a new scaffold simply because it is easier.

## 2. Build Faithfully

Match the selected design's:

- overall composition and section height;
- image choice, crop, focal point, overlays, masks, and geometry;
- typography family, weight, size, line height, and wrapping;
- spacing, alignment, dividers, borders, icons, and color roles;
- visual and DOM hierarchy;
- desktop, tablet, intermediate, and mobile behavior.

Prefer semantic HTML and reusable, content-driven components. Use real links and buttons with correct states. Navigation controllers, tabs, accordions, maps, forms, and phone links must behave as presented.

For React/Vite/Tailwind projects, keep tokens centralized, avoid arbitrary breakpoint patches that conflict, and use CSS geometry such as `clip-path` carefully across all widths. Optimize images and reserve their layout space.

## 3. SEO, Accessibility, and Performance During Build

Include, as appropriate:

- one meaningful page H1 and logical subheadings;
- descriptive document title and metadata;
- crawlable links and stable routes;
- useful alt text, with decorative images correctly silent;
- labels, instructions, errors, and autocomplete for forms;
- keyboard operation, visible focus, and sensible reading order;
- adequate contrast and reduced-motion behavior;
- responsive images, lazy loading below the fold, and limited layout shift;
- structured data only from verified facts.

Do not postpone these concerns until after the visuals are complete.

## 4. Visual QA Matrix

Capture the approved reference and implementation at comparable sizes. Test the project's real breakpoints plus the widths immediately on both sides of each breakpoint.

If no matrix exists, begin with:

| Width | Primary risk |
| --- | --- |
| 320 | smallest supported composition and wrapping |
| 375 / 390 | common phone behavior |
| 640 | large phone/small tablet transition |
| 768 | tablet composition |
| 1024 | final compact-navigation/tablet state |
| 1025 | first wider-layout state |
| 1279 | last intermediate desktop state |
| 1280 | full desktop navigation/layout transition |
| 1440 | intended desktop composition and whitespace |

Also test representative heights. A section can look correct at the right width while hiding a CTA or creating excessive empty space at a shorter height.

At each size verify:

- no horizontal overflow or clipped content;
- intended navigation is present and usable;
- images fill their designed frames with correct focal points;
- special geometry remains visible and clean;
- text wrapping and spacing match the hierarchy;
- buttons, arrows, icons, and dividers do not collide;
- no accidental blank bands or unstable heights;
- adjacent sections join cleanly.

## 5. Functional QA

Verify:

- menus open, close, trap/return focus appropriately, and do not strand the page;
- tabs and accordions retain valid state without hiding all content;
- phone, email, external, internal, and map links resolve correctly;
- forms validate and explain submission behavior;
- sticky navigation does not cover anchor targets;
- browser console has no relevant errors;
- the production build and applicable tests pass;
- content and assets load at the deployed base path when deployment is in scope.

## 6. Record and Report Evidence

Maintain `design-qa.md` with:

- environment and commit/build identity;
- viewport matrix;
- reference and implementation screenshots;
- visual, interaction, accessibility, console, overflow, and build results;
- open defects, severity, and status.

Do not mark QA complete because the build command succeeded. Report the exact state: implemented, partially verified, fully verified locally, published concept, or production-ready.
