# Poker Tournament Timer

A tournament blind timer built for running live poker events — written while
running one of Ireland's largest college poker societies.

Two versions:

- **`Timer.py`** — desktop app (Python/Tkinter, no dependencies beyond the
  standard library). Full blind structure editor: per-level small blind, big
  blind, ante, and duration, with pause/resume and level skip.
- **`Timer_v2.html`** — standalone browser version of the same timer; open the
  file in any browser, no server or install needed. This is the one used at
  the table.

`poker_blinds.jpeg` is the printed blind-structure sheet the default levels
are based on.

## Run

```bash
python Timer.py          # desktop version
start Timer_v2.html      # browser version (Windows; or just double-click it)
```
