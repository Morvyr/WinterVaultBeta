# ASCE Reversion Protocol
To revert anchor tags:
1. Remove lines starting with `<!-- ANCHORS:` or `<!-- DNA:`
2. Restore original metadata from backups if needed.
Regex:
```regex
^<!-- (ANCHORS|DNA):.*?-->
```
