# Probabilités — notes

Notes for `FMA_3TC11_TP`, Télécom Paris 1A, S1 2026-27. The course material they
were written from, and the module README that describes it, stay in
[`don-ko/telecom`](https://github.com/don-ko/telecom/tree/main/fma-3tc11-probabilites) (private)
(`~/Documents/project/telecom/fma-3tc11-probabilites/`): references below to `cours/`, `td/`,
`examens/` and the like are to that directory. The notes moved here from its
`notes/` on 2026-09-28.

**Written.** Nine chapters, 133 pages, built from the 2026-27 poly with the exam
papers in [`examens/`](https://github.com/don-ko/telecom/blob/main/fma-3tc11-probabilites/README.md#examens) supplying worked examples. Build with `latexmk -pdf`
from inside this directory, which is where `custom.sty` has to be found; the built PDF is
committed beside the sources.

The chapters are the poly's eight, one to one, plus a reference chapter the poly has no
counterpart for. Every paper in `examens/` allows *1 feuille A4* and supplies nothing,
so chapter 9 is what that sheet gets built from.

| File | What it is |
|---|---|
| `fma-3tc11-probabilites-notes.tex` | Main file — preamble, title, abstract, and the nine `\input`s |
| `custom.sty` | The shared style package, byte-identical to the house style, `~/Documents/area/tex-templates/notes/custom.sty`, and to the copies in [`nus/y2s1/cs2100`](../../../nus/y2s1/cs2100/) and [`cs3231`](../../../nus/y2s1/cs3231/) |
| `glossary.md` | The French-first term list — each glossed term's French form (the source's spelling), English gloss and the one chapter that glosses it, plus the terms used as they stand. See [the 2026-09-21 spec](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-21-french-first-notes-design.md) |
| `chapters/1-probabilites-discretes.tex` | Discrete probability — the prerequisite, written in full because the generating function and the discrete conditional expectation appear nowhere else |
| `chapters/2-theorie-mesure.tex` | Tribus, measures, negligible sets, measurable functions; carries the uniqueness theorem's proof and explains the notation collisions once for the whole document |
| `chapters/3-integrale-lebesgue.tex` | The Lebesgue integral — construction, the convergence theorems, transfer, change of variables, Fubini; the longest chapter at 26 pages |
| `chapters/4-theorie-probabilites.tex` | Probability spaces, CDFs, densities, moments, random vectors, and the test-function method the annales use most |
| `chapters/5-loi-conditionnelle.tex` | Conditioning on an event, then on a random variable, then the tower property |
| `chapters/6-fonction-caracteristique.tex` | The characteristic function: inversion, moments, and the product rule chapters 7 and 8 run on |
| `chapters/7-vecteurs-gaussiens.tex` | Gaussian vectors, defined by linear combinations, with the counter-example carried in full |
| `chapters/8-theoremes-limites.tex` | Convergence modes, the strong law and the central limit theorem, both proved |
| `chapters/9-annexes-classe-monotone-lois.tex` | Reference — the monotone class lemma, the two law tables extended with computed moments and transforms, and a convergence summary |

**Sources.** The poly `cours/poly-cours-2026-27.pdf` is primary and supplies the
structure; its exercises and their annexe E solutions, and the ten papers in
`examens/`, supply the worked examples. **`cours/cours-mesure-2025-26.pdf` is
deliberately not a source**: its vintage is unsettled — see [The Groupe 4 section is
undated](https://github.com/don-ko/telecom/blob/main/fma-3tc11-probabilites/README.md#the-groupe-4-section-is-undated) — and it covers only poly chapter 2 and the
opening of chapter 3, which the poly itself covers in more depth. A held document is a
notes source when its vintage is confirmed for the year being studied, or when it
supplies content the confirmed sources do not; this deck satisfies neither.

Design and rationale:
[telecom: docs/superpowers/specs/2026-09-17-fma-3tc11-notes-design.md](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-17-fma-3tc11-notes-design.md).

