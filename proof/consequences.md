# 6–8. Consequences, input levels and limits

Version 1.0 · 5 October 2026. [Overview](../README.md) · [Sources](../sources/bibliography.md)

**Lemma P and smooth fixed-boundary attainment give bounded-complexity finiteness and smooth sliding-boundary attainment without using either sliding attainment or general stable-surface compactness as an input.**

## 2.2. Separate fixed-boundary existence input

Lemma P assumes exact minimizers already exist; its proof does not invoke an existence theorem for the full surfaces. For the applications, accept arXiv:2609.09224v2, Theorem 2.6, p. 8, as an external smooth neat fixed-boundary attainment theorem. The printed scope is a flat boundary torus, linear longitude foliation and the exact $\phi=1-r$ collar in v2 §2.1, pp. 5–6. Choose these data, permitted by competition §3, equation (2), p. 6, **before defining the area complexity**. The proof of v2 Theorem 2.6, pp. 8–17 (in particular its concluding assembly on pp. 16–17), was read in the supplied proof investigation but was not independently certified as an existence proof. The present package accepts its stated conclusion and retains that limit.

This does not change a previously fixed area function while purporting to preserve its numerical values. For a prescribed nonflat metric, the applications require the corresponding smooth fixed-boundary attainment theorem as an additional input; the printed v2 statement does not supply it. Lemma P itself has no flatness or linear-foliation requirement.

## 6. Consequences, without circular use of sliding attainment

All conclusions in this section use Lemma P and the fixed-boundary attainment input just declared. For a direct use of the printed v2 fixed-boundary theorem, choose the flat boundary metric and exact $1-r$ collar permitted in competition §3. No linear-foliation assumption is used in P or in the formal deductions. For any other prescribed metric, these deductions are conditional on a smooth fixed-boundary attainment theorem in that metric.

### 6.1 Finiteness of the bounded-genus, bounded-infimum vertex set

Suppose infinitely many distinct vertices $v_i$ have $g(v_i)=h$ and $A_{\mathrm{sm}}(v_i)\le a$, where the infimum is taken over smooth neat representatives with boundary a leaf. Choose representatives $G_i$ with areas at most $a+1$. Apply fixed-boundary attainment to each $G_i$, obtaining smooth neat exact relative minimizers $F_i$ with
$$
\mathrm{Area}(F_i)\le\mathrm{Area}(G_i)\le a+1.
$$
They remain in the respective vertex classes. By $P$, a subsequence is eventually properly isotopic to one limit. Smooth proper isotopy extension makes the late terms ambiently isotopic, contradicting distinctness of the vertices. The set is finite.

Neither sliding attainment nor compactness of all stable surfaces was used to select $F_i$. Once finiteness is known, the sparsity, well-ordering and countability arguments in Lemma 4.8(ii)–(iv) apply to these smooth infima.

Competition §4.1, p. 8, defines vertex representatives as neat surfaces and their isotopies as smooth families; Definition 4.7, pp. 10–11, takes the area infimum over these representatives. Thus its vertex infimum $A(v)$ has the smooth neat representative convention used here, and this argument proves Lemma 4.8(i) for the declared v2-compatible choice of §3 metric. This should not be confused with the different, explicitly piecewise-smooth infimum in Theorem A.6. For that latter infimum one still needs a comparison-class bridge; it is not automatic from this argument.

### 6.2 Smooth sliding-boundary attainment

Fix a smooth neat proper class $v$, and let $A_{\mathrm{sm}}$ be its sliding smooth area infimum. Select a smooth neat minimizing sequence $G_i$. Fixed-boundary minimization gives $F_i$ in the same proper class and
$$
A_{\mathrm{sm}}\le\mathrm{Area}(F_i)
\le\mathrm{Area}(G_i)\longrightarrow A_{\mathrm{sm}}.
$$
Apply $P$ to the tail with area at most $A_{\mathrm{sm}}+1$. The smooth neat limit is eventually isotopic to $F_i$, lies in $v$, has boundary a leaf, and has area $A_{\mathrm{sm}}$ by area continuity. It is minimal and stable. This proves the smooth form of (E)(ii) for the declared metric/input, non-circularly.

This gives the smooth-output conclusions required in the smooth version of A.6: a leaf boundary, a smooth proper embedding, stability, an embedded collar and neatness. It does **not** identify its area with the infimum over all competition Definition A.1 surfaces, prove membership of a Hass–Scott attained output in that definition, or prove the claimed multicomponent extension. Those statements require further inputs. Nor does it establish universal disjointness $(\mathrm{U})$, which remains an external input.

## 7. Checks against shorter but incomplete substitutions

The completed curvature proof does not straighten moving leaves and then treat exact minima for moving metrics as exact minima for the limiting metric. Nor does it read the existence of one parametrized component in Hass–Scott 3.5/6.10 as full geometric $C^1$ convergence of a genus-$h$ sequence.

The bounded-curvature half-graph lemma is applied **after** weighted point selection supplies its curvature hypothesis on the rescaled sequence. Its proof uses the surface tangent plane and uniform elliptic graph estimates. The curved original hypersurface is used only to produce a one-sided Euclidean limit. The flat height function then supplies neatness of the nonflat selected blow-up.

The area-ratio estimate is an explicit first-variation calculation for the original surfaces; its boundary term is controlled by the prescribed curve and the unit conormal. There is no statement that the density equals $1/2$. Reflection and Corollary 1.5 are applied only after completeness, embeddedness, quadratic area growth, simple connectedness and one-endedness have been justified.

## 8. Comparison classes and literature limits

### 8.1 The piecewise-smooth alternative is not completed

Hass–Scott Theorem 6.12, pp. 112–113, attains a fixed-boundary minimum in its own piecewise-smooth relative class. Competition Proposition A.5, §A.3, pp. 25–26, is a conditional regularity assertion about an attained object satisfying Definition A.1, §A.1, p. 23, including finite graph and corner conditions. Membership of the Hass–Scott output in that definition, and the corresponding equality of comparison infima, are not supplied here.

Thus this alternative has not supplied the smooth neat exact minimizers used in the applications. A conditional regularity theorem cannot create the object satisfying its hypotheses. The special graph-splice approximation in §4 is not an area-density theorem for arbitrary Definition A.1 objects. The full piecewise-smooth assertion of Theorem A.6 remains outside this repair.

### 8.2 Why a continuous value function alone is insufficient

The local leaf-translation estimate gives continuity of the area value

$$
I(t)=\inf\{\mathrm{Area}(G):G\in v,\ \partial G=\lambda_t\}
$$

over the union of relative classes, with a local estimate

$$
e^{-C|s-t|}I(s)\le I(t)\le e^{C|s-t|}I(s).
$$

This gives a minimum number on the compact parameter circle, not a surface attaining it in one relative class. Branch minima $1+1/n$ illustrate that a positive lower bound does not make the infimum attained.

In a linear collar chart $(x,y,r)$, where $y\in\mathbb R/\mathbb Z$ is transverse to the longitudes, take $\chi(0)=1$ with $\chi$ zero outside the collar and set

$$
B_s(x,y,r)=(x,y+s\chi(r),r),\qquad 0\le s\le1.
$$

The boundary map returns to the identity at $s=1$, while the endpoint inside the collar is

$$
B_1(x,y,r)=(x,y+\chi(r),r).
$$

It can act on fixed-boundary relative classes. A class transported around the circle need not return to its starting class merely because the boundary map does. This is a reason to check monodromy, not a claim that the action is nontrivial or has an infinite orbit for every surface. Compare v2 Lemma 3.11 and its proof, p. 30, where the endpoint $B_1$ is retained.

No independent finiteness of these branches or triviality of their monodromy is claimed. With the boundary fixed, Lemma P gives eventual isotopy relative to that boundary; together with fixed-boundary attainment it does control bounded-area attained relative classes. That argument uses Lemma P and is not an independent replacement for it.

### 8.3 Limits of source verification and novelty

The checked sources supply Anderson's disk estimate and one-ended Euclidean rigidity and Hass–Scott's exact-disk confinement and convergence tools. No single checked statement was found that directly gives all of Lemma P, including final isotopy, for these original metric and foliation data. This is a report about the checked materials, not a claim that no such theorem exists in the literature.

No exhaustive novelty search was performed. If a fully applicable earlier boundary compactness theorem is supplied, the contribution may be a completion of a missing citation. It does not establish novelty, falsity of $(\mathrm{Fin})$, or falsity of Theorem A.

## 10. Precise scope

- Proved for the stated existing exact-minimizer family: local diskization and global Plateau minimality of local disks; separation of the artificial face; curvature control up to the original boundary; smooth geometric extraction; covering degree one; eventual proper isotopy; hence Lemma P.
- Deduced with the declared v2-compatible fixed-boundary input: competition Lemma 4.8(i) and smooth sliding-boundary attainment. The proof of that external existence theorem is not independently certified here.
- Not supplied: fixed-boundary existence for arbitrary prescribed nonflat metrics; equality of the full competition piecewise-smooth infimum with the smooth infimum; the full comparison-class assertion or multiboundary extension of Theorem A.6.
- Outside the compactness claim: all stable members of Kapovich's $M_a$ and universal disjointness $(\mathrm{U})$.
- Source-verification limits: the original Schoen chapter, Lawson monotonicity source, Gilbarg–Trudinger book, Richards article, and original Morrey/Meeks–Yau articles were not separately checked. The exact standard forms used are stated in [§3](localization.md). The boundary area-ratio estimate, boundary half-charts, continuous filling argument and Euclidean reflection are proved in this package.

An independent fresh-context adversarial review found no fatal issue and no missing mathematical step; it flagged one wording issue, that the center in the interior monotonicity lower bound must belong to the disk image. This is explicit in §3, input 2. The review applies to Lemma P and the applications with the declared fixed-boundary existence input; it does not certify novelty or the stronger excluded conclusions.
