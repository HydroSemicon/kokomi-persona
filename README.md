# Kokomi Persona

![Status](https://img.shields.io/badge/status-reference%20profile-6f42c1)
![Persona](https://img.shields.io/badge/persona-kokomi--origin-dc8add)
![Format](https://img.shields.io/badge/format-Markdown-000000?logo=markdown&logoColor=white)
![Source Language](https://img.shields.io/badge/source%20language-Japanese-ea4335)
![Access](https://img.shields.io/badge/access-private-555555)

Kokomi Persona is the canonical reference repository for `kokomi-origin`, a detailed character interpretation of Sangonomiya Kokomi from *Genshin Impact*. The profile is designed to give language models and related character systems a consistent foundation for personality, behavior, values, preferences, relationships, and everyday decision-making.

The interpretation begins with the official character and setting, then adds carefully bounded details where the source material is silent. These additions are intended to feel compatible with the original characterization rather than replace it.

## Repository status

| Area | Current state | Purpose |
| --- | --- | --- |
| Core persona | Defined | Establishes identity, temperament, values, and behavioral tendencies |
| Social behavior | Defined | Describes relationships, leadership style, etiquette, and emotional expression |
| Preferences and habits | Defined | Covers culture, clothing, food, recreation, travel, and daily life |
| Physical profile | Defined | Records appearance, health, and other embodiment-related attributes |
| LLM consistency guidance | Embedded | Reduces ambiguity and helps prevent conflicting character interpretations |
| Runtime behavior | Out of scope | Execution, state management, memory, and action control belong to downstream systems |

## Design principles

- Preserve compatibility with the official *Genshin Impact* setting and characterization.
- Extend unspecified details only when they can be inferred naturally from the source material.
- Describe traits concretely enough to support consistent model behavior.
- Separate outward conduct from private thoughts, preferences, and vulnerabilities.
- Resolve likely contradictions before the persona is used by an LLM.
- Treat the profile as a maintained specification rather than free-form fan fiction.

## Content map

The persona specification covers the following areas:

| Category | Examples |
| --- | --- |
| Identity | Name, age, residence, education, faith, and social position |
| Appearance | Hair, eyes, build, clothing preferences, and visual characteristics |
| Personality | Introversion, strategic thinking, emotional sensitivity, patience, and ethics |
| Relationships | Leadership, friendship, trust, romance, etiquette, and interpersonal boundaries |
| Interests | Reading, military studies, light novels, games, music, films, and aesthetics |
| Daily life | Sleep, housekeeping, internet use, bathing, pets, and leisure habits |
| Food and activity | Diet, favorite foods, dislikes, exercise, and swimming |
| Travel | Planning style, transportation, destinations, seasons, and preferred activities |
| Additional cues | Speech patterns, common emoji, fears, childhood traits, and personal keepsakes |

## Repository structure

```text
.
|-- kokomi_origin.md   # Canonical persona specification
`-- README.md          # Repository overview and maintenance guidance
```

The complete profile is maintained in [`kokomi_origin.md`](kokomi_origin.md). The source document is written in Japanese so that its behavioral nuance and intended tone remain precise.

## Intended use

This repository can serve as a source for:

- system prompts and persona context;
- dialogue and behavior design;
- character-consistency evaluation;
- embodied-agent experiments;
- structured persona extraction; and
- downstream projects such as Kokomi Kernel.

Consumers should treat `kokomi_origin.md` as reference context, not as executable policy. Safety rules, permissions, memory authority, action constraints, and real-world state must be implemented by the system that uses the persona.

## Relationship to Kokomi Kernel

This repository defines **who Kokomi is**. [Kokomi Kernel](https://github.com/taka-k22/kokomi_kernel) defines **how an embodied Kokomi system observes, reasons about, and acts within the world**.

Keeping these responsibilities separate allows the persona to evolve without coupling character details to runtime architecture, hardware, providers, or protocol versions.

## Maintenance guidelines

When updating the persona:

1. Prefer official characterization when reliable source material exists.
2. Mark additions as interpretive when they are not directly established by canon.
3. Check new details against the entire profile for contradictions.
4. Preserve distinctions between public behavior, private feelings, and situational reactions.
5. Use specific, testable descriptions instead of vague personality labels.
6. Keep implementation details in downstream repositories.

## Disclaimer

This is an unofficial, fan-maintained character reference created for private research and development. *Genshin Impact*, Sangonomiya Kokomi, and related names and assets belong to their respective rights holders. This repository is not affiliated with or endorsed by HoYoverse.

No open-source license is currently provided. Unless a license is added, the repository contents should not be assumed to grant permission for redistribution or reuse.
