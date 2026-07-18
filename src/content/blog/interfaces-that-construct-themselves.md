---
title: Interfaces that construct themselves
description: Why Formation uses viewport travel, reversible geometry, and explicit lifecycle phases.
published: 2026-07-18
category: Interface engineering
featured: true
---

Most interface animation begins after the element is already visually present. Formation explores a different question: what if the interface visibly establishes where it belongs before it appears complete?

## Travel before enclosure

When viewport flow is enabled, four transient lines begin at the window boundaries and travel toward a measured target. Permanent rails start constructing as those lines arrive. Multiple targets are staged rather than appearing simultaneously, which makes the page feel assembled instead of decorated.

The viewport layer never becomes application content. It is hidden from accessibility APIs, ignores pointer input, and disappears when the controller is destroyed.

## Geometry carries meaning

Different profiles communicate different kinds of assembly. Straight rails feel structural. A continuous perimeter feels traced. Distributed segments feel attracted toward locks. Curved blades feel like an aperture closing.

Those differences belong in profile definitions, not in separate application integrations. A profile declares its geometry, supported tokens, completion behavior, renderer, responsive behavior, and reduced-motion outcome. The application continues to select a profile by name.

## Withdrawal must be equally intentional

A dramatic entrance followed by an unrelated disappearance breaks the physical idea. Formation therefore reverses target order, launches the viewport travel in the opposite direction, and deconstructs owned geometry through the same lifecycle contract.

An opposing command may arrive while a transition is active. Line-based profiles reverse from their current state instead of jumping to a new animation.

## Dynamic interfaces are normal

Modern applications insert routes, sections, dialogs, and lists after startup. With observation enabled, Formation batches those mutations, enhances new matches, restores elements that stop matching, and disconnects cleanly during destruction.

This keeps the integration at the application boundary. Developers do not need to modify every individual component simply to participate in Formation.
