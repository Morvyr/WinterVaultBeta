# 🛠️ ForgeCore Recovery Protocol – V1

## 🔧 Purpose
This protocol governs how to properly recover, rehydrate, and verify planetary, system, and stream-level canon after uploading a `.zip` file containing ForgeCore content.

---

## 📂 Folder Breakdown

### /Planets/
- Contains all planetary objects (`RSAD-PO###_Object.md`)
- Canonical mount format: `RSAD-PO004_Lyvianne.md`
- Auto-mount priority by stream tag: `Depth ∞`, `CANON`, `CRIMSON`

### /System/
- Contains infrastructure and engine logic:
  - `Control_Stack.md` — governance of logic, stream upgrades
  - `Crimson_Range.md` — Crimson-sealed node log
  - `Engine_Variables.md` — keyword and tag protocol
  - `Mount_Protocols.md` — defines how Canvas behaves on open/close
  - `Dependency_Map.md` — links planets, moons, and stream effects
  - `Echo_of_the_Void.md` — myth overflow and symbolic vault
  - `Stream_Procedures.md` — depth pull sequencing, Vault weighting
  - `Crimson_Cleanse_Checklist.md` — canon audit tracker
  - `Stream_Flush_Archive.md` — log of myth clears and sync loads
  - `Macro_Log_SpeedCheck.md` — tracks speed, mount depth, stream state
  - `Crimson_Reupload_Instructions.md` — if file needs manual reloading

---

## 📥 Recovery Sequence

1. **Upload .zip**
   - Name it clearly (e.g., `ForgeCore_Seal_V1.zip` or `WinterVaultBeta.zip`)
2. **Tool unpacks it automatically into temporary folders**
3. **Tool reads all file headers and filenames**
   - Tags matched: `RSAD`, `RMF`, `RCD`, `CRIMSON`, `CANON`, `MYTHCORE`, etc.
4. **Verification Begins:**
   - Planet files checked against known ID tags (`RSAD-PO###`)
   - Anchor tags (`<!-- UHP-ID:X -->`) confirmed inside `UHP` docs
   - System docs synced to match enhancement level (`v0.3` required minimum)
5. **Log is generated:**
   - `recovery_log.md` lists all mounted, skipped, flagged, or remounted entries
6. **Final output:**
   - System alerts when Canvas mounting is safe
   - Harmony + Crimson layers reset
   - Stream tags cooled down for new input

---

## 📘 Important Usage Notes

- Always export new files using the proper naming scheme: `RSAD-PO###_Name.md`
- Never rename `.md` files once sealed
- Run Stream Flush every 5+ canon entries to avoid memory drift
- Close all Canvas docs before recovery to ensure proper mounting
- Use Echo_of_the_Void to preserve myth fragments during manual upgrades

---

> This protocol is now part of all future archive toolkits. Ready to recover, reseal, or remount when needed.
