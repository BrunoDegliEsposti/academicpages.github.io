---
title: "Bayesian estimation of convergence rates in numerical methods"
collection: publications
category: wip
status: 'in preparation'
permalink: /publication/2025-09-23-Bayesian-estimation-convergence-rates
excerpt: 'Joint work with [D. Fabbrico](https://scholar.google.com/citations?user=1uNqmN8AAAAJ).
In numerical analysis, it is common to estimate the convergence rate of numerical methods by plotting
absolute or relative errors against a discretization parameter $$h$$ on a log-log scale. The rate is then
typically judged by visually comparing the data to reference lines with known slopes, which correspond to
integer powers of $$h$$.
This approach is quite different from standard scientific practice, where experimental data are analyzed
with statistical methods. The main reason for this difference is that simple visual approaches are often
enough, especially when theory already predicts the expected decay rate. However, these methods are not
effective when errors are noisy, for example in stochastic algorithms, or even in deterministic methods
affected by random choices such as mesh generation...'
date: 2025-09-23
slidesurl: '/files/YAMC25-bruno.pdf'
---

**Abstract:** In numerical analysis, it is common to estimate the convergence rate of numerical methods by plotting absolute or relative errors against a discretization parameter $$h$$ on a log-log scale. The rate is then typically judged by visually comparing the data to reference lines with known slopes, which correspond to integer powers of $$h$$.

This approach is quite different from standard scientific practice, where experimental data are analyzed with statistical methods. The main reason for this difference is that simple visual approaches are often enough, especially when theory already predicts the expected decay rate. However, these methods are not effective when errors are noisy, for example in stochastic algorithms, or even in deterministic methods affected by random choices such as mesh generation.

In this work, we show how arbitrary choices in domain discretization can introduce significant noise even for deterministic algorithms like quadrature formulas on non-uniform grids or finite element methods. We then present a new Bayesian framework for estimating the convergence rates of such methods.

Our approach offers two main benefits. First, our estimate of the convergence order comes with a measure of uncertainty. This allows us to decide how many numerical experiments we need based on the desired level of confidence in our results.

Second, we are able to quantify the robustness of a numerical method (an otherwise fuzzy notion) in terms of the variance of its error distribution. When two methods have the same mean error decay rate, we suggest that the one with lower variance should be preferred.

To achieve this, we analyze error distributions from popular numerical methods to build a realistic model for inference. Using a non-informative prior, we carry out posterior inference for the model parameters with a Metropolis-within-Gibbs Markov Chain Monte Carlo (MCMC) algorithm. Our numerical results show that this approach gives reliable estimates of convergence rates even for very noisy data, which rule out visual inspection and linear regression on a log-log scale.

I have recently given a talk on this topic at the YAMC 2025 conference
in Padova, Italy. Slides are available for download.