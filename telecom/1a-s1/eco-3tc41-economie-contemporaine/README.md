# Introduction à l'économie contemporaine — notes

Notes for `ECO_3TC41_TP`, Télécom Paris 1A, S1 2026-27. The course material they
were written from, and the module README that describes it, stay in
[`don-ko/telecom`](https://github.com/don-ko/telecom/tree/main/eco-3tc41-economie-contemporaine) (private)
(`~/Documents/project/telecom/eco-3tc41-economie-contemporaine/`): references below to `cours/`
and the like are to that directory.

**Written.** Nine chapters, 108 pages. Chapters 1 to 6 are the « micro » half, one per
partie of its course plan, chapter 1 opening with the plan's two introductory items;
chapters 7 to 9 are the « macro » half, one per leçon. Build with `latexmk -pdf` from
inside this directory, which is where `custom.sty` has to be found; the built PDF is
committed beside the sources.

The decks, the « macro » ones above all, state some definitions and facts wrongly. The
notes state the correct fact, checked against primary sources, and where an exam question could turn on it a
remark titled *Formulation du cours* follows with the course's own wording: 49 remarks,
all but one in chapters 7 to 9. The glossary keeps 445 terms: those a page defines or
properly introduces, the labels the figures print only in English, and the acronyms'
expansions.

| File | What it is |
|---|---|
| `eco-3tc41-economie-contemporaine-notes.tex` | Main file — preamble, title, abstract, and the nine `\input`s |
| `custom.sty` | The shared style package, byte-identical to the house style, `~/Documents/area/tex-templates/notes/custom.sty`, and to the copies in [`nus/y2s1/cs2100`](../../../nus/y2s1/cs2100/) and [`cs3231`](../../../nus/y2s1/cs3231/) |
| `glossary.md` | The French-first term list — each glossed term's French form, English gloss and the one chapter that glosses it, plus the terms used as they stand. See [the 2026-09-21 spec](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-21-french-first-notes-design.md) |
| `chapters/1-organisation-transactions.tex` | The plan's introduction and Partie 1 — the questions economics is asked today, the circuit économique and the frontière des possibilités de production, the price of a coffee in a station worked through, how transactions are organised, and Marx vs. Hayek |
| `chapters/2-marche-concurrentiel.tex` | Partie 2 — individual demand from courbes d'indifférence, the TMS and the contrainte budgétaire, the effets de substitution et de revenu, aggregate demand and its elasticity, supply, the équilibre de marché, prix plafonds and planchers, and the effect of taxes |
| `chapters/3-analyse-bien-etre.tex` | Partie 3 — disponibilité à payer and the two surpluses, surplus total, the efficacité de Pareto in the boîte d'Edgeworth and the product mix, and Rawls |
| `chapters/4-analyse-long-terme.tex` | Partie 4 — coûts explicites and coûts d'opportunité, coût moyen and coût marginal, rendements d'échelle, and the équilibre de long terme |
| `chapters/5-defaillances-marche.tex` | Partie 5 — the monopole and its perte sèche, externalités and the three remedies (réglementation, Pigou, cap and trade), biens publics and biens communs, and Akerlof's lemons |
| `chapters/6-rationalite-raisonnements-strategiques.tex` | Partie 6 — rationalité and its axioms, the préférences révélées and WARP, jeux stratégiques and the équilibre de Nash |
| `chapters/7-concepts-cadres-theoriques.tex` | Leçon 1 — the State's role, the national-accounts aggregates and the public finances, the déséquilibres and how policy steers the conjoncture (the Keynesian model and its multiplicateurs), and the leçon's revision questions |
| `chapters/8-politiques-conjoncturelles-1970-2026.tex` | Leçon 2 — French conjunctural policy since 1970: the failed relance of 1970–1982, the franc fort and the SME crises up to the euro and the EU budget rules, the crises of 2007–2026 and the debt they left, the BCE's policy, and the policy mix |
| `chapters/9-situation-actuelle-france.tex` | Leçon 3 — the present French situation: whether the dette publique is sustainable (r − g, the solde primaire stabilisant), and the levers for reducing the deficit and the debt — recettes, dépenses, structural reforms — with the CAE's 2025 study |

**Sources.** The module's two 2026-27 series, and only those: the « micro » half's
course plan and three decks, `cours/cours-patrick-waelbroeck-2026-27/`, for chapters
1 to 6, and the « macro » half's three leçons for chapters 7 to 9 — chapter 9 from the
revision of 8 October 2026. **The six 2025-26 séance decks in `cours/` are
deliberately not a source**: their reuse this year is unconfirmed, and what they cover
is either on the « micro » plan or not taught in 2026-27. A held document is a notes
source when its vintage is confirmed for the year being studied, or when it supplies
content the confirmed sources do not; these satisfy neither.

**Figures.** The « micro » decks borrow textbook figures labelled in English. They
are redrawn in TikZ with French labels; where the course prints no French for a
label, the notes use the standard French term and the glossary row says so.

Design and rationale:
[telecom: docs/superpowers/specs/2026-10-10-eco-3tc41-notes-design.md](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-10-10-eco-3tc41-notes-design.md).
