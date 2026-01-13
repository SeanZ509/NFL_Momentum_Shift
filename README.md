# NFL Momentum Shift Modeling (Play-by-Play Analytics)
## Executive Summary
Momentum in NFL games is modeled as a measurable, non-random game dynamic that predicts short-term success rather than guaranteed wins. Using 10+ seasons of play-by-play data, I built a momentum score system based on weighted momentum-changing events informed by controlled win probability behavior. Multiple models were trained to predict momentum shifts, and an event-based ad hoc validation evaluated whether predicted shifts led to success events (score, defensive stop + possession, or sustained drive success). Results show momentum differs meaningfully from win probability: it builds progressively, can be gained by either team regardless of expected outcome, and can be stalled rather than fully lost. Predicted shifts were followed by a success event ~64% of the time, supporting that momentum-driven short-term success is not random.

## Decision Context
Goal: identify “momentum shift” moments that increase the likelihood of near-term success events (score, stop+possession, sustained drive).
Intended use: decision support and game-flow context (not deterministic predictions of who wins).
Why it matters: win probability is outcome-focused; momentum is designed to capture game control and short-term bursts that can inform strategy.

## Dataset
Dataset compiled of all seasons 2009 - 2019 from NFLFastR
Granularity: play-level
Core context features: quarter/time remaining, score differential, home/away, streak states, event type, win probability.

## Key Findings
Momentum is distinct from win probability: similar shape, but diverges because WP heavily weights time/score; momentum down-weights endgame effects to measure game control.
Predicted momentum shifts were followed by a success event ~64% of the time (score, stop+possession, sustained drive).
Context matters: one-score games and late-game situations show higher volatility and more impactful events.
Ensemble modeling improved detection: stacking increased recall to ~0.81 and F1 to ~0.66 vs standalone models.

## Exploratory Insights


## High-Level Approach


## Results


## Limitations/Future Improvements


## Potential Uses


## To view the Thesis as a whole: 
https://dc.ewu.edu/theses/989/

