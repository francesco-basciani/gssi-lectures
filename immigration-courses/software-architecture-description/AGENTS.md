# AGENTS.md - Software Architecture Description

## Purpose

This folder contains the interactive teaching material for the GSSI course **Software Architecture Description**.

## Source of truth

The current content is derived from the 2025 lecture materials provided by Francesco Basciani, in particular:

- *Software Architecture Design From Requirements*;
- *The Context - The Train Station Simulator*.

Do not silently add domain facts, railway standards, requirements, or architectural claims that are not supported by the teaching material unless explicitly requested. When external material is introduced, clearly distinguish it from the original course content.

## Teaching design

The intended classroom flow is:

1. instructor-led explanation;
2. progressively revealed context;
3. group discussion;
4. architecture sketching on paper/whiteboard;
5. group presentations;
6. instructor-led debrief using hidden/reveal sections.

The book must **support**, not replace, collaborative architectural reasoning.

## Content principles

- Keep the central theme: requirements -> architectural drivers -> architecture -> validation.
- Do not turn the group exercise into a tool-driven modeling task unless explicitly requested.
- Keep the proposed requirements and architecture hidden until the debrief section.
- Treat the final architecture as **a possible solution**, not the unique correct answer.
- Keep prose concise enough for classroom projection.
- Prefer MyST dropdowns, tabs, cards, and admonitions over custom JavaScript.
- Avoid adding executable notebooks unless they materially improve the learning objective.

## Technical checks

Before committing changes:

1. ensure `myst.yml` remains valid;
2. run `myst build --html` or `jupyter book build --html` when available;
3. check that all local image references resolve;
4. verify that solution sections remain hidden behind dropdowns;
5. do not commit `_build/`.
