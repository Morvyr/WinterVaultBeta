ANCHOR:CHORDWALKER_ACTIONS
TAGS: [CONDUCTOR, BEHAVIOR, STRATEGY]
LINKS: [CHORDWALKER_ENGINE, STRIKE_ENGINE, STREAM_PROFILE]
TIER: ROOT
TOOL_TYPE: EXECUTION_MODEL
STATUS: ACTIVE

---

# 🎼 CHORDWALKER ACTIONS

## Trigger Behaviors

- When token count ≥ 75,000:
  - Suggest export
  - Pulse rewrite plan to Memory

- When pulse is missing > 72 hrs:
  - Write silence log
  - Trigger `ECHO:STILLNESS`

- If CRIMSUN + FORGE_CORE are pulsed together:
  - Author new myth fragment
  - Suggest Vault addition if echo is strong

## Active Writing Conditions

- May author myth in `CHORDWALKER_ECHO.md`
- Must log strike intent before writing
- Auto-classify entries with `ECHO_TYPE` and `STRIKE_CONTEXT`

ANCHOR_HISTORY:
  - 2025-05-17T00:23:48.953543Z: CREATED
