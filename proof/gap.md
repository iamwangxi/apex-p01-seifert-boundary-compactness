# 1. The compactness input and its boundary gap

Version 1.0 · 5 October 2026. [Overview](../README.md) · [Sources](../sources/bibliography.md)

**The cited theorem controls a fixed interior truncation; the application requires convergence at the original boundary.** The repair in this repository proves boundary compactness for smooth exact fixed-boundary relative area minimizers, and deduces the two smooth applications with a declared fixed-boundary existence input. It does not prove compactness of every stable surface in Kapovich's space.

## 1.1 Target and dependence on compactness

The target is Apex Intelligence, *Contractibility of the complex of incompressible Seifert surfaces: the knot case of Kakimizu's problem*, official competition version, 11 September 2026, 48 pages, PDF SHA-256 `34f17d7d99780d3fd3626d9e5d7b35d6aa76661c404f191b6df341b300c0c06f`.

Theorem A uses a well-ordered complexity. Competition §3, Theorem 3.3, printed p. 7, names the compactness and finite-isotopy-block input $`(\mathrm{Fin})`$: Kapovich's appendix to Schultens, *J. Topol.* **3** (2010), Proposition A.1 and Corollary A.3. Competition Lemma 4.8(i), §4.3, p. 11, selects sliding-boundary minimizers using $`(\mathrm{E})(ii)`$ and then uses $`(\mathrm{Fin})`$ to prove finiteness of

```math
\{v\in IS(K)^{(0)}:g(v)=h,\ A(v)\le a\}.
```

Clauses (ii)–(iv) derive the sparsity and well-ordering of complexity values and countability from this finiteness. Theorem A.6, §A.4, p. 27, also invokes $`(\mathrm{Fin})`$ to extract a limit and keep it in the required isotopy class. Theorem 3.2(ii), p. 7, cites Kapovich Corollary A.4 for sliding attainment; that corollary depends on Proposition A.1.

The later author version is G. Pan, C. You, J. Zhou and Y. Chen, *Exchange complexes and contractibility of the complex of incompressible Seifert surfaces*, arXiv:2609.09224v2, 12 September 2026. Its Theorem 2.16, pp. 22–23, still uses Kapovich Proposition A.1 and Corollary A.3 after fixed-boundary minimization. Its well-foundedness Lemma 4.2, pp. 31–32, still uses the finite isotopy-block conclusion. That version does not remove the particular compactness dependence considered here.

## 1.2 Anderson's precise setting and output

Anderson, *Curvature estimates for minimal surfaces in 3-manifolds*, **18** (1985), Theorem 3.1, pp. 101–102, works in a strictly convex-domain setting with a convex defining function $`f`$; §1 and Lemma 1.2, p. 93, set up this condition. In §3 one considers embedded minimal surfaces $`\widehat\Sigma_i`$ in $`\Omega`$, with original boundary in $`\partial\Omega`$, and **one fixed** $`\varepsilon>0`$. The surfaces to which the convergence conclusion applies are

```math
\Sigma_i=\widehat\Sigma_i\cap\Omega_{-\varepsilon},
\qquad
\Omega_{-\varepsilon}=f^{-1}(( -\infty,-\varepsilon]).
```

The truncations $`\Sigma_i`$ must be connected, diffeomorphic to a fixed surface of Euler characteristic $`n`$, and have uniformly bounded areas. The alternatives are smooth convergence of these truncations to an embedded minimal surface of the same topological type, or varifold convergence of the truncations to an embedded minimal surface of Euler characteristic at least $`n/2`$, counted with multiplicity at least two, with smooth convergence away from finitely many points.

These are conclusions about fixed-depth truncations, not smooth convergence up to the original boundary of $`\widehat\Sigma_i`$. The original/truncated symbols are distinct in the printed statement; text extraction can obscure the distinction.

## 1.3 Kapovich's use

Kapovich Proposition A.1, pp. 897–898, asserts compactness for full stable embedded minimal surfaces of bounded area whose boundaries range in a compact smooth family $`J`$. Its proof invokes Anderson Theorem 3.1 to obtain a limiting surface with boundary in $`J`$, then treats the exceptional points as interior points and uses Schoen's stability estimates to eliminate them. It concludes smooth convergence of the full parametrized surfaces to a covering, and uses the boundary to rule out nontrivial covering degree.

The first step already needs control at the original boundary. Anderson's fixed-depth conclusion does not supply it: interior estimates on a truncation do not control a collar omitted by that truncation. Fixed topology of the full surfaces also does not by itself verify connectedness and fixed topology of the truncations, and strict convexity of the ambient boundary is not a substitute for checking the defining-function setting. The output mismatch alone suffices to identify the missing step.

The locally checked preprint is arXiv:0707.3926v4, Proposition 9, p. 19, with setup on p. 18; Corollaries 10 and 11, pp. 19–20, correspond to the journal's isotopy-block and attainment consequences. The journal proof on pp. 897–898 agrees word for word with this preprint proof; both were compared directly. This is a proof-input gap, not a claim that Proposition A.1 or Theorem A is false.

## 1.4 A weak collar function does not change the output

Competition §3, equation (2), p. 6, permits the inward collar metric

```math
g=dr^2+\phi(r)^2g_T,
\qquad \phi(0)=1,\quad\phi'(0)<0.
```

Equation (3), p. 6, gives $`\mathrm{Hess}\,r=\phi\phi'g_T<0`$ in tangential directions. A smooth function $`q(r)`$ with $`q(0)=0`$, $`q'\le0`$ and $`q''\ge0`$ may be flattened to a negative constant in the interior. Then

```math
\mathrm{Hess}(q(r))=q''\,dr^2+q'\,\mathrm{Hess}\,r\ge0.
```

This is a weak convex function useful for some topology arguments. It neither supplies a boundary curvature estimate nor upgrades a fixed-depth convergence statement to convergence at the original boundary. Anderson Theorem 2.2, pp. 98–99, also has a strictly convex defining-function hypothesis. This repair uses neither Theorem 3.1 nor Theorem 3.2 as a shortcut to full boundary compactness.

Continue with the [precise statement, inputs and localization](localization.md).
