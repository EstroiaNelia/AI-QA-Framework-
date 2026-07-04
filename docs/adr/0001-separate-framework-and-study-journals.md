# ADR 0001 - Separate Framework and Study Journals

## Status

Accepted

## Date

2026-07-04

## Context

The repository currently contains both AI QA Framework development materials and CT-AI study materials.

These two workstreams are related, but they have different purposes:

- the AI QA Framework journal records the evolution, decisions and work sessions of the framework project;
- the CT-AI study journal records certification study notes, weekly reviews and study packs.

Keeping both types of notes under the same journal structure may create confusion as the repository grows.

## Decision

The repository will separate framework development notes from CT-AI study notes.

Project-related journal entries will remain under:

```text
docs/journal/

