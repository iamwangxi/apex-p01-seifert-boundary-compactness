# 5.6–5.7. Global extraction, covering degree and isotopy

Version 1.0 · 5 October 2026. [Overview](../README.md) · [Sources](../sources/bibliography.md)

The [boundary estimate](boundary-estimate.md) and [localization](localization.md) are the inputs to this final part of Lemma P.

### 5.6 Global geometric extraction

Exact smooth relative minima are two-sided stable minimal surfaces in their interiors. They can be regarded as minimal surfaces in the fixed smooth extension $N$. Every compactly supported variation away from their actual boundary is admissible for sufficiently small time: its support in the surface has positive distance from the ambient boundary. Thus stability is available in $N$ at interior points. The distance restriction is to the **surface's own boundary**, not an artificial assertion that every ambient ball must be contained in $M$.

The preceding argument supplies a uniform curvature bound in a neighborhood of the entire compact limiting longitude. Schoen's estimate controls the complement. Thus the curvatures of the full surfaces are uniformly bounded. The graph construction of §5.2, now without any rescaling, supplies full and half-graph charts, and Schauder gives smooth extraction on smaller patches. The area bound gives finite local sheet number; patches close in intrinsic distance to the actual boundary lie in its single Fermi collar, and the others have full graph patches of uniformly positive area. Choose common subsequences in a finite cover and diagonalize for derivatives. Overlapping local limits agree as geometric limits of the same surfaces.

After passing to a subsequence, the boundary leaves converge smoothly to one leaf $\lambda_\infty$. The result is a compact embedded minimal support $\Sigma$, possibly initially with interior multiplicity. Transverse crossings cannot appear as limits of embedded graphs; tangential coincident sheets have the same support by the strong maximum principle. Local finiteness and the finite-area properness argument of §5.4 make the support compact. Interior contact with $\partial M$ is excluded by (P1). Its actual boundary is $\lambda_\infty$; uniqueness of the local boundary sheet is checked after neatness below.

The boundary graph is neat without a prior angle bound. For the smooth limit, in the original warped collar,
$$
\Delta_\Sigma r
=\frac{\phi'}{\phi}\bigl(2-|\nabla_\Sigma r|^2\bigr)<0.
\qquad\text{(P1)}
$$
Thus an interior zero of $r$ is impossible. The Hopf lemma on the smooth boundary half-chart gives a positive inward derivative at $r=0$. Neatness, and hence a uniform positive angle on the extracted compact subsequence, is a conclusion. This computation uses the original collar only as a barrier, not as a reflection geometry.

An additional boundaryless full limiting graph cannot touch $\partial M$, by the interior minimum contradiction in (P1). Once the actual boundary graph is neat, any extra approximating sheet following it near the edge either has a full chart extending outside $M$, or is in the Fermi collar of the unique actual boundary curve. The former is impossible and the latter is the already identified single boundary chart. Thus the boundary sheet is unique, by the same argument as §5.4. This does not exclude interior multiplicity until the global covering step.

The support is connected. Otherwise its finitely many compact components have disjoint small neighborhoods. Full geometric convergence puts all of each connected $F_i$ in their union for large $i$, and the boundary puts it in the component containing the longitude. It cannot also approximate another component. Thus there is no extra closed component detached from the boundary component.

### 5.7 Multiplicity one and the final proper isotopy

Use a transverse line bundle $L$ to $\Sigma$ adapted to the boundary: along $\partial\Sigma$, its line lies in $T\partial M$ and is transverse to the longitude. Extend it over $\Sigma$, and take a small tubular embedding whose fibers over the boundary stay in $\partial M$, with all other fibers in the interior. This follows directly by using neat collar coordinates near the boundary and a transverse tubular bundle elsewhere. It works before an orientation of $L$ has been selected.

Full geometric smooth convergence puts $F_i$ inside this tube and makes it transverse to all the fibers. Its projection
$$
\pi_i:F_i\longrightarrow\Sigma
$$
is a proper local diffeomorphism of manifolds with boundary, and hence a covering. Its image is open and closed, so it is onto the connected support. Moreover $\pi_i^{-1}(\partial\Sigma)=\partial F_i$, since boundary fibers lie in the ambient boundary. The nearby longitude is a single graph over $\lambda_\infty$ in the boundary tube, so every point of $\partial\Sigma$ has one preimage. The covering has degree one.

This proves multiplicity one, including exclusion of a one-sided double-cover limit. It is stronger and more specific than asserting, without a covering argument, that a nontrivial covering must restrict nontrivially to every boundary component.

Consequently $F_i$ are single graph sections $s_i$ of $L$, tending smoothly to zero. Scaling $s_i$ to zero gives a smooth proper isotopy to $\Sigma$. The boundary remains in $\partial M$; the isotopy need not remain leaf-constrained at intermediate times. The boundary-adapted vector field construction extends it to an ambient isotopy preserving $\partial M$. If all the boundary curves were identical, the graph sections vanish there and the isotopy fixes that boundary pointwise.

This proves P. Area converges smoothly as well. The limit is incompressible, of genus $h$, and orientable, since it is isotopic to the late terms.

The limit is also an exact minimum in its own fixed-boundary relative class, if that closure property is wanted. The graph isotopies have ambient extensions $H_i\to\mathrm{id}$ smoothly with $H_i(\Sigma)=F_i$. For any smooth neat competitor $G$ isotopic to $\Sigma$ relative to its boundary, $H_i(G)$ is a relative competitor for $F_i$. Hence
$$
\mathrm{Area}(F_i)\le\mathrm{Area}(H_i(G))
\longrightarrow\mathrm{Area}(G),
$$
and area convergence gives $\mathrm{Area}(\Sigma)\le\mathrm{Area}(G)$. This does not require universal disjointness.



The [consequences](consequences.md) follow from Lemma P and the declared fixed-boundary attainment input.
