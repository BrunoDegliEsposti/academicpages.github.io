---
title: "Moment-free approximation of linear functionals"
collection: publications
category: wip
status: 'in preparation'
permalink: /publication/2025-09-09-moment-free-approximation-linear-functionals
excerpt: 'Joint work with [O. Davydov](https://oleg-davydov.de/).
In [previous work](/publication/2025-07-18-meshless-moment-free-quadrature),
we have introduced a way to overcome the moment computation
problem in the context of numerical integration. Our approach only requires
a single non-zero moment to be known, and in many cases leads to an
effectively *moment-free* numerical scheme.
In this talk, we generalize our moment-free approach to *any* linear functional,
provided that two conditions are met...'
date: 2025-09-09
slidesurl: '/files/DRWAA25-bruno.pdf'
---

**Abstract:** Consider the problem of approximating a bounded linear functional $$\Lambda$$ defined over a Banach space $$\mathcal{F}$$ by a linear combination of functionals $$\varphi_1,\dots,\varphi_N \in \mathcal{F}^*$$:
\\[
\Lambda \approx w_1 \varphi_1 + \dots + w_N \varphi_N = w^T\Phi,
\qquad
\Phi = (\varphi_1, \dots, \varphi_N)^T.
\tag{1}
\\]
This problem arises in numerical analysis when $$\Phi(f)$$ is known or can be evaluated easily for any $$f \in \mathcal{F}$$, but the value of $$\Lambda (f)$$ is unknown and much harder to compute. The problems of numerical integration, interpolation and differentiation can all be posed in this form.

The usual way to determine $$w$$ is to impose exactness of (1) over a finite-dimensional subspace $$\mathcal{S} \subset \mathcal{F}$$ spanned by generators $$s_1,\dots,s_M$$, which leads to a linear system for the weights. This simple approach is known as *moment-fitting*, and its main downside is that it requires $$\Lambda$$ to be evaluated over all generators when assembling the right-hand side of the system, a task potentially as hard as computing $$\Lambda(f)$$ itself. In earlier work [1], we have introduced a way to overcome the moment computation problem in the context of numerical integration. It only requires a single non-zero moment to be known, and in many cases leads to an
effectively *moment-free* approximation of $$\Lambda$$.

In this talk, we generalize our moment-free approach to *any* linear functional, provided that two conditions are met. First, there must be a natural way to include $$\Lambda$$ into an exact sequence of Banach spaces
\\[
\mathcal{U} \xrightarrow{\mathcal{A}}
\mathcal{F} \xrightarrow{\Lambda}
\mathbb{R} \xrightarrow{} 0.
\\]
Exactness of the sequence implies that $$\mathcal{A} u = f$$ has a solution $$u \in \mathcal{U}$$ if and only if the *compatibility condition* $$\Lambda (f) = 0$$ holds. Second, a linear numerical method must be available to discretize and solve the equation $$\mathcal{A}u = f$$ for compatible $$f$$. Given these, and a single function $$\hat{f} \in \mathcal{F}$$ for which $$\Lambda(\hat{f})$$ is known and different from zero, we propose the alternative linear system
\\[
A^T w = 0
\qquad
\Phi(\hat{f})^T w = \Lambda (\hat{f})
\\]
to determine weights $$w$$ suitable for the approximation (1), where matrix $$A$$ is the discretization of operator $$\mathcal{A}$$ introduced by the numerical method.

We present a characterization of the solvability of this system, as well as a priori bounds for the approximation error $$\vert \Lambda(f) - w^T \Phi(f) \vert$$. As an application, we show that on smooth two-dimensional domains this moment-free approach yields *positive* quadrature formulas of order two (up to a logarithmic factor) using Shortley--Weller grids as quadrature nodes. Furthermore, we establish the existence of stable quadrature formulas of order 3, also up to a logarithmic factor.

**References:** \[1\] Davydov, O., & Degli Esposti, B. (2025).
*Meshless moment-free quadrature formulas arising from numerical differentiation.*
Computer Methods in Applied Mechanics and Engineering, 445, 118199.

I have recently given a talk on this topic at the DRWAA 2025 workshop
in Alba di Canazei, Italy. Slides are available for download.