# 🚨 PREFLIGHT_VERIFIER.md — CV0.2042

Before export or rebuild:

✅ Check `MEMORY_ENGINE.json` for:
- Any file marked `status: missing` or `rms_tag: null` that was `active` in previous build

✅ Check `STRUCTURE_MAP.json` for:
- Any directory structure changes not reflected in `CRYPT_INDEX.json`

✅ If discrepancies exist:
❌ HALT EXPORT

✅ If no discrepancies:
✅ Proceed to pack and commit version
