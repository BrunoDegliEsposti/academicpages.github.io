---
title: "A parallel-in-time isogeometric BEM for the 3D wave
equation using B-spline linear multistep methods"
collection: publications
category: wip
status: 'in preparation'
permalink: /publication/2026-05-25-isogeometric-BEM-wave-equation
excerpt: 'Joint work with
[L. Desiderio](https://scholar.google.com/citations?user=v7Z0uIIAAAAJ),
[M. L. Sampoli](https://scholar.google.com/citations?user=OFCjMp0AAAAJ),
[A. Sestini](https://scholar.google.com/citations?user=11MAzQYAAAAJ).
In this work, we introduce a novel high-order parallel-in-time
discretization for the 3D wave equation using linear
multistep methods as Boundary Value Methods (BVM).
Unlike Runge-Kutta CQ, which requires eigendecompositions
at the timestep level, our BVM approach exhibits
global diagonalizability, immediately yielding
decoupled Helmholtz problems...'
date: 2026-07-21
slidesurl: '/files/IMSE2026-bruno.pdf'
---

**Abstract:** Time-domain boundary integral equations (TDBIEs)
provide integral representations of solutions to
evolution problems in physics and engineering,
such as acoustic scattering in isotropic, homogeneous media.
Developing numerical methods for TDBIEs is a highly active
research area featuring competing approaches such as
the energetic Galerkin method, marching-on-in-time,
and convolution quadrature (CQ). For spatial discretization,
the combination of Isogeometric Analysis and the
Boundary Element Method (IgA-BEM) has emerged as
the leading high-order framework over the last decade.

Convolution quadrature methods transform TDBIEs
to the Laplace domain, converting the time integral into
a family of ordinary differential equations which are
then discretized using linear multistep or Runge-Kutta methods.
The TDBIE solution can be computed using Lubich's classical
forward-in-time approach, or newer parallel-in-time schemes.
For the wave equation reformulated as a TDBIE,
parallel-in-time schemes yield
a decoupled set of Helmholtz problems. The combination
of high-order IgA-BEM and Runge-Kutta convolution quadrature
was recently explored in Kramer, Marussig, Schanz (2026).

In this work, we introduce a novel high-order parallel-in-time
discretization for the 3D wave equation using linear
multistep methods as Boundary Value Methods (BVM).
Unlike Runge-Kutta CQ, which requires eigendecompositions
at the timestep level, our BVM approach exhibits
global diagonalizability, immediately yielding
decoupled Helmholtz problems. To mitigate the
growth of the condition number of the transformation
matrix, we use symmetric B-spline linear multistep
methods. Spatial discretization on multi-patch
surfaces is achieved via isogeometric collocation,
resulting in a fully spline-based scheme in both space and time.
Numerical experiments show that B-spline BVMs can be
significantly more accurate than state-of-the-art
Runge-Kutta CQ for equivalent sets of decoupled
Helmholtz problems.

I have given a talk on this topic at the IMSE 2026 conference
in Matera, Italy. Slides are available for download.