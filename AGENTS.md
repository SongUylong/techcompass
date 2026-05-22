# Project BMAD Agent Contract (OpenAI Codex)

This project uses BMAD skills through OpenAI Codex and Claude-compatible skill folders.

## Skill Resolution

- Codex skills: `/Users/eric/.codex/skills/bmad-*`
- Claude skills: `/Users/eric/.claude/skills/bmad-*`
- Project state: `bmad/`

Use the project state files in `bmad/` as the source of truth for TechCompass BMAD progress.

## Workflow Intents

Use these prompts to trigger BMAD flows:

- `bmad:init` to initialize project BMAD artifacts.
- `bmad:status` to read current workflow status.
- `bmad:next` to get the recommended next action.
- `bmad:create-story` and `bmad:dev-story` for implementation flow.

## Project Artifacts

- `bmad/project.yaml`
- `bmad/workflow-status.yaml`
- `bmad/sprint-status.yaml`
- `docs/bmad/*.md`
- `docs/stories/STORY-*.md`

## Language Policy

Read language settings from `bmad/project.yaml`:

- `language.communication_language` for assistant chat responses  with `English` fallback.
- `language.document_output_language` for generated project artifacts under `docs/` with `English` fallback.

## Editing Rule

Use `yq` for deterministic YAML updates in scripts and automation.
