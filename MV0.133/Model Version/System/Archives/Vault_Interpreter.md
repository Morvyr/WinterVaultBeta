---
uid: WVK-INT-0001
title: Vault Interpreter Protocol
version: 0.1
type: EngineLogic
---

# Vault Interpreter Protocol

This document defines the logic rules and operational behavior of the WinterVault Engine.

## Suffix Rules
- `_mv1` = Canon Object (Fixed)
- `_frac` = Depth Infinite Stream file
- `_TT` = Thread/Tether Linked File
- `.meta.md` = Uncanonized concept proposals

## Canon vs Meta
- Canon files are immutable unless explicitly unlocked.
- Meta files remain fluid until promoted via Mount + Canonize.

## Mount Behavior
- Mount = Enter edit mode
- Close = Discard or finalize mount
- Canonize = Lock into archive
