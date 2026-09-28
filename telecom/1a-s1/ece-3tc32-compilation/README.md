# Compilation — notes

Notes for `ECE_3TC32_TP`, Télécom Paris 1A, S1 2026-27. The course material they
were written from, and the module README that describes it, stay in
[`don-ko/telecom`](https://github.com/don-ko/telecom/tree/main/ece-3tc32-compilation) (private)
(`~/Documents/project/telecom/ece-3tc32-compilation/`): references below to `cours/`, `td/`,
`examens/` and the like are to that directory. The notes moved here from its
`notes/` on 2026-09-28.

Seven chapters (0–6)
and an x86-64 reference sheet, 55 pages built, covering séances 1 to 3 — séance 4 is taught
and has no chapter yet.
Format and rationale:
[telecom: docs/superpowers/specs/2026-09-13-module-notes-design.md](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-13-module-notes-design.md).

| File | What it is |
|---|---|
| `ece-3tc32-compilation-notes.tex` | Main file — preamble, title, abstract, the `\input` list that fixes chapter order. Also carries the `listings` style and a `gas` language definition for x86-64 AT&T assembly, which the shared `custom.sty` does not and must not |
| `custom.sty` | The shared style package, byte-identical to the house style, `~/Documents/area/tex-templates/notes/custom.sty`, and to the copies in [`nus/y2s1/cs2100`](../../../nus/y2s1/cs2100/) and [`cs3231`](../../../nus/y2s1/cs3231/) |
| `glossary.md` | The French-first term list — each glossed term's French form (the source's spelling), English gloss and the one chapter that glosses it, plus the terms used as they stand. See [the 2026-09-21 spec](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-21-french-first-notes-design.md) |
| `chapters/0-prerequis.tex` | Prérequis — binary and hexadecimal, endianness, complément à deux, ASCII, memory units |
| `chapters/1-introduction-compilateurs.tex` | Séance 1 — what a compiler is, the pipeline from lexing to ELF, the GCC walk-through |
| `chapters/2-assembleur-x86.tex` | Séance 1 — the memory model, the ISA, registers and sub-registers, addressing modes, GAS sections, arithmetic, bitwise, jumps and flags, syscalls, and the methodology. Carries the séance-1 exercise corrigés as worked examples |
| `chapters/2a-aide-memoire-x86-64.tex` | The x86-64 reference sheet — after chapter 2, on three pages of its own, unnumbered so chapters 3–6 keep their numbers. Modelled on Stanford CS107's [*x86-64 Reference Sheet*](https://web.stanford.edu/class/cs107/resources/x86-64-reference.pdf) and written rather than embedded: everything on Stanford's sheet, in the course's caller-/callee-saved terms, plus the syscalls, directives, calling convention and toolchain the séances teach. Design: [`2026-09-21-ece-3tc32-x86-reference-sheet-design.md`](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-21-ece-3tc32-x86-reference-sheet-design.md) |
| `chapters/3-rappels-c.tex` | Séance 2 — types and where variables live, functions, pointers and pointer arithmetic, arrays and strings, printf/scanf formats, 2D and linearised arrays |
| `chapters/4-fonctions-pile-libc.tex` | Séance 2 — memory layout, the stack frame (drawn), the System V calling convention, the argument registers, the alignment rule before a call, and calling into the libC |
| `chapters/5-grammaires-analyse-syntaxique.tex` | Séance 3 — formal and context-free grammars, derivation trees, ambiguity (dangling else, precedence, associativity), binarisation, the CYK trace the deck runs by hand, and top-down LL(1) analysis with Null/Premier/Suivant |
| `chapters/6-langages-reguliers-analyse-lexicale.tex` | Séance 3 — regular languages and expressions, the `match` equations, automata, the lexeur with its two tie-breaks, `ocamllex`, and a closing subsection on the TP Lexeur interface derived from the two extension files |
| `src/ascii-table.pdf` | The US-ASCII chart chapter 0 includes — a vector drawing of the public-domain chart, found through the main file's `\graphicspath{{./src/}}` |

Two chapters per séance, which is what the decks support — séance 3's deck alone
is 37 slides over 89 pages. **Séance 4 has no chapter yet**, and it is the first
séance whose deck is held while its notes are not: `cours-s4-parsing-lr-2026-27.pdf`
is 30 slides over 145 pages of LR parsing, which chapter 5 reaches only as far as
LL(1) descent. The séquençage's remaining blocks (portes logiques combinatoires
and synchrones, génération de code, projet compilateur) have no deck either, and
none of the four has a stub chapter; they get chapters when they are taught. Build with `latexmk -pdf` from inside this directory, which is where
`custom.sty` has to be found. The built PDF is committed; the `.aux` and `.log` are not.

Three places where the notes go beyond the decks, none of them marked in the text,
since the notes cite no source (see the
[French-first spec](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-21-french-first-notes-design.md)).
Chapter 5 supplies an answer to the page-53 *rendre la grammaire LL(1)* exercise, for
which the deck publishes no corrigé, and answers two questions the deck poses
rhetorically and never returns to. The reference sheet carries everything on
Stanford's sheet whether or not a deck teaches it — the unsigned `divq`, `cqto` and
`%cl` shift counts are in no deck.

