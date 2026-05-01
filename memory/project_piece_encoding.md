---
name: Piece value encoding decision
description: Planned change to piece values in pieces.py to support stack height encoding
type: project
---

Decided to change piece values to: TOTT=1, TZARRA=16, TZAAR=50.

**Why:** The current values (TOTT=1, TZARRA=11, TZAAR=21) cause collisions when encoding stack height as `height * top_piece_value`. 11 TOTTs stacked = 11 = single TZARRA, ambiguous. New values give clean non-overlapping ranges: TOTT stacks 1–15, TZARRA stacks are multiples of 16, TZAAR stacks are multiples of 50. LCM(16,50)=400 which is unreachable in a real game.

**How to apply:** When updating pieces.py, change Piece enum to TOTT=1, TZARRA=16, TZAAR=50. Stack height is decoded as: value < 16 → TOTT (height=value), value % 16 == 0 → TZARRA (height=value/16), value % 50 == 0 → TZAAR (height=value/50). Also update get_piece_value range checks in scoring.py accordingly.
