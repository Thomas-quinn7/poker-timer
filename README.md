# Poker society tooling

Tools written while running one of Ireland's largest college poker societies.

| What | File | Use it for |
|---|---|---|
| Blind timer, desktop | [`Timer.py`](Timer.py) | Running a tournament clock with a full blind-structure editor |
| Blind timer, browser | [`Timer_v2.html`](Timer_v2.html) | The one actually used at the table |
| Blind structures | `poker_blinds*.jpeg` | Printed sheets the default levels come from |

## Tournament timer

A tournament blind timer built for running live poker events.

Two versions:

- **`Timer.py`**: desktop app (Python/Tkinter, no dependencies beyond the
  standard library). Full blind structure editor: per-level small blind, big
  blind, ante, and duration, with pause/resume and level skip.
- **`Timer_v2.html`**: standalone browser version of the same timer; open the
  file in any browser, no server or install needed. This is the one used at
  the table.

`poker_blinds.jpeg` is the printed blind-structure sheet the default levels
are based on. `poker_blinds_johnny.jpeg` is the same sheet with Johnny's
Revolut QR (@johnpa61dj) for buy-ins. `poker_blinds_cash.jpeg` is the cash-game
version: 5c/10c blinds, chips white 5c, red 25c, blue €1, orange €2, purple €5,
yellow €10 (no 50c), €5/€10/€15 buy-ins with the chip count for each, and Michael's Revolut QR (@michaelt8b).

## Run

```bash
python Timer.py          # desktop version
start Timer_v2.html      # browser version (Windows; or just double-click it)
```
