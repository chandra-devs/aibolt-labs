---
title: Introducing DYNT
description: Formation and Kinetic are now independent, framework-neutral interface engines.
published: 2026-07-18
category: Release
featured: true
---

DYNT is an open-source interface system for applications that need more than a generic entrance animation or a decorative hover effect. It gives existing HTML two distinct capabilities: **Formation**, which constructs and reveals an interface through geometry, and **Kinetic**, which responds to contact through bounded physical behavior.

The two engines are intentionally separate. An application may install only `@dynt/formation`, only `@dynt/kinetic`, or both. React and Web Component packages remain thin lifecycle adapters over the same framework-neutral core.

## Formation is a lifecycle

Formation does not treat appearance as a single fade. A target can be located by lines travelling inward from the viewport, enclosed by permanent geometry, revealed, withdrawn, and deconstructed. The public lifecycle exposes those stages so applications can coordinate their own behavior without depending on animation timing guesses.

Nine built-in profiles express different construction grammars while preserving one initializer and controller contract. Line Push, Line Rise, Arc Trace, Squircle Sweep, Chamfer Fold, Magnetic Segment, Radial Compass, Aperture Iris, and Elastic Membrane each own their geometry and reversible sequencing.

## Kinetic begins at contact

Kinetic resolves the nearest managed surface and uses the input location as a physical cause. The near edge compresses while the far edge lifts. Clicks and programmatic impacts send circular fronts through square, connected hexagon, circular, or interlocked cells.

The canvas remains clear during ordinary pointer movement. Cells are rendered only while a wave is active. Semantic content can react at bounded depths, while application transforms, events, and accessibility remain application-owned.

## One boundary, existing HTML

Both engines initialize against a root and a selector. They discover matching elements without replacing them, support dynamic insertion through batched observation, and restore the exact state they own when destroyed.

```js
const root = document.querySelector('#app');

createFormation({ root, selector: '[data-surface]' });
createKinetic({ root, selector: '[data-surface]' });
```

This is the essential DYNT idea: keep the application semantic and framework-owned, then add construction or physical response at a boundary.

The first public release is available through npm, with source, API documentation, accessibility requirements, performance budgets, browser examples, and package verification in the public repository.
