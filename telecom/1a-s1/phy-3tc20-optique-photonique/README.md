# Optique et Photonique — notes

Notes for `PHY_3TC20_TP`, Télécom Paris 1A, S1 2026-27. The course material they
were written from, and the module README that describes it, stay in
[`don-ko/telecom`](https://github.com/don-ko/telecom/tree/main/phy-3tc20-optique-photonique)
(`~/Documents/project/telecom/phy-3tc20-optique-photonique/`): references below to `cours/`, `td/`,
`examens/` and the like are to that directory. The notes moved here from its
`notes/` on 2026-09-28.

Seven chapters, 91 pages built. Format and rationale:
[telecom: docs/superpowers/specs/2026-09-13-module-notes-design.md](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-13-module-notes-design.md).

| File | What it is |
|---|---|
| `phy-3tc20-optique-photonique-notes.tex` | Main file — preamble, title, abstract, the `\input` list that fixes chapter order |
| `custom.sty` | The shared style package, byte-identical to the house style, `~/Documents/area/tex-templates/notes/custom.sty`, and to the copies in [`nus/y2s1/cs2100`](../../../nus/y2s1/cs2100/) and [`cs3231`](../../../nus/y2s1/cs3231/) |
| `glossary.md` | The French-first term list — each glossed term's French form (the source's spelling), English gloss and the one chapter that glosses it, plus the terms used as they stand. See [the 2026-09-21 spec](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-21-french-first-notes-design.md) |
| `chapters/1-optique-geometrique.tex` | Poly ch. 1 — index, chemin optique, Descartes-Snell, dispersion, angle limite — **plus** the interference material from the two mise-à-niveau decks, which the poly has no chapter for and chapters 4 and 6 depend on |
| `chapters/2-ondes-analyse-spectrale.tex` | Poly ch. 2 — Maxwell, the plane wave, polarisation, complex notation, spherical waves, then Fourier series, the Fourier transform, its properties and the usual distributions |
| `chapters/3-diffraction.tex` | Poly ch. 3 — Huygens-Fresnel, the Fresnel and Fraunhofer approximations, the lens as a Fourier transform (carrying the TD's explicit calculation), convolution, and image processing |
| `chapters/4-fibre-optique.tex` | Poly ch. 4 — RTI and the cone d'acceptance, intermodal dispersion, transverse modes by interference, the dielectric plane guide, and the Maxwell resolution |
| `chapters/5-laser.tex` | Poly ch. 5 — thermal radiation, spontaneous and induced transitions, the Einstein equations, population inversion and amplification, the cavity, threshold, and the beam's properties |
| `chapters/6-holographie.tex` | Poly ch. 6 — recording, the algebra of the three read-out orders, transmission vs reflection holograms, experimental constraints, applications |
| `chapters/7-annexe-transformees-fourier.tex` | Poly Annexe 1 — the Fourier transform table. This is **the one document supplied at the exam**, per the Moodle règles: *« L'examen est SANS document et SANS calculatrice. Le tableau de transformées de Fourier vous sera fourni »* |

Chapters 1–6 map onto the poly's six numbered chapters and onto the six `cours/`
decks. Build with `latexmk -pdf` from inside this directory, which is where `custom.sty`
has to be found. The built PDF is committed; the `.aux` and `.log` are not.

