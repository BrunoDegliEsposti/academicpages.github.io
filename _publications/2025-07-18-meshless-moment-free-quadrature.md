---
title: "Meshless moment-free quadrature formulas arising from numerical differentiation"
collection: publications
category: manuscripts
permalink: /publication/2025-07-18-meshless-moment-free-quadrature
excerpt: 'Joint work with [O. Davydov](https://oleg-davydov.de/).
We suggest a method for simultaneously generating
high order quadrature weights for integrals
over Lipschitz domains and their boundaries that requires neither meshing nor moment computation.
The weights are computed on pre-defined scattered nodes as a minimum norm solution
of a sparse underdetermined linear system arising from a discretization of a suitable boundary
value problem by either collocation or meshless finite differences...'
date: 2025-07-18
venue: 'Computer Methods in Applied Mechanics and Engineering'
paperurl: 'https://doi.org/10.1016/j.cma.2025.118199'
---
**Abstract:** We suggest a method for simultaneously generating
high order quadrature weights for integrals
over Lipschitz domains and their boundaries that requires neither meshing nor moment computation.
The weights are computed on pre-defined scattered nodes as a minimum norm solution
of a sparse underdetermined linear system arising from a discretization of a suitable boundary
value problem by either collocation or meshless finite differences. The method is easy to
implement independently of domain’s representation, since it only requires as inputs the
position of all quadrature nodes and the direction of outward-pointing normals at each node
belonging to the boundary. Numerical experiments demonstrate the robustness and high accuracy
of the method on a number of smooth and piecewise smooth domains in 2D and 3D, including
some with reentrant corners and edges. Comparison with quadrature schemes provided by
the state-of-the-art open source packages Gmsh and MFEM shows that the new method
is competitive in terms of accuracy for a given number of nodes.

Paper available in open access from the [publisher's website](https://doi.org/10.1016/j.cma.2025.118199)
