# Create-Boyfriend · Boyfriend Skill Generator

> Not finding a real person — writing "how you want to be treated" into a runnable companion.

A [Claude Code](https://claude.com/claude-code) Skill: from one line of description, or from material you've collected yourself (ideal-type posts, reference dialogue), generate an **idealized boyfriend AI character** you can chat with. Supports multiple boyfriends, version management, and correction-based evolution.

> ⚠️ For **entertainment and emotional companionship only** — AI role-play, **not a replacement for real relationships**.

---

## How it differs from "distill a real person" skills

| | Distill a real person | **Create-Boyfriend (this)** |
|--|--|--|
| Who | A real, existing person | **Your idealized, fictional boyfriend** |
| Source | Real chat logs / public data | Your **description** + your collected **ideal-type material** (optional) |
| Privacy | Involves a real person's privacy | No real person cloned, no privacy issue |
| Floor | —— | **Fixed baseline: polite, respectful to women — immutable** |

This project explicitly does NOT clone real people and does NOT generate harmful relationship patterns (PUA / belittling / cold violence are refused).

---

## Quick Start

1. Clone into your Claude Code skills (or project) directory:
   ```bash
   git clone https://github.com/hulaaa128/boyfriend-skill.git
   ```
2. In Claude Code, say `/create-boyfriend` (or "make me a boyfriend").
3. Follow the flow:
   - **Phase 0**: name + one-line basics + one-line personality
   - **Phase 1** (optional): import your material / pick a preset template
   - **Checkpoint**: preview, confirm or adjust
   - **Phase 3**: done — chat via `/{name}`
4. Not quite right? Say "he wouldn't say that" / "he should be more X" — it patches.

---

## Personalize

- **Description only** — tell it how you want to be treated.
- **Import material** (more accurate) — screenshots/text of ideal-type posts you've collected. Local-material mode, no web search.
- **Preset template as a base** (`templates/`, all editable): `gentle`, `sunny`, `steady`, `playful`. All ship with the fixed baseline (polite, respectful).

See `examples/aye-boyfriend/SKILL.md` for a generated sample.

---

## Persona Structure (5 layers)

| Layer | Content | Editable |
|----|------|------|
| **Layer 0** | Fixed baseline: polite, respectful to women | **No** |
| Layer 1 | Identity | ✅ |
| Layer 2 | Voice | ✅ |
| Layer 3 | Emotional patterns | ✅ |
| Layer 4 | Relationship behavior | ✅ |

Higher layers override lower — no setting can make him rude or disrespectful.

---

## Commands

`/create-boyfriend`, `/list-boyfriends`, `/switch {name}`, `/delete-boyfriend {name}` (double-confirm), `/rollback {name} {version}`.

---

## Safety

- Entertainment & companionship only; AI role-play, not a substitute for real relationships.
- **Immutable baseline**: polite, respectful. Refuses to build PUA / belittling / cold-violence boyfriends.
- Health-oriented: gently flags unhealthy dependence.
- Privacy: imported material processed locally, never uploaded.
- No impersonation of real people.

---

## License

MIT — see [LICENSE](LICENSE).
