---
title: 'Tutorial: HotelFlow Reservation Workflow'
nextPage: '[[1|Lesson 1: Introduction & Setup]]'
---

Build PicoFlow's `HotelFlow` from the current demo source. It is a durable
reservation conversation that collects Portland-area hotel criteria, searches
a local catalog, presents priced results, supports repeated comparisons, and
ends in a booking confirmation.

You will learn how to:

- Register providers and flows in a NestJS application.
- Configure a flow model, step overrides, and memory compaction.
- Use `ExploreStep`, `PresentStep`, and `CompareStep` as focused stages.
- Route validated tool calls with `go(...)` and `stay(...)`.
- Preserve durable state while isolating stale presentation and comparison
  history.
- Safely evolve session documents and reason about step lifecycle hooks.

The source of truth is `src/myflow/hotel-flow` in the reference project. This
tutorial also applies the shared PicoFlow workflow and step-authoring
contracts.
