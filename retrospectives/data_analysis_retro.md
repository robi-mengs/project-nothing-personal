# Retrospective: Data Analysis Phase

## What Went Well

Running the Python code with the synthetic dataset and experimenting with
different analytical angles felt deeply rewarding. Generating clear, compelling
visuals and seeing the **85% protection / 85% utility balance** emerge from the
data was a powerful moment. I never expected the results to so cleanly validate
my original intuition: that privacy and market intelligence *can* coexist.
Watching the side-by-side charts reveal how differential privacy masks strategic
intent while preserving trend-level insight gave me real confidence in the
approach.

## What Was Unexpected

I originally planned to follow a full data science pipeline including dedicated
data exploration and preparation phases but I intentionally skipped them. At
first, I worried this was a gap. But then I remembered: this wasn’t meant to be
a traditional predictive or descriptive project. It was an **evaluative data
science experiment** designed to test a hypothesis, not model outcomes. Omitting
EDA and preprocessing turned out to be not just acceptable, but *appropriate*
for the goal. Still, it felt unfamiliar, and I had to trust my own design
choice.

## What Surprised Me  

The **clarity of the visual outputs** stunned me. The timeline showing idea
leakage, the bar chart comparing raw vs. protected queries—these weren’t just
technical outputs; they were *narratives*. They told the story of risk and
protection so vividly that even non-technical founders could grasp the stakes in
seconds. I didn’t anticipate that synthetic data + simple privacy logic could
produce such persuasive evidence.

### What I’d Do Differently Next Time  

If I were to redo this analysis, I’d **explore a wider range of epsilon (ε)
values** not just ε = 1.0. I’d test ε = 0.1 (maximum privacy), ε = 0.5, ε = 2.0,
and beyond to map the full privacy-utility trade-off curve. With more epsilon
tuning, I could offer founders nuanced guidance: *“Use ε = 0.5 if you’re in
stealth mode; ε = 1.5 if you’re validating before filing.”* Knowing this earlier
would have strengthened both the rigor and practicality of the analysis.
