# 精确相对最小面积 Seifert 曲面的边界紧性

**引理 P 证明：已存在的光滑精确定边界相对极小元，在面积有界、单一经线边界条件下，存在直到原边界光滑收敛的子列，并最终与极限 proper 同痕。** 另接受明确声明的定边界存在性输入后，可非循环地推出比赛版 Lemma 4.8(i) 和光滑滑动边界达到性。

版本 1.0，2026 年 10 月 5 日。[English overview](README.md)。

## 目标与贡献

目标为 Apex Intelligence 署名的比赛版 *Contractibility of the complex of incompressible Seifert surfaces: the knot case of Kakimizu's problem*，2026 年 9 月 11 日，48 页。PDF SHA-256：

`34f17d7d99780d3fd3626d9e5d7b35d6aa76661c404f191b6df341b300c0c06f`。

拟申报类别为突破贡献：修补关键紧性缺口。比赛版 Theorem 3.3 的 $`(\mathrm{Fin})`$（p. 7）、Lemma 4.8（p. 11）及 Theorem A.6（p. 27）依赖 Kapovich 在 Schultens 论文附录中的 Proposition A.1 及其推论。该证明调用的 Anderson Theorem 3.1，只控制凸定义函数域中的固定正深度截断，未供应原曲面直到原边界的收敛。

Pan、You、Zhou、Chen 的作者后续版本 arXiv:2609.09224v2（2026 年 9 月 12 日）在 Theorem 2.16（pp. 22–23）及良序性 Lemma 4.2（pp. 31–32）中仍保留相应依赖。领子上的弱凸函数不能把截断收敛结论升级为原边界收敛。详见[缺口分析](proof/gap.md)。

## 证明和应用

精确最小性先通过全局 Plateau 比较盘、相对盘替换及特定接缝的面积逼近，迫使原局部盘本身成为全局最小面积盘。边界一阶变分给出二次面积上界，不预设密度为 $`1/2`$。加权曲率点选使人工边界在缩放中退至无穷远；已有曲率界后才建立 Fermi 半图像。实际边界的唯一弧先锚定一重，再提升闭环并用极小子盘取得不逃逸的连续填充。仅对欧氏极限反射，取得一端、有限拓扑型及二次面积增长后，才使用 Anderson Corollary 1.5。全局抽取的边界适配管状投影给出覆盖度一及最终同痕。

引理 P 的[准确陈述](proof/localization.md)假设曲面已存在，并在固定光滑相对环境同痕类内精确达到定边界面积下确界；它不要求平直环面或线性叶层。

两项应用以 v2 Theorem 2.6（p. 8）为外部定边界达到性输入，未独立认证其证明。直接使用该印刷陈述时，在定义面积复杂度之前，选择比赛版 §3 允许的平直边界环面、线性经线叶层和精确 $`1-r`$ 领子。任意已固定的非平直度量还需要相应的定边界达到性定理。

## 范围

- 全称不交性 $`(\mathrm{U})`$ 仍是外部输入。
- 不证明 Kapovich 的全部稳定曲面空间 $`M_a`$ 紧。
- 不证明比赛版附录 A 的完整分片光滑类别、分片与光滑 infimum 的桥或多边界版本。
- 未进行完整新颖性检索；如存在完全适用的旧定理，贡献可能应降为补充引用。这里不主张 Theorem A 或 $`(\mathrm{Fin})`$ 为假。
- Schoen 原章、Lawson 来源、Gilbarg–Trudinger 原书、Richards 原文和 Morrey/Meeks–Yau 原文未单独核对。所用标准形式和核查层级见[输入](proof/localization.md)与[文献表](sources/bibliography.md)。

## 仓库导览

1. [缺口](proof/gap.md)：印刷依赖路径、截断条件与输出错配。
2. [局部化](proof/localization.md)：引理 P、输入条件、凸替换域、接缝和精确盘最小性（§§2–4）。
3. [边界估计](proof/boundary-estimate.md)：面积比、半图像、点选、一重锚定、单连通与欧氏反射（§§5.1–5.5）。
4. [抽取与同痕](proof/extraction-and-isotopy.md)：整曲面抽取、覆盖度一、最终同痕（§§5.6–5.7）。
5. [推论与限制](proof/consequences.md)：有限性、光滑滑动达到性、存在性输入及分片替代路径的限制（§§6–8、10）。
6. [文献表](sources/bibliography.md)：版本、核对过的印刷定位及公开获取方式。
7. [许可](LICENSE)与[文件哈希](MANIFEST.sha256)：散文 CC BY 4.0；清单覆盖仓库中除清单自身外的全部文件。

完整英文证明分布于五个证明文件，保留的节号用于跨文件定位。不附外部全文、PDF、代码或计算产物。

## 复核与 AI 声明

已有全新上下文对抗复核结论为：致命问题 0 条、可修补级数学缺步 0 条、表述问题 1 条。表述修正已落实到局部化 §3 输入 2：内部单调性下界的球心必须属于该极小盘的像。该复核只覆盖已声明的引理 P 和条件式应用，不认证新颖性或更强结论。Kapovich Proposition A.1 的期刊版证明（第 897–898 页）已与预印本证明直接对照，逐字相同。

AI 声明：

> GPT-6.1 Sol, in OpenAI Codex under human direction, developed the proof and drafted this text; a separate GPT-6.1 Sol session in a fresh context performed an adversarial review. Claude planned the work, checked key steps against the sources, and reviewed and edited the final text. No human expert has certified the work.

## 版本说明

本版本与 `6179e85e49f30e9b02e4e7956d02eb94e2931f7e` 相比，只改了公式的写法。GitHub 的 Markdown 处理会去掉 `$...$` 里的 `\{`、`\,` 等反斜杠转义，还有部分公式没被识别，所以全部公式改用 GitHub 的原样数学语法。数学文字没有任何改动。

## 许可

原创散文及本材料的原创选择与编排，在适用权利存在的范围内采用 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)。外部论文保留各自许可与版权，只作引用或链接。署名方式和范围见 [LICENSE](LICENSE)。
