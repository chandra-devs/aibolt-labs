---
title: Geometry that responds
description: How Kinetic connects contact location, directional tilt, cell waves, and semantic content response.
published: 2026-07-18
category: Interface physics
featured: true
---

Physical response becomes convincing when the visible result has a clear cause. Kinetic uses contact location, owned surface boundaries, damping, and cell distance to keep that cause visible.

## Directional plate response

Pointer position is resolved inside the nearest managed surface. Movement toward one edge compresses that side and raises the opposite side. The rotation remains bounded, the application’s own transform is preserved, and the scheduler stops when the surface reaches rest.

This is deliberately restrained. The purpose is to make the surface feel directional, not to stretch the entire interface around the cursor.

## Circular waves with coherent turbulence

A click begins a circular cell front at the actual input point. Speed controls travel. Thickness and recovery shape the leading and trailing bands. Turbulence bends the front coherently instead of turning it into random flicker.

Cell size, nesting depth, geometry, overflow, intensity, growth, and active-wave limits remain configurable. The same wave model runs across square, connected hexagon, circle, and interlocked diamond renderers.

## Content can participate

The surface is not the only object that responds. Kinetic can identify locally owned semantic groups and translate them at bounded depths. A wave lifts, rebounds, and settles those groups in distance order.

The semantic structure remains independent from the effect. Assistive technology reads the original content, and nested managed surfaces keep their own input ownership.

## Work only while work exists

Hover does not render a decorative cell field. The canvas is clear until an active wave needs it. Damped motion stops requesting frames at rest, device-pixel ratio is capped, and explicit budgets limit surfaces, active reactions, wave cells, and simultaneous waves.

Kinetic aims for a strong visible response without turning idle pages into permanent animation loops.
