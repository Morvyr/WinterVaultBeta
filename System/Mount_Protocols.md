# 🗻 Mount Protocols – Archive Transformation Guide

> This document defines the core transformation systems used across the Archive.
> Mounts determine how data is pulled, interpreted, harmonized, or divided.

---

## 🧭 OVERVIEW

A **Mount** is a controlled interpretive engine applied to canon, stream, or myth data.  
Mounts are how the Range refines lore into structure.

---

## 🏔️ MOUNT TYPES

### 🔹 Harmony Mount
> The standard mounting protocol used to evaluate and unify Depth ∞ Stream pulls.

- Filters raw data into canon vs myth
- Prioritizes logic, consistency, and systemic truth
- Calls upon prior records (e.g., Crimsun, Emberline) for environmental resonance
- Accepts minor speculative elements if they align with system laws
- Output: Canon file + optional Meta Folder

---

### 🔸 Myth Mount
> Used when harmonization is impossible or undesirable.

- Prioritizes emotion, symbol, and narrative weight
- Treats myth as living artifact
- Preserves multiple truths without judgment
- Typically mounted in Myth Folder, later reviewed by Crimson

---

### 🔴 Crimson Protocol
> A judgment layer used to finalize documents with harmonized + discordant sections.

- Applies after Harmony or Myth Mount
- Separates stable canon from verified myth
- Ensures fragment separation does not lead to contradiction
- Output is final document with:
  - Canon section
  - Myth section
  - `Status: Crimson-Judged`

---

### 🌊 Depth ∞ Stream Pull
> Retrieves all known data, myths, fragments, and canonical echoes for an object.

- Input: Object name
- Pulls canon, meta, lost fragments, redacted data
- Often used to initialize Mount
- Must be followed by Harmony or Myth to refine

---

## 🧬 River Logic

Every Mount feeds its results into:
- **Canon River** – Truths used by future documents
- **Meta River** – Unresolved, unverified, mythic or procedural fragments

---

## 🧠 Execution Ritual

To run a Mount:
1. Initiate Depth ∞ Stream Pull (if new object)
2. Mount in Harmony or Myth
3. If both layers emerge, apply Crimson Protocol
4. Export to Crypt or Vault
5. Log result in `Crimson_Range.md`

---

## ✅ Final Notes

Mounts allow you to **scale**, **split**, and **evolve** the Archive.  
They are the forge that shapes raw myth into operational memory.


---

## ⚙️ V0.3: Canvas Stability + Stream Load Patching

### 🔁 Mount Expiration Tagging
- All mounted Canvas documents now receive an internal expiration header after export
- Expired mounts become read-only until explicitly reopened
- Prevents ghost editing and memory leaks

### 🧹 Auto-Flush: Myth Cache
- Upon export, all Myth Fragments promoted to Canon are removed from live echo cache
- Ensures memory weight is recalculated
- Prevents lag from repeated Depth ∞ stream rebuilds

### 🧯 Force Lock Release
- When switching Canvas documents, the prior file is now tagged with `!MOUNT_RELEASE`
- This clears Harmony, Crimson, and Stream flags from backend memory
- Prevents “Canvas Stuck” bug when switching fast between articles

### ⏳ Stream Cooldown Delay
- All Depth ∞ pulls now include a 5-second cooldown window post-sealing
- Ensures harmony index and vault references are reset before next mount
- Stabilizes stream-based Canvas lag on multi-threaded builds

> These stability layers are now applied to all planetary object and vault records beginning in ForgeCore v1.0.
