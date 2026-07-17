# Plate Discipline

**The Moneyball of NYC food** — an over/underrated guide to New York pizza (Mexican and Thai next).

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

One Bite (Barstool) public reviews (~57k, 2018–2026), NYC DOHMH inspections,
editorial "best pizza" lists via the Wayback Machine, and a Yelp snapshot.
NYC only. A demo — signals, not gospel.

## Logo

A pepperoni pizza whose pepperonis trace a baseball's two seams (`logo.svg`).
