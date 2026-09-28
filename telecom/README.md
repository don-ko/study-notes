# Télécom Paris — notes

Notes for the **Diplôme d'ingénieur, 1ère année**, academic year **2026-27**.
`1a-s1/` holds semester S1, one directory per module, named from the official
sigle as in the coursework repo. The course material the notes were written
from — `cours/`, `td/`, `examens/` — and the module READMEs that describe it stay
in [`don-ko/telecom`](https://github.com/don-ko/telecom)
(`~/Documents/project/telecom/`). The notes moved here from its
`<module>/notes/` directories on 2026-09-28.

Five modules have notes: four are written from the material in their `cours/`,
`td/` and `examens/`, and one FMA module holds only the setup, described below.
The notes are **not** a second copy of the decks: the decks are slides, and
these are continuous prose in the format the rest of my notes use, so the two
are read for different things.

## Layout and format

    1a-s1/<module>/
      README.md                   what each file is, and what the notes cover
      <module>-notes.tex          main file: preamble, title, abstract, \input list
      <module>-notes.pdf          the built notes, committed
      custom.sty                  the shared style package, byte-identical across modules
      glossary.md                 each glossed term's French form, English gloss and home chapter
      chapters/<n>-<topic>.tex    one file per chapter, \section at the top
      src/ascii-table.pdf         compilation only: the one included figure (see Figures)

Compilation's `chapters/` also holds `2a-aide-memoire-x86-64.tex`, an unnumbered
x86-64 reference sheet that is not a chapter; the letter keeps it sorted after
chapter 2 without renumbering the chapters that follow.

The format is the one already used for [`nus/y2s1/cs3231`](../nus/y2s1/cs3231/)
and [`cs2100`](../nus/y2s1/cs2100/): `article` at 10pt, 1in margins, sans-serif
headings via `sectsty`, a `fancyhdr` running head carrying the section,
`\microtoc`, and the unnumbered theorem-like environments `definition` /
`example` / `theorem` / `remark` / `notation` / `proof` that carry most of the
content. The two reference documents differ on three lines, and **`cs3231` is the
one followed here**: `\parindent` 0in rather than 0.2in, `secnumdepth` 2 rather
than 3 — subsubsections carry no number — and `titlesec` setting
`\subsubsection` in `\large\bfseries\sffamily`. `fontenc` at `T1` is the one
departure the French forces, and `fix-cm` rides with it: EC's optical sizes
would otherwise print the 30pt title light where the reference prints it bold.
`custom.sty` is **copied unchanged** from there — `shasum -a 256` matches across
all seven documents and the house style's reference copy,
`~/Documents/area/tex-templates/notes/custom.sty` — so anything module-specific
(TikZ libraries, `pgfplots`, the `listings` language definition for x86-64 GAS
assembly) is declared in that module's main file instead, and the style package
never forks.

| Module | Chapters | Pages | Built from |
|---|---|---|---|
| [`phy-3tc20-optique-photonique`](1a-s1/phy-3tc20-optique-photonique/) | 7 | 91 | the 159-page poly, the six chapter decks, and the two mise-à-niveau decks |
| [`ece-3tc21-propagation-antennes`](1a-s1/ece-3tc21-propagation-antennes/) | 6 | 69 | the 131-page poly, the L1–L3 and L4–L5 amphi decks, and the three autonomy TD series |
| [`ece-3tc32-compilation`](1a-s1/ece-3tc32-compilation/) | 7 + reference sheet | 55 | the séance-1 to séance-3 decks, the séance-1 x86 corrigés, the séance-3 TP templates, and Stanford CS107's x86-64 reference sheet — the séance-4 deck is held and has no chapter yet |
| [`fma-3tc11-probabilites`](1a-s1/fma-3tc11-probabilites/) | 9 | 133 | the 187-page poly, its 102 exercises with their annexe E solutions, and the ten annales — the one lecture deck held is deliberately not a source |

The page counts are of the committed PDFs; `latexmk -pdf` from inside a module
directory reproduces them, and that is where `custom.sty` has to be found.

`1a-s1/fma-3tc10-analyse-fonctionnelle-fourier/` is set up and not yet written.
It holds its main file, `custom.sty` and the built PDF, and no `chapters/`: the
`\input` list is empty, the abstract says no chapters exist, and the preamble
keeps only what the written modules share: their common lines and the TikZ
libraries they all load, `arrows,calc`. A setup is not a stub — no chapter file
exists until its chapter does — and the notes follow in their own spec. The commit that adds the first chapter deletes
the abstract's "No chapters are written yet" paragraph, which is true only of
the setup.

A setup does not run against the Économie precedent below either: it commits to
no content. 3TC10's material is 2025-26 too, but the decision to write its notes
rests on one thing Économie lacks: its 2026/2027 Moodle course publishes those
polys under *Supports et programme* with no rival 2026-27 series beside them.
The vintage stays a recorded risk for the notes.

Économie has no notes. Its six séance decks print 2025 on every cover and the
module README records their reuse this year as unconfirmed, so there is nothing
yet worth writing notes against.

Compilation's seven chapters cover séances 1 to 3. **Séance 4 is the first
séance whose deck is held while its notes are not** — 145 pages of LR parsing
that chapter 5 reaches only as far as LL(1) descent. It and the séquençage's
remaining blocks — portes logiques combinatoires and synchrones, génération de
code, and the projet compilateur — get chapters when they are written; no stubs
are left for them.

## Language

The notes are **French-first**. Section titles, at every level, are French —
the source's own heading where it has one. A technical term appears, in the
chapter that defines it, as the source's French in bold with its English gloss
in italics — `\textbf{facteur de réflexion} (\textit{reflection coefficient})` —
and everywhere else in French alone, English prose included (a noun only: an
English adjective such as *executable* stays English). Each module's
`glossary.md` fixes the French term, its gloss and the one chapter that glosses
it. Definitions, theorems and any prose that closely translates the source are
the source's own French; the commentary written here stays English. The notes
cite no source document — no slide, poly, corrigé or séance — so they stand on
their own, and where a source is wrong they state the correct fact without
pointing at the error. The exams are sat in French, and this is the vocabulary
they use.

## Figures

Figures are drawn in TikZ and `pgfplots` in the chapter source. There are no
raster crops of slides: the notes stand on their own rather than re-importing
the decks. The one included file is compilation's `src/ascii-table.pdf`, a
vector drawing of the public-domain US-ASCII chart.

## Design

The dated specs that designed these notes stay in the coursework repo: the
format, the byte-identical `custom.sty` and the drawn figures
([2026-09-13](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-13-module-notes-design.md)),
the Probabilités notes
([2026-09-17](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-17-fma-3tc11-notes-design.md)),
the Compilation x86-64 reference sheet
([2026-09-21](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-21-ece-3tc32-x86-reference-sheet-design.md)),
and the French-first rewrite
([2026-09-21](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-21-french-first-notes-design.md)).
