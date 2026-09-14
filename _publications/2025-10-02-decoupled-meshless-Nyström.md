---
title: "Decoupling solution and quadrature nodes in meshless
Nyström methods for second-kind Fredholm integral equations"
collection: publications
category: wip
status: 'under review'
permalink: /publication/2025-10-02-decoupled-meshless-Nyström
excerpt: 'Preprint available on [arXiv](https://arxiv.org/abs/2510.17680).
Joint work with [A. Sestini](https://scholar.google.com/citations?user=11MAzQYAAAAJ).
We introduce a meshless Nyström method for Fredholm integral equations of the second
kind with smooth kernels in which the solution and quadrature nodes are chosen
independently. Meshless moment-free quadrature formulas discretize the integral
operator on scattered nodes, while local reconstruction with polyharmonic spline
radial basis functions transfers values from a coarser set of solution nodes
to a finer set of quadrature nodes. This construction yields a high-order
method applicable to complex domains and irregular node distributions...'
date: 2026-08-10
slidesurl: '/files/SMART2025-bruno.pdf'
---

**Abstract:** We introduce a meshless Nyström method for Fredholm integral equations of the second kind with smooth kernels in which the solution and quadrature nodes are chosen independently. Meshless moment-free quadrature formulas discretize the integral operator on scattered nodes, while local reconstruction with polyharmonic spline radial basis functions transfers values from a coarser set of solution nodes to a finer set of quadrature nodes. This construction yields a high-order method applicable to complex domains and irregular node distributions. We provide a well-posedness and convergence analysis of the resulting discretization. Under natural assumptions, we establish unique solvability for sufficiently dense node sets and derive an error bound that separates the contributions of quadrature and reconstruction. The overall convergence order is determined by the lower of the quadrature and reconstruction orders. When these orders coincide, we propose a coarse-grid parameter sweep to identify a nearly optimal ratio between the densities of solution and quadrature nodes. Numerical experiments on planar domains confirm the predicted rates and demonstrate a substantial increase in computational efficiency over the classical Nyström method, especially for narrow kernels.

I have given a talk on this topic at the SMART 2025 conference
in Reggio Calabria, Italy. Slides are available for download.
Preprint available at [https://arxiv.org/abs/2510.17680](https://arxiv.org/abs/2510.17680)