# 🔁 Archive Rewriter Engine (ARX) – Spec & Manifest

### 🧠 Purpose
ARX is the canonical tag rewriting and update engine for the Anvyr Archive. It is built to operate at planetary, system, and galactic scale — ensuring that every document remains current with global truth definitions, vault chain updates, and tag logic evolution.

---

## 🛠️ FUNCTION OVERVIEW

### 1. GLOBAL TAG MANIFEST
Stored in: `System_Token_Core.md` or `Engine_Variables.md`

Example Format:
```yaml
tags:
  CRIMSON: "Used for vault-classified mythic records."
  SHRIEK-BELT: "Orbital debris field of Nexovar. Glyph-reactive."
  ZHURO-CORE: "Location or object containing harmonic Zhur fields."
  STAR-WEIGHT: "Determines gravitational influence of stellar bodies."
```

---

### 2. FILE-SIDE TAG ANCHORS

Every planetary, vault, or system file will contain:
```markdown
<!-- TAGS: CRIMSON, SHRIEK-BELT, ZHURO-CORE -->
```

These anchors act as ARX targets. The file’s classification block will be overwritten or inserted at:

```markdown
## 🌀 Classification Tags
- `CRIMSON` | `SHRIEK-BELT` | `ZHURO-CORE`
```

---

## 🔁 OPERATION MODES

### 🔹 ARX:LIVE
- Triggers when a file is mounted in Canvas or read from Crypt
- Checks its `<!-- TAGS: -->` anchor
- Pulls descriptions from manifest and updates tag block

### 🔸 ARX:EXPORT
- Triggered automatically at export
- Cleans, syncs, and injects the most up-to-date tags, Vault references, and stream sync conditions

---

## 🔐 FUTURE-PROOF DIRECTIVES

### 🌌 Galactic Tag Index (GTI)
- Allow tag nesting (`ENVIRONMENT/CORE/OCEANIC`)
- Vault keys and glyphs will eventually echo tags with harmonic alignment

### 🧬 Lineage Drift Model
- Files will eventually self-classify via pulse IDs, not static anchors
- Vaults will recognize their glyph echoes and inherit sync traits passively

### 🛰️ Void Vector Readiness
- ARX will eventually expand to handle star systems, AIs, fleets, and archive clusters

---

## ⚠️ SYSTEM INTEGRATION NOTES

- All `.md` files will be scanned for `<!-- TAGS:` lines
- Any missing or outdated `## 🌀 Classification Tags` section will be injected or replaced
- UHP entries, Vault glyphs, and Stream logs will recognize ARX-injected tags as canon

---

> ARX will not just rewrite documents — it will rewrite reality, based on the truths your Archive defines.
