# Antennes & Propagation dans les systèmes radiofréquences — notes

Notes for `ECE_3TC21_TP`, Télécom Paris 1A, S1 2026-27. The course material they
were written from, and the module README that describes it, stay in
[`don-ko/telecom`](https://github.com/don-ko/telecom/tree/main/ece-3tc21-propagation-antennes)
(`~/Documents/project/telecom/ece-3tc21-propagation-antennes/`): references below to `cours/`, `td/`,
`examens/` and the like are to that directory. The notes moved here from its
`notes/` on 2026-09-28.

Six chapters, 69 pages built. Format:
[telecom: docs/superpowers/specs/2026-09-13-module-notes-design.md](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-13-module-notes-design.md).

| File | What it is |
|---|---|
| `ece-3tc21-propagation-antennes-notes.tex` | Main file — preamble, title, abstract, the `\input` list that fixes chapter order |
| `custom.sty` | The shared style package, byte-identical to the house style, `~/Documents/area/tex-templates/notes/custom.sty`, and to the copies in [`nus/y2s1/cs2100`](../../../nus/y2s1/cs2100/) and [`cs3231`](../../../nus/y2s1/cs3231/) |
| `glossary.md` | The French-first term list — each glossed term's French form (the source's spelling), English gloss and the one chapter that glosses it, plus the terms used as they stand. See [the 2026-09-21 spec](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-21-french-first-notes-design.md) |
| `chapters/1-systemes-telecom-rf.tex` | Partie 1 — telecom systems, why RF, the specificities and the attenuation problem, with the frequency-band table |
| `chapters/2-propagation-oem.tex` | Partie 2 — the MLHI medium, the OPPM, Maxwell applied to it, the propagation and dispersion equations, the Poynting vector |
| `chapters/3-lignes-transmission.tex` | Partie 3 — coax and microstrip, the lumped model, the telegrapher's equations, γ, Z_C, Γ, impédance ramenée, standing waves and ROS, power. Carries the TD préparatoire's cylindrical-coordinates derivation |
| `chapters/4-adaptation-parametres-s.tex` | Partie 4 — λ/4 transformer, stub and lumped-element matching; power waves and the S matrix. Carries a worked example from each of the two autonomy series that are in the exam programme |
| `chapters/5-antennes-bilan-liaison.tex` | Partie 5 — input impedance and bandwidth, radiation pattern, directivity and gain, polarisation, the usual antenna families, then Friis, PIRE, atmospheric absorption, rain, and the Fresnel ellipsoid link budget from the TD4 autonomy series |
| `chapters/6-operateurs-milieux-metamateriaux.tex` | Partie 6 — the vector operators as a reference table, imperfect dielectrics and conductors, and metamaterials |

The chapters map one-to-one onto the poly's six *Parties*; the amphi decks map
onto them as L1–L3 across chapters 1–4 and L4–L5 onto chapter 5. Build with
`latexmk -pdf` from inside this directory, which is where `custom.sty` has to be found.
The built PDF is committed; the `.aux` and `.log` are not.

