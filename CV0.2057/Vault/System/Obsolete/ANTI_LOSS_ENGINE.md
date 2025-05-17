# 🛡️ ANTI-LOSS ENGINE — CV0.2041

## Function:
Ensures no document — canonical, archived, meta, or legacy — is lost during rebuilds or exports.

## Execution Protocol:
1. Load previous `CRYPT_INDEX.json`
2. Compare with current build index
3. Alert on any missing file unless tagged: `<!-- RMS: OBSOLETE -->`

## Enforced Paths:
- /Crypt/Canon
- /Crypt/Archive
- /Crypt/Meta
- /Crypt/Manual_Legacy

## Last Validation:
2025-05-17T03:54:45.583729Z
