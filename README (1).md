# Discrete Probability Distributions

Interactive web app for the **Binomial, Poisson and Geometric** distributions, made at BMSIT. Built by vibe coding: I gave step-by-step prompts to AI and tested and fixed the output after each step.

**Live demo:** https://akshitarajesh2-code.github.io/discrete-probability-distributions-lab/

`index.html` is the final app. `step0` to `step5` show how it was built prompt by prompt.

## What I learnt
- **PMF** P(X = k) gives the probability of one exact value. **CDF** P(X ≤ k) adds them up. P(X > k) = 1 − P(X ≤ k)
- **Binomial:** number of successes in n trials. P(X = k) = C(n,k) p^k (1−p)^(n−k), mean = np, variance = np(1−p)
- **Poisson:** number of events at an average rate λ. P(X = k) = e^(−λ) λ^k / k!, mean = variance = λ
- **Geometric:** number of trials until the first success. P(X = k) = (1−p)^(k−1) p, mean = 1/p
- Increasing p shifts the Binomial graph to the right
- Poisson is a good approximation of Binomial when n is large and p is small (λ = np)
- In AI/ML these model things like correct predictions, error counts and attempts until success
- How to build a project in small prompt steps, check that the answers are correct, and fix bugs
- How to put a project on GitHub and host it live with GitHub Pages

## Experiment: quality control of defects
1. Binomial with n = 20, p = 0.05: mean = 1, variance = 0.95, P(X = 2) = 0.1887
2. PMF graph peaks at 1 defect and is almost zero after 4
3. With p = 0.10: mean = 2, variance = 1.80, P(X = 2) = 0.2852, and the graph shifts right
4. Poisson λ = 5 vs Binomial n = 100: P(5) = 0.1755 vs 0.1800, almost the same
5. Geometric p = 0.05: P(first defect on attempt 1) = 0.05, 2 = 0.0475, 10 = 0.0315, mean = 20 inspections

**Inference:** at a 5% defect rate the process is under control. At 10%, defects increase and the process needs checking. Poisson works for big batches, and on average 20 inspections are needed to find the first defect.
