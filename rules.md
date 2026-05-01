# TZAAR — Complete Rules Reference

**Players:** 2 | **Type:** Abstract Strategy | **Release:** 2008

---

## Overview

TZAAR is a two-player abstract strategy game played on a hexagonal board. Players capture opponent pieces and build stacks, aiming to eliminate all of one piece type from the opponent's forces, or trap them into an illegal game state.

---

## Components

Each player receives 30 pieces in their color, split across three types. White and Black each have 6 Tzaars, 9 Tzarras, and 15 Totts, for a total of 60 pieces on the board. There is also one hexagonal game board and one rulebook.

---

## The Board

The board is hexagonal with a triangular grid. The 60 intersections are the only valid positions, called **spaces**. Pieces travel along the lines that connect spaces. There is no central space — pieces cannot cross the center of the board. Once a space becomes empty, it stays empty for the rest of the game.

---

## Piece Types

There are three types of pieces, which matter only for the win condition — not for movement or capture power.

**Tzaar** is the rarest piece. Each player starts with only 6. Losing all of your Tzaars means you lose the game.

**Tzarra** is the mid-tier piece. Each player starts with 9. Losing all of your Tzarras means you lose the game.

**Tott** is the most common piece. Each player starts with 15. Losing all of your Totts means you lose the game.

> Piece type does not determine strength. Strength is determined solely by stack height (see Section: Stacking).

---

## Setup

### Standard (Random)
Orient the board so its long axis runs between the two players. Place all 60 pieces randomly across the board, one per space. Draw lots to determine color. White always moves first.

### Fixed (Optional)
Place pieces in concentric rings on the hexagonal board. The innermost ring holds 6 Totts alternating by color. The next ring holds 12 Tzaars alternating by twos. The third ring holds 18 Tzarras alternating by threes. The outermost ring holds 24 Totts alternating by fours.

### Tournament
Start with an empty board. Players alternate placing one piece at a time in any order until all 60 are placed. Once full, the game proceeds normally with White moving first.

---

## Win Conditions

You win by achieving one of the following:

**Elimination** — Capture every opponent piece of a single type. Removing all of their Tzaars, all of their Tzarras, or all of their Totts wins the game instantly.

**Immobilization** — Put the opponent in a position where they cannot legally execute their mandatory first-move capture on their turn.

> ⚠️ Only solo pieces and the **top piece of each stack** count toward type-presence. Pieces buried inside a stack do NOT count. If the last piece of a type is buried, that type is considered gone and you lose.

---

## Turn Structure

### White's Very First Turn (Game Start Only)
White makes exactly one move: a mandatory capture of an adjacent Black piece. Because the board is full at game start, only adjacent captures are possible on this first move.

### All Subsequent Turns
Every turn after the opening consists of exactly two moves in order.

**Move 1 — Forced Capture (mandatory, cannot be skipped)**

Select one of your pieces or stacks. Move it in a straight line to the first space occupied by an opponent's piece or stack. The path may cross any number of empty spaces, but cannot jump over any other piece or stack. Your piece or stack replaces the opponent's, which is permanently removed from the game. Your piece or stack must be at least equal in height to the target. A stack of 2 can capture a stack of 1 or 2. A stack of 3 can capture a stack of 1, 2, or 3. And so on.

**Move 2 — Choose One of Three Options:**

*Option A: Second Capture* — Execute another capture following the exact same rules as Move 1. You may use the same piece or stack that captured in Move 1, or a different one.

*Option B: Strengthen (Stack)* — Move one of your pieces or stacks in a straight line onto another one of your own pieces or stacks. The movement rules are identical to capturing — straight line, over empty spaces only, no jumping pieces. The two combine into a single taller stack. Stacks can only contain pieces of one color. There is no height limit. Any type can stack onto any other type. Only the top piece of the resulting stack counts for type-presence.

*Option C: Pass* — Do nothing. Your turn ends immediately.

> ⚠️ You can never pass Move 1. The forced capture is always mandatory.

---

## Movement Rules

These constraints apply universally to all moves — captures and stacking alike.

A piece or stack always moves in a straight line along the grid. It may travel over any number of empty spaces to reach its destination. It cannot jump over any occupied space, friendly or enemy. It can never move to an empty space — the destination must always be occupied. Pieces cannot cross the center of the board.

---

## Stacking Rules

A stack is treated as a single entity at all times. It moves and is captured as a whole unit. The height of a stack determines its strength for capture purposes. Only the top piece of a stack counts for type-presence on the board. A stack can be of unlimited height. Stacks may only contain pieces of one color.

---

## End of Game

The game ends immediately when either win condition is met. You win if your opponent loses all pieces of any one type — including through burial in a stack where only the buried piece of that type remains. You also win if your opponent cannot legally make a forced capture on their turn.