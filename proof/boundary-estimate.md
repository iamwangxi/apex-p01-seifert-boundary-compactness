# 5.1–5.5. Boundary estimate and Euclidean contradiction

Version 1.0 · 5 October 2026. [Overview](../README.md) · [Sources](../sources/bibliography.md)

## 5. Boundary curvature control and proof of P

The essential new step is an until-boundary curvature bound. It is proved for the exact-minimizer sequence using [§4](localization.md). The proof does not require a flat boundary metric, translations that are isometries, or a moving-metric version of Hass–Scott 6.9.

### 5.1 A boundary-centered quadratic area bound, without a density assumption

Let $`q\in\lambda_i=\partial F_i`$, let $`\rho=\mathrm{dist}_N(q,\cdot)`$, and write
```math
\mu_i(s)=\mathrm{Area}(F_i\cap B_N(q,s)),\qquad
\Theta_i(s)=\frac{\mu_i(s)}{s^2}.
```
All constants in this subsection are uniform in $`i`$ and $`q`$, for $`s\le s_0`$, because the ambient extension is fixed and the boundary curves form a smooth compact embedded family. Choose $`s_0`$ below their isolated-arc radius and the ambient injectivity radius.

The surface is minimal in $`N`$ away from its actual boundary. Apply its first-variation/divergence identity to $`X=\nabla(\rho^2/2)=\rho\,\partial_\rho`$ on $`F_i\cap B_N(q,s)`$. At almost every regular radius,
```math
2\mu_i(s)+O(s^2\mu_i(s))
=s\int_{F_i\cap\partial B_s}|\nabla_{F_i}\rho|
+\beta_i(s),
\quad
\beta_i(s)=\int_{\lambda_i\cap B_s}\langle X,\eta_i\rangle\,d\ell.
\qquad\text{(B2)}
```
Here $`\eta_i`$ is the unit outward surface conormal. The radial Hessian error is uniform over tangent planes and does not require a curvature bound on $`F_i`$.

Since $`\eta_i`$ is perpendicular to the boundary tangent, the tangential part of the radial vector makes no contribution. For a smooth curve through its center with uniformly bounded ambient curvature, the remaining part is $`O(\rho^2)`$. Also $`\mathrm{Length}(\lambda_i\cap B_s)\le Cs`$. Therefore
```math
|\beta_i(s)|\le Cs^3.
\qquad\text{(B3)}
```
In particular this bound does not require an angle bound or a half-plane density.

Coarea gives $`\mu_i'(s)=\int_{F_i\cap\partial B_s}|\nabla_{F_i}\rho|^{-1}`$. Combining this with (B2) and $`|\nabla_{F_i}\rho|\le1`$ yields
```math
s\mu_i'(s)-2\mu_i(s)\ge
-Cs^2\mu_i(s)-Cs^3,
\qquad
\Theta_i'(s)\ge-Cs\Theta_i(s)-C.
\qquad\text{(B4)}
```
These inequalities hold at regular radii and hence in their integrated, absolutely continuous form. Multiplication by $`e^{Cs^2/2}`$ and integration from $`s`$ to $`s_0`$, using $`\mu_i(s_0)\le a`$, give
```math
\mathrm{Area}(F_i\cap B_N(q,s))\le C_a s^2
\qquad(0\lt s\le s_0).
\qquad\text{(B5)}
```
This is an upper area-ratio bound; it neither fixes nor assumes the boundary density.

### 5.2 What an assumed curvature bound does give at a boundary

We need a local compactness observation **after** curvature point selection has supplied a curvature bound. It is not a boundary curvature estimate for the original sequence.

Suppose smooth minimal surfaces have $`|A|\le C`$ in a fixed relative neighborhood, their only actual boundary there is a single isolated smoothly controlled embedded arc, and their ambient metrics converge smoothly. At a point of the arc, use surface Fermi coordinates: $`s`$ is its arclength and $`t\ge0`$ runs along inward surface geodesics normal to it.

The intrinsic Gaussian curvature is bounded by the Gauss equation. The boundary geodesic curvature is at most the ambient curvature of the prescribed arc. The $`s`$-Jacobi field along the $`t`$-geodesics consequently stays close to its initial nonzero tangent on a uniformly small rectangle. The derivative of the inward conormal along the arc is bounded by its geodesic curvature and $`|A|`$. Along the $`t`$-geodesics the ambient acceleration and the rotation of the surface normal are bounded by $`|A|`$ and the ambient geometry.

Projection of this parametrized rectangle onto the surface tangent plane at its central boundary point thus has derivative within $`O(Cr)`$ of the identity, for a small fixed chart radius $`r`$. It is injective on a smaller rectangle and covers a fixed half-neighborhood bounded by the projected boundary arc. A short inward geodesic cannot meet that same arc again: its normal displacement is $`t+O(t^2)`$, whereas a displacement along the isolated boundary arc has normal part $`O(s^2)`$. It cannot meet a different actual boundary arc, by isolation. Thus the Fermi rectangle exists uniformly. This also excludes a premature global identification of the chart: its tangent-plane projection is bi-Lipschitz on the parameter rectangle.

The resulting graph has uniformly small slope and a uniform $`C^{1,1}`$ bound, the latter following from $`|A|`$ and the graph formula for second fundamental form. Its projected boundary and boundary trace are uniformly smooth. The stated Schauder input gives uniform $`C^k`$ bounds up to the arc on smaller charts. Interior points at fixed intrinsic distance from the actual boundary have the ordinary full graph version of the same argument.

This construction does not require transversality to any fixed ambient hypersurface: the graph is over the surface's **own** tangent plane. In particular it remains valid if the original angle with $`\partial M`$ tends to zero. It uses no reflection of the original metric. An area bound gives finite local sheet number: interior sheets not in the Fermi collar have full patches of positive area; sheets in the collar are accounted for by the single actual boundary arc. This yields local geometric extraction, possibly with interior multiplicity.

### 5.3 Weighted curvature point selection

Take a small generic rounded domain $`U`$ from §4 around a point of the limiting boundary leaf, and a protected smaller central neighborhood $`V`$. Let $`Y`$ be the artificial face, also including the parts of the physical face outside the central patch, and let $`d(x)=\mathrm{dist}_N(x,Y)`$. On $`V`$, $`d\ge d_0>0`$. This is fixed before any boundary convergence is known.

Suppose the curvatures in $`V`$ are unbounded. Select $`x_i\in F_i\cap U`$ maximizing $`d(x)^2|A_i(x)|^2`$, and put
```math
k_i=|A_i(x_i)|,\qquad d_i=d(x_i).
```
Then $`k_i d_i\to\infty`$, and
```math
|A_i(x)|\le2k_i
\quad\text{if }x\in F_i,\ \mathrm{dist}_N(x,x_i)\le d_i/2.
\qquad\text{(B6)}
```
Only points of the surface in the relative domain are intended in (B6); the ball may cross the ambient boundary in $`N`$.

Schoen's intrinsic interior estimate gives, for large $`i`$,
```math
\mathrm{dist}_{F_i}(x_i,\partial F_i)\le C_S/k_i.
\qquad\text{(B7)}
```
Indeed if the intrinsic distance were larger, use
$`\rho=\min\{\rho_0,\mathrm{dist}_{F_i}(x_i,\partial F_i)/2\}`$ in the estimate. Since $`k_i\to\infty`$, its bound forces (B7). Choose $`q_i\in\lambda_i`$ and an intrinsic path to $`x_i`$ of length at most $`(C_S+1)/k_i`$.

Rescale $`N`$ by $`k_i`$, centered at $`q_i`$. On every fixed ball the metrics converge to the Euclidean metric, the rescaled ambient manifold $`M`$ tends to a closed half-space $`H`$, and the actual boundary arcs tend smoothly to a single complete straight line $`L\subset\partial H`$. The artificial face goes to infinity. By (B6) the rescaled curvatures are at most 2 on every fixed ball for large $`i`$; at the rescaled $`x_i`$ they equal 1. By (B5) the whole rescaled surface has area at most $`C_aR^2`$ in every fixed radius-$`R`$ ball centered at $`q_i`$.

Apply §5.2 and interior graph extraction. Follow the bounded-length intrinsic path in (B7), rather than selecting unrelated Hausdorff components. It selects a connected smooth limiting surface $`D_\infty`$ containing the limit $`x_\infty`$ and the actual boundary line $`L`$, with
```math
|A_{D_\infty}(x_\infty)|=1.
\qquad\text{(B8)}
```
Continuation of these uniformly sized local charts makes the limit complete up to $`L`$: the artificial boundaries recede, and any finite intrinsic path can be continued unless it reaches the actual boundary. The whole actual boundary of this component is $`L`$, occurring once; a second copy would require a second boundary arc in an ambient bounded region, excluded by the isolated-arc property of $`\lambda_i`$.

The limit is embedded as a support. Transverse crossings would occur in the approximating embedded surfaces; touching ordered interior minimal graphs coincide by the maximum principle. The area bound is retained for this selected component:
```math
\mathrm{Area}(D_\infty\cap B_R)\le C_aR^2.
\qquad\text{(B9)}
```

The limit is not contained in $`\partial H`$, by (B8). The height above $`\partial H`$ is nonnegative and harmonic on the minimal limit. It is positive in the interior by the strong maximum principle, and the Hopf lemma at the smooth boundary charts makes the inward derivative positive along $`L`$. Thus $`D_\infty`$ is neat relative to the half-space. This obtains the angle in the blow-up limit; it does not assume a uniform angle for the original sequence.

### 5.4 Boundary multiplicity and simply connectedness of the blow-up

First anchor the multiplicity at $`L`$. In a chart of the neat nonflat limit, a boundaryless full graph sufficiently close to it would extend across the supporting plane into the outside of $`H`$. Such a graph cannot be approximated by surfaces contained in the inward side of the rescaled $`M`$. If its intrinsic distance to the actual boundary is small instead, §5.2 puts it in the Fermi collar of the unique actual arc. Hence there is one graph sheet on this limiting component near $`L`$. Interior sheet multiplicity is locally constant under the bounded-curvature smooth extraction, so connectedness propagates multiplicity one throughout $`D_\infty`$. This argument permits other limiting components, for example a plane in $`\partial H`$; they are not counted as sheets on the selected nonflat component.

The selected surface is proper. In a fixed compact ambient set, points a fixed intrinsic distance from $`L`$ have full graph patches of a fixed positive area; points near the actual boundary are in its finite collection of half-graph charts. A nonproper accumulation after an unbounded intrinsic journey would therefore produce infinitely many distinct patches and violate (B9). This is also the usual finite-sheet properness argument for bounded curvature and locally finite area.

We now prove simple connectedness; it is not inferred merely from the disks used in localization. Let $`\gamma`$ be a smooth embedded loop in $`\mathrm{Int}\,D_\infty`$. Multiplicity one, anchored at the boundary as just proved, gives a **closed** smooth lift $`\gamma_i\subset F_i`$ on the rescaled surfaces, converging smoothly to $`\gamma`$. Without that multiplicity step the lift might instead have nontrivial sheet monodromy, which would be inadequate.

In original units, $`\gamma_i`$ has length $`O(k_i^{-1})`$ and is inside the fixed domain $`U`$ for large $`i`$. It lies in a single component of $`F_i\cap U`$, which by §4 is a global least-area disk in $`N`$. Its unique subdisk $`E_i`$ is also a global Plateau minimum: a cheaper disk map could be inserted into that global minimizing disk, lowering its area. Hass–Scott 2.1 gives
```math
\mathrm{Area}(E_i)\le C\,\mathrm{Length}(\gamma_i)^2=O(k_i^{-2}).
```
Choose $`\epsilon_i=C_\gamma/k_i`$ large enough to contain $`\gamma_i`$ and exceed its length. Hass–Scott 3.2 puts $`E_i`$ in $`B_N(q_i,\epsilon_i)`$. After rescaling, its area, image diameter and curvature are bounded in a fixed ball.

For the topological filling we only need a continuous disk limit, not a new until-boundary derivative estimate. Parametrize $`E_i`$ conformally as least-energy disks, normalizing three separated boundary points of the fully controlled Jordan curves $`\gamma_i`$. Their energies are uniformly bounded. The Courant–Lebesgue estimate and short-loop confinement give equicontinuity in the interior, as in Hass–Scott 3.3. They also give equicontinuity on the entire boundary: a short source arc cannot map around almost the whole limiting Jordan curve because it contains at most one of the three fixed marks, whereas such a long image arc would contain at least two. Uniform smooth convergence to the embedded $`\gamma`$ then makes its image short. The half-disk version of short-loop confinement gives the corresponding neighborhood control, exactly the continuous part of the argument of Hass–Scott 3.5, p. 100. Here the **whole** Jordan curve is controlled, not just one possibly insufficient open-arc component.

Arzelà–Ascoli gives a continuous limit $`f:\overline{\mathbb D}\to\mathbb R^3`$, whose boundary is a weakly monotone degree-one parametrization of $`\gamma`$. In the interior $`f`$ is Euclidean harmonic. Indeed the rescaled harmonic map equations have Christoffel coefficients tending to zero uniformly on the fixed image ball; the energy bound makes their quadratic-gradient right-hand sides tend to zero in distributions. The uniform limit and weak $`W^{1,2}`$ convergence therefore give $`\Delta f=0`$.

All images lie in the limiting half-space. The boundary loop has strictly positive height, so harmonicity gives positive height throughout the disk. Its image consequently avoids $`L`$. The geometric limit there is a locally finite union of embedded minimal plaques; a continuous disk image in those plaques, attached along $`\gamma`$, stays on the selected leaf. Properness of that leaf excludes a limit switch to a different accumulating plaque. Thus $`f(\overline{\mathbb D})\subset D_\infty`$, and it supplies a nullhomotopy of $`\gamma`$. Its degree-one boundary parametrization is homotopic in $`\gamma`$ to its usual parametrization.

Every surface fundamental-group class is generated by such interior simple loops (loops may first be pushed off the boundary collar). Hence $`D_\infty`$ is simply connected. This proves the no-escaping-fillings assertion using exact disk minimality, rather than assuming that a pointed limit of disks is automatically a disk.

### 5.5 Euclidean reflection, one end, and the contradiction

Rotate $`D_\infty`$ by $`\pi`$ about $`L`$. This reflection is performed **only in the Euclidean blow-up**. Locally in conformal half-disk coordinates with $`L`$ the first coordinate axis, the two transverse coordinate functions have zero Dirichlet values. The longitudinal coordinate has zero normal derivative, by conformality. Extend the longitudinal coordinate evenly and the transverse coordinates oddly. They remain harmonic, the extension is conformal, and the nonzero boundary derivative supplied by the preceding Hopf argument excludes a branch. This proves the Schwarz extension here instead of assuming a reflection for the original warped collar.

Since the interior of $`D_\infty`$ lies in the open half-space, its rotated copy lies in the opposite open half-space. Their union $`\widehat D_\infty`$ is therefore smoothly embedded. Stability of the reflected double is not asserted or needed; the argument uses one-ended quadratic-growth rigidity. It is complete, properly embedded, and has no boundary. It has quadratic area growth by (B9), because balls centered at the origin on $`L`$ are invariant under the rotation.

The double is simply connected by van Kampen: both halves are simply connected and their overlap retracts to the line $`L`$. It is a connected noncompact surface without boundary, so surface classification makes it a plane topologically. In particular it has finite topological type and exactly one end. Anderson Corollary 1.5 therefore makes it a Euclidean plane geometrically. This contradicts (B8).

The assumed boundary curvature blow-up is impossible. A finite cover of the compact limiting longitude gives a uniform boundary curvature bound; Schoen controls the complement. This proves the until-boundary estimate required for the general sequence, without assuming a half-space rigidity theorem or any density value.


Continue with [global extraction and isotopy](extraction-and-isotopy.md).
