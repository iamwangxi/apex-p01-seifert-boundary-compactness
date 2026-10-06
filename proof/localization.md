# 2–4. Statement, inputs and exact disk localization

Version 1.0 · 5 October 2026. [Overview](../README.md) · [Sources](../sources/bibliography.md)

## 2. Setting and Lemma P

Let $`M=E(K)`$ be the compact irreducible orientable exterior of a nontrivial knot. Give it a fixed smooth metric with the strictly convex collar permitted by competition §3, equation (2), p. 6:

```math
g=dr^2+\phi(r)^2g_T,\qquad \phi(0)=1,\quad \phi'<0
```

on a sufficiently small inward collar. No flatness of $`g_T`$ is assumed in Lemma P. Let $`J`$ be the compact smooth leaf family of embedded preferred longitudes on $`\partial M`$. The family has uniform curvature and higher derivative bounds and a uniform isolated-arc radius. These are the boundary-geometry properties used below.

All surfaces considered here are connected, orientable, smooth, properly and neatly embedded, incompressible, and have one boundary circle. Neat means transverse to the ambient boundary. Incompressibility is used as $`\pi_1`$-injectivity, equivalently the loop-theorem formulation in this setting. An **exact fixed-boundary relative minimizer** attains the least area among smooth neat embeddings in its own smooth relative ambient isotopy class, fixing its prescribed boundary pointwise. This definition does not assert minimization among all maps.

**Lemma P.** Fix a genus $`h`$ and an area bound $`a`$. Let $`F_i`$ be exact fixed-boundary relative minimizers as above with $`g(F_i)=h`$, $`\mathrm{Area}(F_i)\le a`$ and $`\partial F_i\in J`$. A subsequence converges smoothly up to the boundary, modulo reparametrization of the compact source surface, to a smooth neat embedded surface $`F_\infty`$ whose boundary is a leaf of $`J`$. The subsequence is eventually properly isotopic to $`F_\infty`$; by smooth isotopy extension the isotopy is ambient and preserves $`\partial M`$ setwise. If the prescribed boundary curve is the same throughout, the final isotopy fixes it pointwise.

The limit is incompressible, orientable and of genus $`h`$ by this final isotopy, and areas converge. It also attains the minimum in its own fixed-boundary relative class. The proof uses incompressibility and exact minimality rather than a separate genus estimate. It assumes the exact minimizers already exist. The [applications](consequences.md) declare their separate fixed-boundary attainment input.

## 3. Inputs and source status

Pinpoint citations refer to the editions in the [bibliography](../sources/bibliography.md). The following standard statements are used in the indicated forms; an original source not checked is explicitly distinguished from a locally checked statement.

1. **Plateau existence, boundary regularity and embeddedness.** A smooth Jordan curve bounding a finite-area disk in a closed or homogeneously regular Riemannian manifold has a Plateau-area-minimizing disk, with a conformal least-energy parametrization. In a compact 3-manifold with strictly convex boundary, such a disk with smooth Jordan boundary on the ambient boundary is properly embedded; disks with disjoint boundary curves are disjoint. These are the Morrey and Meeks–Yau forms recorded by Hass–Scott, Theorems 2.7 and 2.9, pp. 94–96. The original Morrey and Meeks–Yau papers were not separately checked.

2. **Interior monotonicity, with the center on the disk.** In a fixed compact smooth ambient extension $`N`$, there are $`c>0`$ and $`\rho_0>0`$ such that, if $`D`$ is a minimal disk, **$`x`$ belongs to the image of $`D`$**, and $`\partial D`$ is disjoint from $`B_N(x,\rho)`$, then

   $`\displaystyle \mathrm{Area}(D\cap B_N(x,\rho))\ge c\rho^2, \qquad 0<\rho\le\rho_0.`$

   Parametrized area is intended before embeddedness is known. Only interior balls in $`N`$ are used. This is standard minimal-surface monotonicity; Hass–Scott Lemma 2.3, p. 92, explicitly records the on-disk center condition for least-area disks, which are the disks used in the confinement argument. Lawson's original monotonicity source was not checked. The displayed on-disk condition corrects the sole wording issue identified in the fresh-context review.

3. **Interior stability.** In a fixed smooth ambient 3-manifold of bounded geometry, there are $`\rho_0,C>0`$ such that a two-sided stable minimal surface with an intrinsic ball of radius $`2\rho`$ about $`p`$ disjoint from its actual boundary satisfies $`|A|^2(p)\le C\rho^{-2}`$ for $`\rho\le\rho_0`$. Interior derivative estimates give smooth finite-sheet extraction on smaller patches under an area bound. This is the Schoen interior estimate; the original 1983 chapter was not checked. Hass–Scott's remark on p. 99 records the interior curvature consequence for exact disks. No boundary estimate is obtained from this input alone.

4. **Relative disk isotopy and extension.** Properly embedded disks with the same boundary in an irreducible smooth 3-manifold are isotopic relative to that boundary after their incoming collars are matched. A disjoint system is treated by cutting successively along disks. The necessary innermost-disk and ball argument is given in §4.3 below. Hatcher's three-manifold notes, pp. 1 and 20, record the smooth category, isotopy extension and the ball case; those pages are not represented as a proof of the full general relative statement.

5. **Short-loop comparison and confinement.** Hass–Scott Lemma 2.1, p. 91, supplies a spanning disk with area at most $`C\,\mathrm{Length}(\gamma)^2`$ for a curve in a sufficiently small coordinate ball. Lemma 3.2, pp. 96–97, says that, for sufficiently small $`\epsilon`$, if a closed curve has length less than $`\epsilon`$ and lies in $`B_N(x,\epsilon)`$, every global least-area disk spanning it lies in that ball. These are used only after the surface subdisks have been proved to be global minima. The continuous equicontinuity mechanism is in Lemma 3.3, pp. 97–99, and the proof of Lemma 3.5, p. 100.

6. **Euclidean rigidity.** Anderson Corollary 1.5, p. 96: a complete embedded minimal surface in $`\mathbb R^3`$, of finite topological type, with quadratic area growth and one end, is a plane. All these hypotheses are established for the reflected limit in §5.5; no half-space classification or stability of the double is assumed.

7. **Graph regularity and interior extraction.** A uniformly $`C^{1,1}`$ graph satisfying a smooth uniformly elliptic minimal graph equation, on uniformly smooth domains with uniformly smooth Dirichlet data, has uniform $`C^{2,\alpha}`$ bounds on smaller closed boundary patches and then uniform $`C^k`$ bounds for every fixed $`k`$. Write the equation in nondivergence form, apply boundary Schauder to its uniformly $`C^\alpha`$ coefficients, and bootstrap. Gilbarg–Trudinger, second edition (1983), Chapter 6, is used at standard-statement level; the original book and exact pages were not checked. Anderson's interior bounded-curvature compactness statement on p. 96 was checked in the supplied proof investigation. The extension to a boundary arc is proved in §5.2, not read into the interior statement.

8. **Topology of the reflected surface.** The simply connected special case of van Kampen is Hatcher, *Algebraic Topology*, Theorem 1.20, p. 43: two simply connected path-connected open sets with path-connected intersection have simply connected union. The halves are thickened by collars. Classical surface classification then says that a connected simply connected noncompact surface without boundary is a topological plane. Richards (1963) is a standard source; its original was not checked.

For comparison only, Anderson Theorem 2.3, p. 99, gives a boundary curvature theorem for an embedded minimal **disk** with controlled full Jordan boundary in a convex domain. It is not applied here to artificial cut curves with uncontrolled derivatives or to arbitrary stable surfaces. Hass–Scott Lemmas 6.9 and 6.11, p. 112, give fixed-arc geometric convergence of exact disks; they are not needed as a moving-metric boundary compactness assertion in this proof.

## 4. General localization for smooth exact minimizers

This section does not require a flat torus or a linear foliation. Its conclusion will be used in the [boundary estimate](boundary-estimate.md).

### 4.1 Smooth strictly convex replacement balls and global comparison disks

Extend $`M`$ isometrically across its boundary into a closed smooth Riemannian 3-manifold $`N`$. Only a fixed small neighborhood of $`M`$ is relevant; a smooth collar extension followed by any smooth completion suffices. No reflected metric, reflection of the original longitude, or reflection of an original surface is used.

At $`p\in\partial M`$, start with outward signed distance $`d=-r`$. Strict convexity makes the tangential Hessian of $`d`$ positive definite at the boundary. Replacing it by $`u=d+Cd^2`$, with $`C`$ large, and shrinking the coordinate neighborhood, makes $`\mathrm{Hess}\,u`$ positive definite in a fixed neighborhood. In that neighborhood $`M=\{u\le0\}`$.

Set $`v_R(x)=\mathrm{dist}_N(p,x)^2-R^2`$, for small $`R`$. Both $`u`$ and $`v_R`$ have positive definite Hessians on a fixed larger coordinate ball. Let $`\theta_\epsilon`$ be a smooth even convex approximation to absolute value, equal to absolute value for $`|t|\ge\epsilon`$, with $`\theta_\epsilon\ge |t|`$ and $`|\theta_\epsilon'|\le1`$. Define
```math
w_{R,\epsilon}
=\frac{u+v_R+\theta_\epsilon(u-v_R)}2,
\qquad U=\{w_{R,\epsilon}\le0\}.
```
Its Hessian is
```math
\frac{1+\theta_\epsilon'}2\mathrm{Hess}\,u
+\frac{1-\theta_\epsilon'}2\mathrm{Hess}\,v_R
+\frac{\theta_\epsilon''}2\,d(u-v_R)\otimes d(u-v_R).
```
Thus $`U`$ is a smooth strictly convex rounded half-ball, contained in $`M\cap B_N(p,R)`$, and its central boundary patch agrees exactly with $`\partial M`$. For sufficiently small $`\epsilon\ll R^2`$, the two outward normals at the old corner are not opposite, so the zero level is regular. A prescribed smaller relative neighborhood of $`p`$ is retained.

There is an area bound $`\mathrm{Area}(\partial U)\le C_0R^2`$, uniform in the rounding width. One way to see it is to use normal coordinates. The Euclidean Hessians remain positive for small $`R`$, so $`U`$ is Euclidean convex and contained in a radius-$`R`$ ball. Divide its outward normals among six signed coordinate directions having component at least $`1/\sqrt3`$. Each corresponding projection is injective, its projected area is at most $`\pi R^2`$, and metric comparison gives the bound. Interior balls use the ordinary squared-distance defining function.

For any cut Jordan curve $`\gamma\subset\partial U`$, a cap on the sphere $`\partial U`$ has area at most $`C_0R^2`$. Minimize its Plateau area **in $`N`$**, obtaining $`D_\gamma`$. This distinction matters: an old disk in the surface might initially leave $`U`$, so minimizing only in $`U`$ would not give the needed comparison.

Choose once a larger coordinate neighborhood on which $`w_{R,\epsilon}`$ is strictly convex. If the global minimizing disk left it, a point a fixed positive distance from the small boundary curve would contribute a fixed positive area by interior monotonicity. For small enough $`R`$ this contradicts the cap upper bound. The disk is therefore in that coordinate neighborhood. Subharmonicity of $`w_{R,\epsilon}`$ on its conformal minimal parametrization and the boundary value zero put the entire disk in $`U`$.

Meeks–Yau embeddedness and disjointness now apply in $`U`$. Smoothness at the cut curve is supplied by Plateau boundary regularity in the stated disk input. Neatness there can also be checked without a branch-point assumption: apply the Hopf lemma to $`-w_{R,\epsilon}\circ f`$, which is positive in the disk and zero on its boundary; its inward derivative is nonzero, and conformality then gives rank two for $`df`$. Hence all comparison disks for disjoint cut curves are embedded and pairwise disjoint. Their interiors are in $`\mathrm{Int}\,U`$, and they minimize area not just in $`U`$, but among all Plateau disk competitors in $`N`$. In particular their areas are at most the areas of the original surface disks, wherever those disks lie.

### 4.2 The outermost disks and the retained surface

Choose the domain generic for the extended neat surface $`F`$. Its intersection with $`\partial U`$ is a finite disjoint system of smooth Jordan curves. If $`U`$ meets the prescribed boundary in one small arc, exactly one cut curve contains that arc. The other cut curves are interior curves on $`F`$.

For a countable sequence, one common generic radius is available. Keep a rounding width fixed over a small radius interval preserving the protected core. Wherever the spherical term has positive weight, $`\partial_Rw=-2R`$ times that weight is nonzero. Wherever that weight is zero, $`\partial U`$ is the original boundary and the extended neat surfaces are already transverse to it. Parametric transversality and a countable intersection of full-measure sets therefore give a common radius. This is transversality of the individual input surfaces, not a bound on the resulting artificial curves.

Every cut curve is null-homotopic in $`M`$, since it lies on the boundary sphere of $`U`$. Incompressibility makes every interior curve bound its unique disk in $`F`$, the disk not containing the original boundary. For the cut curve sharing a boundary interval, push that interval slightly into $`F`$, apply the same null-homotopy argument, and restore the strip. This gives the boundary-attached disk bounded by the original curve. Choose the maximal, or outermost, disks $`D_1,\dots,D_m`$; nested disks are included in an outermost one.

Their retained complement $`C`$ is connected and contains the original boundary outside $`U`$. Its interior contains no cut curve. Since it contains points outside $`U`$, connectedness puts all of $`C`$ outside $`\mathrm{Int}\,U`$. This proves that the new comparison disks miss the retained surface. It does **not** yet assert that the old disks lie inside $`U`$.

### 4.3 Relative isotopy and an area approximation for this particular splice

Replace the outermost disks by their comparison disks, producing the embedded raw surface
```math
P=C\cup D'_1\cup\cdots\cup D'_m.
```
It has the same prescribed boundary and
```math
\mathrm{Area}(P)
=\mathrm{Area}(F)-\sum_j\mathrm{Area}(D_j)
+\sum_j\mathrm{Area}(D'_j)
\le\mathrm{Area}(F).
\qquad\text{(L1)}
```

Here are the class and smoothing justifications needed to compare it with the smooth minimum.

First match the old and new neat boundary collars in an arbitrarily thin strip along their shared portion of the prescribed boundary. This can be done with area error tending to zero: both graph functions have the same trace, so their difference is $`O(r)`$; a cutoff at width $`\delta`$ has derivative $`O(\delta^{-1})`$, and the interpolated graphs have bounded first derivatives for this fixed configuration on a strip of area $`O(\delta)`$. In coordinates $`(x,y,r)`$ with that boundary $`y=r=0`$, both are smooth graphs $`y=g(x,r)`$. Interpolate in those graph coordinates, fixing $`r=0`$, and make the transition in a thin strip. For this fixed finite configuration, its area cost tends to zero with the strip width. After the collars match, trimming their common collar reduces the qualitative comparison to interior disk replacements, with a smooth retained surface and closed disk boundaries. Thus no cusped exterior piece is being assumed to be a neat smooth subsurface at its flat-transition endpoint.

Cut $`M`$ along the retained surface. This cut manifold is irreducible: an interior sphere bounds a ball in $`M`$, and the connected retained surface, being disjoint from the sphere and reaching $`\partial M`$, is outside that ball. The ball therefore remains in the cut manifold. Old and new disks are proper disks there with the same boundaries after their incoming collar germs are identified. At every artificial cut curve both incoming disk rays enter the $`U`$-side, whereas the retained ray is outside $`U`$; they can be rotated into alignment without crossing that retained ray. Thus the two boundaries lie on the same boundary curve of the cut manifold, rather than on different copies of the cut surface. Matching their collars, put them in general position. An innermost intersection circle gives an embedded sphere made from two subdisks; the sphere bounds a ball. Pushing a subdisk across this ball removes that circle and any nested ones. The retained surface is fixed in the cut manifold. After all circles are removed, the sphere between the two disks bounds a ball, giving the final relative disk isotopy. Cut successively along disks to perform the disjoint-system version. Restoring the common boundary collar proves that the replacement preserves the relative class after smoothing.

The actual raw splice has finite locally Lipschitz graph charts. Away from the ambient boundary, project along the cut-curve coordinate and the signed normal to $`\partial U`$; transversality of the old sheet and neatness of the new disk give common graph charts on opposite sides. At a transition on the ambient boundary, the projection to $`(x,r)`$ is invertible on both neat sheets. If the cut curve projects to $`r=h(x)`$, $`h\ge0`$, the joined graph has the form
```math
g(x,r)=g_o(x,r)+\max\{r-h(x),0\}\,b(x,r),
```
with $`b`$ smooth locally, because the two smooth graphs agree on the cut curve. Its trace on $`r=0`$ is the prescribed trace. This is a Lipschitz graph even when the retained strip is cuspidal.

Odd extension of the zero-trace residual in $`r`$, followed by convolution with an even kernel and cutoffs, gives smooth graphs with the same trace. Interior charts use ordinary convolution. Convergence is uniform and in $`W^{1,1}`$, with bounded first derivatives for this fixed configuration, so graph areas converge. A finite sequential chart procedure smooths the whole seam. For a fixed index, use an enlarged chart whose smaller core contains only the selected local graph; the remaining pieces of the compact embedded surface have positive clearance from that core. Distinct selected sheets also have positive clearance. Choose the smoothing widths and supports below these clearances. Graph interpolation and smooth isotopy extension, together with the preceding disk moves, keep the smoothed surface in the original smooth relative class.

Consequently, for every $`\eta>0`$ there is a smooth neat relative competitor $`P_\eta`$ with
```math
\mathrm{Area}(P_\eta)\le\mathrm{Area}(P)+\eta.
\qquad\text{(L2)}
```
No estimate uniform over a sequence is needed for (L2). The width can depend on the fixed surface and on $`\eta`$. Nor is (L2) an area-density theorem for arbitrary surfaces in competition Definition A.1. It applies only to these explicit graph splices.

### 4.4 Exactness forces the original pieces to be global least-area disks

Since $`F`$ is an exact minimum in the smooth relative class, (L1)–(L2) imply
```math
\mathrm{Area}(F)\le\mathrm{Area}(P)\le\mathrm{Area}(F).
```
Each summand $`\mathrm{Area}(D_j)-\mathrm{Area}(D'_j)`$ is nonnegative, so each is zero. Thus every original outermost disk $`D_j`$ itself attains the global Plateau minimum in $`N`$ for its boundary.

Apply the cap area bound, interior monotonicity and the convex-function confinement from §4.1 to the **original** disk $`D_j`$. It lies in $`U`$, and its interior is in $`\mathrm{Int}\,U`$. Therefore the components of $`F\cap U`$ are precisely these disks, and they are exact least-area disks in $`N`$, hence in $`U`$.

This establishes the local disk property from exact relative isotopy minimality. It did not assume that property from stability, and did not assume that an arbitrary isotopy minimum was already a homotopy minimum.
