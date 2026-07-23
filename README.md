# Plate Discipline

**The Moneyball of NYC food** — an over/underrated guide to New York pizza, Mexican, and Thai. Live at [platedisciplinenyc.com](https://www.platedisciplinenyc.com).

Star ratings, the line out the door, the cheese-pull photo describe *attention*,
not the next slice. Plate Discipline borrows the Moneyball move: separate the
review signals that *travel* (forecast next year) from the ones that just
happened, and surface the shops the market has mispriced — the neighborhood
spots where the rating doesn't tell the whole story.

**Two inspirations**

- *Moneyball* (Michael Lewis) — Billy Beane's A's used data to buy the value the
  market mispriced.
- *Prospect Theory* (Kahneman & Tversky) — enjoyment is judged against a
  reference point; delight is beating your expectation.

## Run it

`index.html` is a single self-contained page — data embedded, no build step.
Open it in a browser, or serve the folder:

```
python3 -m http.server
```

Two views:

- **Where to Go** — each shop's current rating vs the forward review signal the
  model reads, with a "worth-it" line marking the picks.
- **Hidden Gems** — attention vs modeled quality (the discovery read).

## Data

Model fit on the Yelp Open Dataset (~7M dated reviews, 11 metros); NYC venues
scored on current Google Places ratings and reviews. Venue universe from NYC
DOHMH inspections; attention axis from editorial best-of lists (Eater,
Infatuation, Grub Street). The earlier One Bite–only pizza build (~57k dated
slices, 2018–2026) is archived as v1. NYC only. A demo — signals, not gospel.

## Logo

A pepperoni pizza whose pepperonis trace a baseball's two seams (`logo.svg`).
