# Exalted Reliquary

Crusader Kings III gameplay mod. Version **0.1.0**. Supported game version **1.20.***.

Canonical working copy: `Documents/Development/CK3 Mods/er` (outer descriptor `er.mod` beside the folder).

## Fantasy

One umbrella pack for the suite’s **artifact power fantasy**:

| Module | Name | Verbs |
| --- | --- | --- |
| M1 | Reliquary Core | Craft, Upgrade, Repair, Awaken, Vault Grandeur |
| M2 | Supreme Regalia | Commission title-scaling crown, refresh, auto-equip on succession |
| M3 | Dynasty Heirlooms | Bind to house, reclaim, never-lost restore |

Power lives on **artifacts and court grandeur**, not a demigod personal trait.

## Economy (headline ruleset)

Game rule `er_rule_economy` (Tweaks), default **`paid_expensive`**:

| Option | Multiplier |
| --- | --- |
| Free | ×0 |
| Paid — Modest | ×1 |
| Paid — Expensive | ×3 |
| Paid — Ruinous | ×8 |

Hub may cycle the live mode mid-campaign unless locked. AI defaults to always-free so treasuries are not wiped.

## Requirements

- **Royal Court (EP1)** soft-required for artifact verbs. Without it the manage hub still opens and a one-time toast explains the gate.
- No hard Workshop dependency. Soft peers only (SS / ED / SU).

## Player entry

One top-level decision: **Manage Reliquary** → hub → action menus. Game rules under **Tweaks**.

## Footprint

Additive only. Prefix `er_` on all IDs. No `replace_path`. Append-only on-actions. Unique artifact templates under `common/artifacts/templates/er_templates.txt`.

## Load order

If another artifact pack conflicts, load **Exalted Reliquary last** among artifact mods.
