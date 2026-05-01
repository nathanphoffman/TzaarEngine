---
name: TzaarEngine development roadmap
description: Planned 6-step progression from game engine to advanced AI
type: project
---

Agreed 6-step development plan:

1. **Game engine** — rules, move generation, board state, win detection. Pure logic, no AI. Foundation everything else depends on.
2. **Manual input class** — human can play and test positions. Verifies engine correctness before AI is layered on.
3. **Heuristic lookahead class** — non-AI traditional lookahead play (approximated by current captures.py). Baseline to measure AI improvement against, also generates plausible self-play data.
4. **Retrieval-based AI (user's approach)** — nearest-neighbor lookup against self-play dataset. Each (board_state, outcome_score) pair stored. Simpler than true Q-learning, generates labeled dataset as side effect.
5. **True Q-network** — train on dataset from step 4 as bootstrap. Retrieval approach acts as teacher giving network its initial signal. Dataset from step 4 is directly reusable here.
6. **AlphaZero-style** — policy + value networks with MCTS. Game engine, dataset, and Q-network from prior steps all feed in.

**Why:** Each step builds on the previous. Each stage provides a sparring partner for the next, giving a concrete measure of improvement. Dataset generated in step 4 remains useful in step 5 as labeled training data.

**How to apply:** When discussing new features or architecture, situate suggestions within this progression. Don't skip ahead — step 1 (complete correct game simulator) is the hard prerequisite for everything else.
