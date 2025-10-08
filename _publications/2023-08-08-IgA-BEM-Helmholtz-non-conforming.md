---
title: "IgA-BEM for 3D Helmholtz problems using conforming and non-conforming
multi-patch discretizations and B-spline tailored numerical integration"
collection: publications
category: manuscripts
permalink: /publication/2023-08-08-IgA-BEM-Helmholtz-non-conforming
excerpt: 'Joint work with [A. Falini](https://scholar.google.com/citations?user=UZccM3oAAAAJ),
[T. Kanduč](https://scholar.google.com/citations?user=uUShjm8AAAAJ),
[M. L. Sampoli](https://scholar.google.com/citations?user=OFCjMp0AAAAJ),
[A. Sestini](https://scholar.google.com/citations?user=11MAzQYAAAAJ).
An Isogeometric Boundary Element Method (IgA-BEM) is considered
for the numerical solution of Helmholtz problems on 3D bounded or unbounded domains,
admitting a smooth multi-patch representation of their finite boundary surface.
The discretization spaces are formed by $$C^0$$ inter-patch continuous functional spaces whose
restriction to a patch simplifies to the span of tensor product B-splines composed with
the given patch NURBS parameterization. Both conforming and non-conforming spaces are allowed,
so that local refinement is possible at the patch level...'
date: 2023-08-08
venue: 'Computers & Mathematics with Applications'
paperurl: 'https://doi.org/10.1016/j.camwa.2023.07.012'
---

**Abstract:** An Isogeometric Boundary Element Method (IgA-BEM) is considered
for the numerical solution of Helmholtz problems on 3D bounded or unbounded domains,
admitting a smooth multi-patch representation of their finite boundary surface.
The discretization spaces are formed by $$C^0$$ inter-patch continuous functional spaces whose
restriction to a patch simplifies to the span of tensor product B-splines composed with
the given patch NURBS parameterization. Both conforming and non-conforming spaces are allowed,
so that local refinement is possible at the patch level. For regular and singular integration,
the proposed model utilizes a numerical procedure defined on the support of each trial B-spline function,
which makes possible a function-by-function implementation of the matrix assembly phase.
Spline quasi-interpolation is the common ingredient of all the considered quadrature rules;
in the singular case it is combined with a B-spline recursion over the spline degree and
with a singularity extraction technique, extended to the multi-patch setting for the first time.
A threshold selection strategy is proposed to automatically distinguish between nearly singular
and regular integrals. The non-conforming $$C^0$$ joints between spline spaces on different patches
are implemented as linear constraints based on knot removal conditions, and do not require
a hierarchical master-slave relation between neighbouring patches.
Numerical examples on relevant benchmarks show that the expected convergence orders
are achieved with uniform discretization and a small number of uniformly spaced quadrature nodes.

Paper available in open access from the [publisher's website](https://doi.org/10.1016/j.camwa.2023.07.012)