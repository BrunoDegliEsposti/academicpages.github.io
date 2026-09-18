---
title: "A neural approach to point membership
classification using local boundary samples"
collection: publications
category: wip
status: 'in preparation'
permalink: /publication/2026-09-17-meshless-inclusion-tests
excerpt: 'Joint work with
[G. A. D''Inverno](https://scholar.google.com/citations?user=JsXiefkAAAAJ),
[F. Pelosi](https://scholar.google.com/citations?user=nAMdLzgAAAAJ),
[M. L. Sampoli](https://scholar.google.com/citations?user=OFCjMp0AAAAJ).
In this work, we explore the use of neural
networks to solve the point membership classification problem.
The network learn a suitable function and delivers a nearest-neighbor
method whose accuracy on randomly sampled query points exceeds
that of state-of-the-art nearest-neighbor methods, even on non-smooth domains.
Since the neural networks only take as inputs local boundary samples,
they are naturally domain-independent and very quick to evaluate...'
date: 2026-09-17
slidesurl: '/files/YAMC2026-contributed-bruno.pdf'
---

**Abstract:** Determining whether an arbitrary query point y in
$$\mathbb{R}^d$$ lies within the interior of a bounded domain is a
fundamental problem in computational geometry.
This point membership classification becomes particularly
challenging when the domain boundary is represented by
a scattered set of nodes $$Z$$ (a point cloud) and
their associated outward-pointing normal vectors.
Existing point inclusion techniques for this
representation generally fall into three categories:
nearest-neighbor queries, generalized winding numbers,
and surface reconstruction methods, each offering distinct trade-offs.

Nearest-neighbor inclusion tests are exceptionally fast
and therefore the most suitable for being used as subroutines
in more complex algorithms working on point clouds,
such as advancing front node generation in meshless algorithms.
However, nearest-neighbor methods, which test for inclusion only by
evaluating a function $$F$$ of the position of the $$K$$ nearest boundary nodes
and their normals, require expensive ad-hoc techniques to handle
non-smooth features of the boundary, such as edges and vertices.

In this work, we explore the use of neural
networks to solve the point membership classification problem.
The network learn a suitable function $$F$$ and delivers a nearest-neighbor
method whose accuracy on randomly sampled query points exceeds
that of state-of-the-art nearest-neighbor methods, even on non-smooth domains.
Since the neural networks only take as inputs local boundary samples,
they are naturally domain-independent and very quick to evaluate.

I have recently given a talk on this topic at YAMC 2026
in Torino, Italy. Slides are available for download.
