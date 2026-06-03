# session_capsule_protocol
Portable continuity protocol for AI sessions: preserves state, failures, next steps, and do-not-repeat instructions so future sessions restore context instead of starting cold.
# Session Capsule Protocol

AI keeps losing the plot.

Every serious AI workflow eventually hits the same wall: the session resets, the context disappears, and the user has to rebuild everything manually.

What were we doing? What broke? What worked? What should not be repeated? What is the next safe step?

The **Session Capsule Protocol** is a portable continuity system for AI workflows. It creates a handoff capsule that preserves operational state so a later AI session can restore context instead of starting cold.

## What a capsule preserves

- current state
- failure history
- restore point
- next safe step
- do-not-repeat instructions
- JSON continuity records
- Markdown continuity records
- lightweight recall behavior for future sessions

## Proof artifacts

- `session_capsule_app.py` — reusable Python utility for creating, validating, saving, loading, indexing, and recalling capsules.
- `examples/example_capsule.json` — machine-readable sample capsule.
- `examples/example_capsule.md` — human-readable sample capsule.
- `TEST_RESULTS.md` — validation output showing 13/13 checks passed.

## Why this matters

Most AI systems answer from the current prompt window. When the session resets, the user has to rebuild context manually.

The Session Capsule Protocol gives the workflow a portable restore point: state, failures, next steps, and boundaries travel together.

## Current validation status

The current local validation run passed 13/13 checks.

## Core thesis

AI should not generate before it orients.

AI should not make users rebuild context every time a session resets.

Live demo: https://clairesystems.ai

Created by Steven Roth, founder of CLAIRE Systems.

Patent-pending AI continuity / governed memory architecture.
