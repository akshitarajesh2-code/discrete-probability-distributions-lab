# Discrete Probability Distributions – AIML Lab

Interactive web lab for exploring the **Binomial, Poisson and Geometric distributions**, built step by step as part of the AIML Lab at BMS Institute of Technology and Management (BMSIT).

**Live demo:** https://akshitarajesh2-code.github.io/discrete-probability-distributions-lab/

## Features
- Inputs for number of trials `n`, success probability `p` and target successes `k`, with validation
- Live statistics: mean `np`, variance `np(1-p)`, standard deviation, second moment `E[X²]`, skewness
- PMF calculator: `P(X = k) = C(n,k) · p^k · (1-p)^(n-k)`
- CDF calculator: `P(X ≤ k)` and complement `P(X > k)`
- Interactive PMF bar chart with the `k` bar highlighted and a dashed line at the mean
- **Poisson module:** rate `λ`, target count `k`, PMF `e^-λ λ^k / k!`, CDF, mean/variance `λ`, skewness `1/√λ`, chart with mean line
- **Geometric module:** success probability `p`, trial `k`, PMF `(1-p)^(k-1) p`, CDF `1-(1-p)^k`, mean `1/p`, variance `(1-p)/p²`, chart with mean line

Default checks: Binomial `n = 20, p = 0.35` → mean 7, variance 4.55 · Poisson `λ = 4, k = 3` → P(X = 3) = 0.1954 · Geometric `p = 0.2, k = 3` → P(X = 3) = 0.1280.

## Project structure
| File | Description |
|------|-------------|
| `index.html` | Final version: Binomial, Poisson and Geometric modules |
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
