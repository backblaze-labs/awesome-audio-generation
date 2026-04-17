# CLAUDE.md — awesome-audio-generation

## What this list is

A curated directory of AI audio-generation tools that developers can integrate today: text-to-speech, music and sound generation, voice agents, and the surrounding infrastructure.

## Scope

**Include**
- Commercial TTS, music, and sound-generation APIs with developer access.
- Open-source models with a hosted endpoint or a `pip install` path.
- SDKs, CLIs, and libraries for audio processing.
- Voice-agent frameworks and real-time audio transport.
- GPU platforms commonly used to serve audio models.
- Evaluation leaderboards and perceptual-quality metrics.
- Template/demo projects and reference implementations.

**Exclude**
- Research papers without runnable code or an API.
- Paywalled tools that gate developer access.
- Duplicate entries — cross-listing across our other awesome-* lists is fine, duplicates within this list are not.
- Self-promotional content with no developer value.

**Inclusion requirements (every entry)**
- Public product or docs page; URL resolves.
- Activity signal within the last 12 months (commit, release, docs update).
- Either a public API or an open-source install path.

## Files in this repo

- `entries.yaml` — source of truth. Only hand-edit this file.
- `categories.yaml` — the section taxonomy. Authoritative for what slugs are valid.
- `header.md`, `footer.md` — hand-written prose bracketing the generated list.
- `README.md`, `llms.txt` — **generated**. Do not edit.
- `CONTRIBUTING.md` — instructions for human PR authors.
- `.enrichment-cache.json` — local star-count cache; gitignored.

## Schema

Full schema at `~/awesome-lists/_shared/schema.json`. Required: `name`, `url`, `description`, `category`, `last_verified`. Optional: `docs_url`, `github`, `sdks`, `license`, `tags`, `b2_integration`.

`b2_integration` is a URL pointing to docs for the tool's B2 integration. Leave as the empty string `""` when none exists yet. When a new integration ships, set this field and drop the tool from `~/awesome-lists/_internal/priorities.yaml`.

`category` must be a slug defined in `categories.yaml` — validate.py will reject anything else.

## Workflow

Adding or updating an entry:

1. Edit `entries.yaml` only. Append new entries at the end; ordering inside the file doesn't matter.
2. Validate:
   ```
   python ~/awesome-lists/scripts/validate.py --repo .
   ```
3. (Optional) Refresh stars:
   ```
   python ~/awesome-lists/scripts/enrich.py --repo .
   ```
4. Regenerate:
   ```
   python ~/awesome-lists/scripts/generate.py --repo .
   ```
5. Commit `entries.yaml`, `README.md`, `llms.txt` together. One entry per PR.

## Hard rules

- Never edit `README.md` or `llms.txt` by hand — any manual edit is overwritten on the next `generate.py` run.
- Never commit `.enrichment-cache.json`.
- Never delete an entry outright. If a tool is dead or discontinued, tag it `tags: [needs-review]` and file a note in `~/awesome-lists/_tasks/`.

## Good vs. rejected entries

**Good**
```yaml
- name: Pipecat (Daily)
  url: https://github.com/pipecat-ai/pipecat
  docs_url: https://docs.pipecat.ai
  description: Open-source Python framework for STT → LLM → TTS voice agent pipelines.
  category: voice-agent-frameworks
  github: pipecat-ai/pipecat
  license: BSD-2-Clause
  sdks:
    - {language: Python (pip install pipecat-ai)}
  b2_integration: ""
  last_verified: 2026-03-01
```

**Rejected**
- Out of scope: an STT-only service with no TTS/generation story.
- Vaporware: a landing page with a waitlist, no docs, no repo.
- Dead link: homepage 404s or repo archived >12 months ago with no successor.
