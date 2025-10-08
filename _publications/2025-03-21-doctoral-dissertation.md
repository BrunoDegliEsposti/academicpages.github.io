---
title: "Domain discretization and moment-free quadrature for meshless methods"
collection: publications
category: dissertation
permalink: /publication/2025-03-21-doctoral-dissertation
excerpt: 'This dissertation addresses two fundamental challenges
in meshless numerical methods: robust node generation for
real-world 3D domains, including CAD geometries,
and high-order numerical integration on scattered nodes.
The results in Chapters 4 and 5 have been expanded and
[published](/publication/2025-07-18-meshless-moment-free-quadrature).
The results in the other chapters are being split
into two papers, and will be submitted to peer-reviewed journals
in the upcoming months.'
date: 2025-03-21
venue: 'Florence'
thesisurl: 'https://hdl.handle.net/2158/1417355'
---

**Abstract:** Meshless methods are a versatile class of numerical techniques that discretize computational domains using scattered, unstructured nodes, avoiding the complexities and limitations of conventional mesh generation. These methods are especially well-suited for problems involving complex geometries and dynamic phenomena such as free boundaries, large deformations, and crack propagation, where traditional meshing approaches often become computational bottlenecks. This thesis addresses two fundamental challenges in the meshless paradigm: robust node generation for real-world 3D domains, and high-order numerical integration on scattered nodes. First, we propose a fully meshless advancing front node generation algorithm tailored for 3D domains described in the B-rep (boundary representation) format, the standard used in Computer-Aided Design (CAD). Our algorithm efficiently converts trimmed NURBS surfaces into variable-density point clouds that sample both the interior and boundary of the domains. The method operates hierarchically by progressively advancing a front over lower-dimensional entities (edges and faces) before higher-dimensional ones (volumes), and incorporates a novel meshless inclusion test that prevents nodes from being placed outside the domain of interest, even in the case of piecewise smooth boundaries. The algorithm is shown to perform effectively on complex 3D geometries, producing well-distributed node configurations suitable for numerical simulations using meshless finite difference methods. Second, we introduce a novel approach to numerical integration by simultaneously generating high-order quadrature weights for integrals over Lipschitz domains and their boundaries without relying on meshing or the computation of moments (integrals of basis functions). The weights are obtained on given scattered nodes as a minimum norm solution of a sparse underdetermined linear system arising from a discretization of a suitable boundary value problem. This discretization is achieved using either tensor-product B-spline collocation or meshless finite differences, such as those based on polyharmonic radial basis functions (RBF-FD). The proposed moment-free method is easy to implement, and does not depend on the domain’s representation (parametric or implicit), since it only requires as inputs the position of all quadrature nodes and the direction of outward-pointing normals at each node belonging to the boundary. Comprehensive numerical experiments demonstrate the robustness and high accuracy of the method on a number of smooth and piecewise smooth domains in 2D and 3D, including some with reentrant corners and edges. Together, the contributions presented in this thesis advance the state of the art in meshless methods by addressing critical challenges in node generation and numerical integration, and by providing robust tools for challenging real-world applications involving complex geometries and high-order accuracy requirements.

Dissertation available in open access from the
[official archive](https://hdl.handle.net/2158/1417355)
of the University of Florence.
