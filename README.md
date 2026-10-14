# Discrete Probability Distributions – AIML Lab

Interactive web lab for exploring the **Binomial distribution**, built step by step as part of the AIML Lab at BMS Institute of Technology and Management (BMSIT).

**Live demo:** https://akshitarajesh2-code.github.io/discrete-probability-distributions-lab/

## Features
- Inputs for number of trials `n`, success probability `p` and target successes `k`, with validation
- Live statistics: mean `np`, variance `np(1-p)`, standard deviation, second moment `E[X²]`, skewness
- PMF calculator: `P(X = k) = C(n,k) · p^k · (1-p)^(n-k)`
- CDF calculator: `P(X ≤ k)` and complement `P(X > k)`
- Interactive PMF bar chart with the `k` bar highlighted and a dashed line at the mean
- Placeholder modules for Poisson and Geometric distributions

Default check: `n = 20, p = 0.35` gives mean = 7, variance = 4.55.

## Project structure
| File | Description |
|------|-------------|
| `index.html` | Final version (all features) |
| `step0-binomial-explorer.html` | Slider-based explorer with PMF/CDF chart |
| `step1-input-validation-pmf-chart.html` | Number inputs with validation + PMF chart |
| `step2-statistics.html` | Mean, variance, std dev, 2nd moment, skewness |
| `step3-pmf-calculator.html` | Exact `P(X = k)` calculator |
| `step4-cdf-calculator.html` | `P(X ≤ k)` and `P(X > k)` calculator |
| `step5-pmf-graph-mean-line.html` | PMF graph with highlighted `k` and mean line |

## Tech stack
HTML, JavaScript, Tailwind CSS, Chart.js (+ annotation plugin). No build step — open `index.html` in a browser.

## Author
Akshita Rajesh — B.E. CSE (AIML), BMSIT
