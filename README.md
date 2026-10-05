# Boundary compactness for exact relative least-area Seifert surfaces

**Lemma P gives smooth compactness up to the original boundary and eventual proper isotopy for existing smooth exact fixed-boundary relative area minimizers with one longitude boundary and bounded area.** With the separately declared fixed-boundary existence input, it yields competition Lemma 4.8(i) and smooth sliding-boundary attainment without using general stable-surface compactness or sliding attainment to choose the minimizers.

Version 1.0 · 5 October 2026. [中文说明](README.zh-CN.md).

## Target and contribution

Target: Apex Intelligence, *Contractibility of the complex of incompressible Seifert surfaces: the knot case of Kakimizu's problem*, official competition version dated 11 September 2026, 48 pages. PDF SHA-256:

`34f17d7d99780d3fd3626d9e5d7b35d6aa76661c404f191b6df341b300c0c06f`.

The category proposed for review is **breakthrough contribution: repair of a key compactness gap**. The dependence is competition Theorem 3.3 $(\mathrm{Fin})$, p. 7, Lemma 4.8, p. 11, and Theorem A.6, p. 27, through Kapovich Proposition A.1 and its corollaries in Schultens, *J. Topol.* **3** (2010). Anderson Theorem 3.1, the cited compactness tool, controls a fixed positive-depth truncation in its convex defining-function setting; it does not supply convergence at the original boundary.

The later author version, Pan–You–Zhou–Chen, arXiv:2609.09224v2 (12 September 2026), retains this dependence in Theorem 2.16, pp. 22–23, and Lemma 4.2, pp. 31–32. The [gap analysis](proof/gap.md) records the hypotheses, output mismatch and the reason a weak convex collar function does not fix it.

## Result and proof

In the fixed smooth strictly convex collar geometry of the target, let $J$ be its compact smooth family of longitude leaves. Fix genus $h$ and $a>0$. If $F_i$ are connected orientable smooth incompressible neat embeddings with one boundary leaf, area at most $a$, and each attains the area minimum in its own smooth relative ambient isotopy class fixing its boundary pointwise, **Lemma P** supplies a smoothly convergent subsequence modulo reparametrization, a neat embedded limit with boundary in $J$, and eventual proper ambient isotopy. If the boundary curve is fixed throughout, the final isotopy fixes it pointwise. See the [full statement](proof/localization.md).

Exactness first forces every localized outermost disk to be a global Plateau minimum in a fixed smooth ambient extension. The boundary first-variation calculation gives a quadratic area upper bound without assuming density $1/2$. Weighted point selection makes the artificial boundary recede; bounded-curvature Fermi half-charts select a nonflat Euclidean half-space limit. Its unique actual boundary arc anchors multiplicity one before loops are lifted. Global minimizing subdisks give continuous fillings on the same leaf, proving simple connectedness. Only this Euclidean limit is reflected. Van Kampen and surface classification give one end and finite topological type, so Anderson Corollary 1.5 forces a plane and contradicts the normalized curvature. Full extraction and a boundary-adapted tubular covering give degree one and the final isotopy.

## Input levels and limits

- Lemma P assumes existence of the exact minimizers. It does not require a flat torus or a linear foliation.
- The two applications accept v2 Theorem 2.6, p. 8, as an external smooth fixed-boundary attainment input; its proof has not been independently certified here. For this printed input, choose the flat boundary metric, linear longitude leaves and exact $1-r$ collar permitted by competition §3 **before** defining the area complexity.
- For another prescribed nonflat metric, the applications require the corresponding fixed-boundary attainment theorem. Lemma P does not supply existence by itself.
- Universal disjointness $(\mathrm{U})$ remains an external input. This repair does not prove compactness for all stable surfaces in Kapovich's $M_a$, the full piecewise-smooth assertion of Appendix A, or a multiboundary version.
- No exhaustive novelty search was performed. A fully applicable earlier theorem could reduce the contribution to a missing-citation completion. No falsity of Theorem A or $(\mathrm{Fin})$ is claimed.

The original Schoen chapter, Lawson source, Gilbarg–Trudinger book, Richards article and Morrey/Meeks–Yau papers were not separately checked. Their standard forms are declared in [§3](proof/localization.md); the [bibliography](sources/bibliography.md) distinguishes direct text checks, recorded visual/source checks and unchecked originals.

## Repository guide

1. [proof/gap.md](proof/gap.md): printed dependence paths, Anderson's truncation theorem and the boundary-output mismatch.
2. [proof/localization.md](proof/localization.md): Lemma P, precise standard inputs, convex replacement domains, relative splices and exact disk minimality (§§2–4).
3. [proof/boundary-estimate.md](proof/boundary-estimate.md): area ratio, half-charts, point selection, boundary multiplicity, continuous fillings and Euclidean reflection (§§5.1–5.5).
4. [proof/extraction-and-isotopy.md](proof/extraction-and-isotopy.md): full smooth extraction, neatness, covering degree one and eventual isotopy (§§5.6–5.7).
5. [proof/consequences.md](proof/consequences.md): noncircular finiteness and sliding attainment, fixed-boundary input, piecewise alternative and precise scope (§§6–8, 10).
6. [sources/bibliography.md](sources/bibliography.md): editions, checked printed locations and public acquisition routes.
7. [LICENSE](LICENSE): CC BY 4.0 scope and attribution. [MANIFEST.sha256](MANIFEST.sha256): SHA-256 of every other repository file, relative to the repository root.

No third-party full text, PDF, code or computation is bundled. The complete proof is in the five proof files. Their retained section numbers make cross-file references unambiguous.

## Review and AI disclosure

An independent adversarial review in a fresh context found **no fatal issue and no missing mathematical step**. It flagged one wording issue, now fixed in localization §3, input 2: the center of an interior monotonicity ball lies on the disk image. The review covers Lemma P and the two applications with the declared existence input; it does not certify the excluded stronger conclusions or novelty. The journal proof of Kapovich's Proposition A.1 (pp. 897–898) was compared directly with the preprint proof and is word for word the same.

> GPT-6.1 Sol, in OpenAI Codex under human direction, developed the proof and drafted this text; a separate GPT-6.1 Sol session in a fresh context performed an adversarial review. Claude planned the work, checked key steps against the sources, and reviewed and edited the final text. No human expert has certified the work.

## License

Original prose and the original selection and arrangement of this package are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), to the extent applicable rights exist. External publications retain their own terms and are cited or linked, not redistributed. See [LICENSE](LICENSE) for attribution and scope.
