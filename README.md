# Poker society tooling

Tools written while running one of Ireland's largest college poker societies.

| What | File | Use it for |
|---|---|---|
| Blind timer, desktop | [`Timer.py`](Timer.py) | Running a tournament clock with a full blind-structure editor |
| Blind timer, browser | [`Timer_v2.html`](Timer_v2.html) | The one actually used at the table |
| Blind structures | `poker_blinds*.jpeg` | Printed sheets the default levels come from |
| Kit sourcing | [`KIT_SOURCING.md`](KIT_SOURCING.md) · [`kit-sourcing.html`](kit-sourcing.html) | Working out where to buy buttons and cut cards after the 2026 EU import rules |

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
version: 5c/10c blinds, chips 5c/25c/50c/€1/€2/€5, €5/€10/€15 buy-ins with
the chip count for each, and Michael's Revolut QR (@michaelt8b).

## Run

```bash
python Timer.py          # desktop version
start Timer_v2.html      # browser version (Windows; or just double-click it)
```

## Kit sourcing

Written in October 2026 when the society needed dealer buttons, all-in buttons
and cut cards for eight mats. It turned into a real piece of work because the
EU dropped the 150 euro duty-free threshold on 1 July 2026, so the cheapest
shelf price and the cheapest doorstep price stopped being the same thing.

[`KIT_SOURCING.md`](KIT_SOURCING.md) is the write-up: what the new duty rules
actually cost, the three supply routes compared on landed price and delivery
time, what to buy and the exact specs to insist on, and where the numbers could
be wrong.

[`kit-sourcing.html`](kit-sourcing.html) is the same thing as a page you can
poke at. The basket quantities and the China unit price are adjustable and
everything recalculates, which matters because the unit price is what decides
the whole thing. It also carries the pre-purchase checklist. Open the file in
any browser, no server needed.

The short version, if you only want the one number: the breakeven on a 50 mm
four-piece button set is around 3.50 euro. Below that, buy from China. Above
it, Amazon UK is the same money and arrives in a third of the time.

## Picking this up on another machine

Two separate things live in two separate places, and only one of them is here.

**In this repo**, so a `git pull` gets it: the research, the decisions and the
reasoning behind them, plus the offline copy of the page. That is
`KIT_SOURCING.md` and `kit-sourcing.html`.

**In the Claude account**, not in the repo: the live basket figures and which
pre-purchase boxes have been ticked. Those are at
<https://claude.ai/artifact/E9LvqqVE2QWna55CbcAo6h> and follow the account
across machines. The `kit-sourcing.html` copy in this repo saves to whatever
browser opens it, so ticking a box there does not travel.

So on the other box: `git pull` for the write-up, and open the artifact link
for the working state.
