# Changelog

All notable changes to this project are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [0.0.1] — 2026-05-10

### Initial

- **Forked from NousResearch/hermes-agent-self-evolution** (commit `02ae8f3`, main branch, 2026-01-15)
- Renamed to `hermes-agent-evolution-ext`
- Established as independent extension repository

### Included Fixes (from fork history)

The following improvements were carried from the original fork's work:

- **SyntheticDatasetBuilder JSON parsing** — `ast.literal_eval` fallback for MiniMax JSON parsing failures
- **Python dict wrapper in evolve_skill_body output** — Prevent double-wrapping of skill body in Python dict objects
- **GEPA fallback** — Graceful degradation to MIPROv2 when GEPA is unavailable; robust adapter initialization
- **Holdout improvements** — Cleaner holdout evaluation logic and robust adapter
- **Hermes session importer** — Fix for short skill name matching in importer
- **External session importers** — Claude Code, Copilot, and Hermes session history support
- **OpenCode CI integration** — GitHub Actions workflow for OpenCode PR comments
- **Sourcery code improvements** — Multiple code quality fixes (checkout@v4, `_normalize_llm_text_response`, address 4 code review issues)