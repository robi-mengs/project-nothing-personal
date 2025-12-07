# Retrospective: Creating the Synthetic Patent Dataset

## What Went Well

It felt really good better than I expected. I never thought I’d be able to
generate a realistic-looking patent dataset on my own, but once I focused, it
clicked. The task came down to simple programming: building dictionaries,
looping through dates, and using random sampling concepts I’d learned in the MIT
Emerging Talent course. It even reminded me of Somaiya’s class on generating
synthetic data, which gave me the confidence to trust the process. Seeing the
final CSV with thousands of structured, plausible records was incredibly
satisfying.

## What Was Challenging

The hardest part was reverse-engineering what real USPTO data *might* look like
without ever accessing it. I spent several iterations studying public patent
examples, trying to understand field formats (like patent numbers), date
patterns, and common technology categories. I wanted the synthetic data to feel
authentic not just random strings, but something that mirrors real-world
structure and variation. That required patience, research, and several rounds of
refinement before the output felt credible.

## What I’d Do Differently Next Time  

If I were to do this again, I’d explore broader applications. Instead of
focusing only on USPTO-style patent records, I might generate synthetic **search
logs**, **user query trails**, or even simulate data from other innovation
platforms (like WIPO or Crunchbase). I’d also consider testing the same privacy
framework on a completely different domain—perhaps healthcare or academic
publishing to see how generalizable the approach really is. This experience
opened the door; next time, I’d walk through it wider.
