# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

Build a flashcard application for practicing German vocabulary from a personal word list, while also using this project to learn Claude Code.

## Current State

This project is in early development. There is no build system, test framework, or application code yet — only raw vocabulary data and this documentation.

## Data

`data/raw/from_notes_app.txt` contains ~2300 lines of German vocabulary in plain text, organized into sections:

- **Adjektive** — adjectives
- **Nomen** — nouns (with grammatical gender, e.g. `Der Zweck`)
- **Verben** — verbs
- **Adverben** — adverbs
- **Phrasen** — phrases
- **Redewendung** — idioms
- **Slang**

Each entry follows the pattern: `German term - Norwegian translation, English meaning (optional notes)`

## Custom Skills

- `/commit` — creates a git commit using `.claude/skills/commit/SKILL.md`, which injects git status/diff/log as context automatically.
