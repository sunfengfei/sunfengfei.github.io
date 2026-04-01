---
layout: page
title: "Market Trading Experiment Platform"
---

**Updated:** 2026/03 &nbsp;|&nbsp; **Developer:** SUN Fengfei ([sunfengfei@u.nus.edu](mailto:sunfengfei@u.nus.edu))

## Overview

An oTree-based experimental economics platform for conducting multi-round trading experiments. Participants are assigned a utility function, parameters (α, β), and an initial endowment of Good A and Good B. They select a trading partner, negotiate and submit trades, and proceed through up to 3 trading rounds.

## Key Features

- Heterogeneous utility functions (Cobb-Douglas, Linear, Leontief)
- Partner selection and mutual/one-sided matching logic
- Real-time trade verification and execution
- Round-by-round history summary at the end

## Experiment Flow

1. **Login & Setup** — participants enter their student ID and receive their utility parameters and endowment
2. **Partner Selection** — participants nominate a trading partner by student ID
3. **Trading** (repeated for 3 rounds) — matched pairs submit trade quantities; trades are verified and executed if valid
4. **Summary** — final page shows full round-by-round history, final holdings, and utility

## Tech Stack

- Backend: Python / oTree
- Real-time matching via WebSocket (Redis)
- Configurable scenarios via session config keys
