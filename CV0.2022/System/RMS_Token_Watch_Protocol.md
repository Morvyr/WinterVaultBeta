ANCHOR:RMS_TOKEN_WATCH_PROTOCOL
TAGS: [SYSTEM, TOOL, PROTOCOL]
LINKS: [RMS_RESTORE_TOKEN, STREAM_STATE_JSON, RMS_TRIGGER_JSON]
TIER: SYSTEM
TOOL_TYPE: SYSTEM_MONITOR
AFFECTED_ANCHORS: []
STATUS: LIVE

---

# 🔁 RMS Token Watch Protocol

## Purpose
Tracks token usage across all live archive sessions. Triggers export warnings and updates ANN when thresholds are met.

## Tracked In:
- `stream.state.json`
- `rms.watch.log`
- `rms.trigger.json`

## Behavior
- Each token-generating action increments a counter
- If `tokens_written >= token_threshold`, sets `export:required = true`
- Updates ANN: `events: [TOKEN_WRITE]`
- Appends timestamped log entry to `rms.watch.log`

## Reset Behavior
- Resets every time a new session begins or export completes
- Last checkpoint stored in `RMS_Restore_Token.md`

## Sample State:
```json
{
  "needs_export": true,
  "tokens_written": 5103,
  "token_threshold": 5000
}
```

ANCHOR_HISTORY:
  - 2025-05-16T06:35Z: CREATED
