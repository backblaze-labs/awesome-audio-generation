# Contributing

Thanks for your interest in contributing. This list is the single source for developer-focused AI audio-generation tools; small, careful PRs keep it useful.

## How to contribute

1. Fork this repo.
2. Edit **`entries.yaml`** only. Do not edit `README.md` or `llms.txt` — those are regenerated from `entries.yaml`.
3. Place your entry in the appropriate category (see `categories.yaml` for the list of valid category slugs).
4. Open a PR. One entry per PR.

A maintainer will validate your entry, regenerate `README.md` + `llms.txt`, and merge.

## What belongs in the list

**We accept**
- Commercial TTS, music, or sound-generation APIs with developer access.
- Open-source models with a hosted endpoint or a `pip install` path.
- SDKs, CLIs, and libraries for audio processing.
- Voice-agent frameworks and real-time audio transport.
- GPU platforms commonly used to serve audio models.
- Evaluation leaderboards and perceptual-quality metrics.
- Template/demo projects and reference implementations.

**We don't accept**
- Research papers without runnable code or an API.
- Paywalled tools without developer access.
- Duplicate entries.
- Self-promotional content with no developer value.

## Inclusion requirements

- Public product or documentation page; URL resolves.
- Activity signal within the last 12 months (commit, release, docs update).
- Either a public API or an open-source install path.

## Entry format

Every entry is a YAML object in `entries.yaml`. Full schema at [`_shared/schema.json`](https://github.com/backblaze-labs/awesome-lists-spine/blob/main/_shared/schema.json) (maintained privately).

Example:

```yaml
- name: Kokoro TTS
  url: https://github.com/hexgrad/kokoro
  docs_url: https://huggingface.co/hexgrad/Kokoro-82M
  description: 82M param TTS model, top-ranked on TTS Arena. 8 languages, 26 voices.
  category: open-source-tts-models
  github: hexgrad/kokoro
  license: Apache-2.0
  sdks:
    - {language: Python (pip install kokoro)}
  b2_integration: ""
  last_verified: 2026-04-17
```

### Fields

| Field | Required | Notes |
|---|---|---|
| `name` | yes | Display name. |
| `url` | yes | Primary homepage or repo URL. |
| `description` | yes | One sentence, ≤300 chars. |
| `category` | yes | Slug from `categories.yaml`. |
| `last_verified` | yes | ISO date the entry was last checked. |
| `docs_url` |  | Developer documentation, if different from `url`. |
| `github` |  | `owner/repo` slug. Used for star enrichment. |
| `sdks` |  | Array of `{language, url}`. |
| `license` |  | SPDX short id (e.g., `MIT`, `Apache-2.0`). |
| `tags` |  | Kebab-case tags. |
| `b2_integration` |  | URL to docs for the tool's Backblaze B2 integration. Blank if none. |

## What happens after you submit

A maintainer validates the entry against the schema, runs star enrichment, regenerates the README, and merges. If your entry is out of scope or missing information, you'll get feedback on the PR.

## Code of conduct

This project follows standard open-source community norms. Be kind, be constructive, focus on the contribution.
