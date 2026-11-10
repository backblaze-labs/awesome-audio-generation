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

Every entry is a recommendation to developers, so each one must pass all four checks:

1. **In scope** for this list (see above).
2. **Usable today:**
   - the URL resolves;
   - a dated sign of activity in the last 12 months (release, commit, or dated changelog);
   - a developer access path: a documented public API or SDK with self-serve signup (paid is fine; waitlists and "contact sales" are not), public source with an install path, or downloadable datasets/weights with a stated license.
3. **Not already listed.** One entry per product: a vendor's per-model SDKs, or an API plus its MCP server, are one entry. New versions update the existing entry.
4. **Fits an existing category** in `categories.yaml`.

Self-submissions are welcome and held to the same bar. Low star counts are fine; clear docs matter more.

**We don't accept:** thin resellers of a single model, unofficial access to products that have no official API, consumer apps with no API/CLI/library, guides or directories of other tools (unless this list accepts them above), products whose primary purpose is adult content, and tools built to evade access controls (e.g. CAPTCHA solving) or impersonate real people.

**Writing the entry:**
- One factual sentence on what it does, ≤300 characters. No marketing adjectives, superlatives ("fastest", "#1"), or pricing/free-tier claims.
- Canonical URLs only: no `utm_`, referral, or affiliate parameters.
- `license` is the SPDX id from the repo; `sdks.language` is just the language name.
- Leave `b2_integration` as `""`; maintainers set it.
- Add or edit only your own product's entry.

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
| `b2_integration` |  | Maintainers only. Leave as `""`. |

## What happens after you submit

A maintainer checks the entry against the requirements above. Small fixes (formatting, URLs, description length, merge conflicts) are made for you, keeping you as the commit author. If we need information only you have, we'll ask one specific question; if the entry is out of scope, we'll close the PR with the reason.

## Code of conduct

This project follows standard open-source community norms. Be kind, be constructive, focus on the contribution.
