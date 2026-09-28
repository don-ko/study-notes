# Glossaire — ECE 3TC32: Compilation

The French-first rule's term list for these notes
([spec](https://github.com/don-ko/telecom/blob/main/docs/superpowers/specs/2026-09-21-french-first-notes-design.md)).
Each term below is glossed exactly once, in its Home chapter, as
`\textbf{terme} (\textit{English})` — or as `terme (\textit{English})` when the
gloss sits in a definition's or theorem's title — and appears in French alone
everywhere else. Section is the innermost heading over the gloss in the notes;
Source is where the source introduces the term. A chapter written later glosses
only a term not yet in this table, and adds it here. Compilation chapters 0 to 2.3, the
hand-written reference, keep their own gloss forms (chapter 1's plain
`compilateur (\textit{compiler})`, for one). Chapter 5 glosses Premier and Suivant on
their math names, `$\mathit{Suivant}(X)$ (\textit{follow})`.

| Terme | English | Home | Section | Source |
|---|---|---|---|---|
| grand-boutien | big-endian | 0-prerequis.tex | Endianness (petit-boutien / grand-boutien) | cours-s1-introduction-generale-2026-27 p. 31 |
| petit-boutien | little-endian | 0-prerequis.tex | Endianness (petit-boutien / grand-boutien) | cours-s1-introduction-generale-2026-27 p. 31 |
| complément à deux | two's complement | 0-prerequis.tex | Complément à deux | cours-s1-introduction-generale-2026-27 p. 34 |
| compilateur | compiler | 1-introduction-compilateurs.tex | Compilateurs | cours-s1-introduction-generale-2026-27 p. 15 |
| analyse lexicale | lexing | 1-introduction-compilateurs.tex | Analyse lexicale | cours-s1-introduction-generale-2026-27 p. 18 |
| lexème | token | 1-introduction-compilateurs.tex | Analyse lexicale | cours-s1-introduction-generale-2026-27 p. 18 |
| analyse syntaxique | parsing | 1-introduction-compilateurs.tex | Analyse syntaxique | cours-s1-introduction-generale-2026-27 p. 19 |
| arbre de syntaxe abstrait | Abstract Syntax Tree | 1-introduction-compilateurs.tex | Analyse syntaxique | cours-s1-introduction-generale-2026-27 p. 19 |
| analyse sémantique | semantic analysis | 1-introduction-compilateurs.tex | Analyse sémantique | cours-s1-introduction-generale-2026-27 p. 20 |
| élimination du code mort | dead code elimination | 1-introduction-compilateurs.tex | Optimisation | cours-s1-introduction-generale-2026-27 p. 21 |
| propagation des constantes | constant propagation | 1-introduction-compilateurs.tex | Optimisation | cours-s1-introduction-generale-2026-27 p. 22 |
| analyse des alias | alias analysis | 1-introduction-compilateurs.tex | Optimisation | cours-s1-introduction-generale-2026-27 p. 23 |
| dépliement de boucles | loop unrolling | 1-introduction-compilateurs.tex | Optimisation | cours-s1-introduction-generale-2026-27 p. 24 |
| analyse de vie | liveness analysis | 1-introduction-compilateurs.tex | Optimisation | cours-s1-introduction-generale-2026-27 p. 24 |
| sous-expressions communes | common subexpression elimination | 1-introduction-compilateurs.tex | Optimisation | cours-s1-introduction-generale-2026-27 p. 24 |
| fichier objet | object file | 1-introduction-compilateurs.tex | Assemblage | cours-s1-introduction-generale-2026-27 p. 26 |
| édition de liens | linking | 1-introduction-compilateurs.tex | Édition de liens | not in source |
| fichier binaire | binary file | 1-introduction-compilateurs.tex | Édition de liens | cours-s1-introduction-generale-2026-27 p. 27 |
| instruction set architecture | Instruction Set Architecture | 2-assembleur-x86.tex | Bases de x86-64 | cours-s1-premiers-pas-x86-2026-27 p. 7 |
| registre | register | 2-assembleur-x86.tex | Le Mémoire d'un Ordinateur | cours-s1-premiers-pas-x86-2026-27 p. 3 |
| RAM | Random Access Memory | 2-assembleur-x86.tex | Le Mémoire d'un Ordinateur | cours-s1-premiers-pas-x86-2026-27 p. 4 |
| pointeur d'instruction | instruction pointer | 2-assembleur-x86.tex | Le Programme | not in source |
| processus | process | 2-assembleur-x86.tex | Le Format Binaire | cours-s1-premiers-pas-x86-2026-27 p. 8 |
| exécutable | executable | 2-assembleur-x86.tex | Le Format Binaire | cours-s1-premiers-pas-x86-2026-27 p. 8 |
| sous-registre | subregister | 2-assembleur-x86.tex | Les Registres Généraux | cours-s1-premiers-pas-x86-2026-27 p. 12 |
| registre de drapeaux | flags register | 2-assembleur-x86.tex | Drapeaux utiles | cours-s1-premiers-pas-x86-2026-27 p. 31 |
| entrée standard | standard input | 2-assembleur-x86.tex | Interaction avec l'OS | cours-s2-rappels-c-2026-27 p. 23 |
| sortie standard | standard output | 2-assembleur-x86.tex | Interaction avec l'OS | cours-s1-premiers-pas-x86-2026-27 p. 38 |
| descripteur de fichier | file descriptor | 2-assembleur-x86.tex | Interaction avec l'OS | cours-s1-premiers-pas-x86-2026-27 p. 33 |
| décimal petit-boutien | little-endian decimal | 2-assembleur-x86.tex | Afficher un entier en décimal | cours-s1-premiers-pas-x86-2026-27 p. 43 |
| proche de la machine | close to the machine | 3-rappels-c.tex | Rappels de C | cours-s2-rappels-c-2026-27 p. 3 |
| impératif | imperative | 3-rappels-c.tex | Rappels de C | cours-s2-rappels-c-2026-27 p. 3 |
| passage par valeur | pass-by-value | 3-rappels-c.tex | Rappels de C | cours-s2-rappels-c-2026-27 p. 3 |
| statiquement typé | statically typed | 3-rappels-c.tex | Rappels de C | cours-s2-rappels-c-2026-27 p. 3 |
| pointeur | pointer | 3-rappels-c.tex | Pointeur | cours-s2-rappels-c-2026-27 p. 12 |
| modificateur | modifier | 3-rappels-c.tex | Types en C | cours-s2-rappels-c-2026-27 p. 4 |
| durée de vie | lifetime | 3-rappels-c.tex | Variable | cours-s2-rappels-c-2026-27 p. 5 |
| chaîne de caractères | string | 3-rappels-c.tex | Chaînes de caractères | cours-s2-rappels-c-2026-27 p. 22 |
| valeur gauche | left-value | 3-rappels-c.tex | Valeur gauche | cours-s2-rappels-c-2026-27 p. 11 |
| sucre syntaxique | syntactic sugar | 3-rappels-c.tex | Tableaux | cours-s2-rappels-c-2026-27 p. 18 |
| pile | stack | 4-fonctions-pile-libc.tex | Organisation de la mémoire | cours-s2-suite-x86-libc-fonctions-2026-27 p. 2 |
| valeur de retour | return value | 4-fonctions-pile-libc.tex | Où vont les arguments | not in source |
| appelant | caller | 4-fonctions-pile-libc.tex | Fonctions en assembleur | cours-s2-suite-x86-libc-fonctions-2026-27 p. 8 |
| mémoire statique | static memory | 4-fonctions-pile-libc.tex | Organisation de la mémoire | cours-s2-suite-x86-libc-fonctions-2026-27 p. 2 |
| tas | heap | 4-fonctions-pile-libc.tex | Organisation de la mémoire | cours-s2-suite-x86-libc-fonctions-2026-27 p. 2 |
| organisation de la pile pour les fonctions | stack discipline | 4-fonctions-pile-libc.tex | Organisation de la pile pour les fonctions | cours-s2-suite-x86-libc-fonctions-2026-27 p. 4 |
| fonction appelée | callee | 4-fonctions-pile-libc.tex | Fonctions en assembleur | cours-s2-suite-x86-libc-fonctions-2026-27 p. 7 |
| alignement | alignment | 4-fonctions-pile-libc.tex | Questions d'alignement | cours-s2-suite-x86-libc-fonctions-2026-27 p. 12 |
| registre d'argument | argument register | 4-fonctions-pile-libc.tex | Où vont les arguments | not in source |
| fonction variadique | variadic function | 4-fonctions-pile-libc.tex | Où vont les arguments | not in source |
| sauvegardé par l'appelé | callee-saved | 4-fonctions-pile-libc.tex | Registres sauvegardés par l'appelant et par l'appelé | not in source |
| zone rouge | red zone | 4-fonctions-pile-libc.tex | Questions d'alignement | not in source |
| sauvegardé par l'appelant | caller-saved | 4-fonctions-pile-libc.tex | Registres sauvegardés par l'appelant et par l'appelé | not in source |
| grammaire formelle | formal grammar | 5-grammaires-analyse-syntaxique.tex | Grammaires formelles | cours-s3-analyse-lexicale-2026-27 p. 2 |
| grammaire non contextuelle | context-free grammar | 5-grammaires-analyse-syntaxique.tex | Grammaires non contextuelles | cours-s3-analyse-lexicale-2026-27 p. 8 |
| problème de l'appartenance | membership problem | 5-grammaires-analyse-syntaxique.tex | Le problème de l'appartenance | cours-s3-analyse-lexicale-2026-27 p. 5 |
| symbole terminal | terminal symbol | 5-grammaires-analyse-syntaxique.tex | Grammaires formelles | cours-s3-analyse-lexicale-2026-27 p. 2 |
| symbole non-terminal | non-terminal symbol | 5-grammaires-analyse-syntaxique.tex | Grammaires formelles | cours-s3-analyse-lexicale-2026-27 p. 2 |
| symbole de départ | start symbol | 5-grammaires-analyse-syntaxique.tex | Grammaires formelles | cours-s3-analyse-lexicale-2026-27 p. 2 |
| règle de production | production rule | 5-grammaires-analyse-syntaxique.tex | Grammaires formelles | cours-s3-analyse-lexicale-2026-27 p. 8 |
| règle de réécriture | rewriting rule | 5-grammaires-analyse-syntaxique.tex | Grammaires formelles | cours-s3-analyse-lexicale-2026-27 p. 3 |
| indécidable | undecidable | 5-grammaires-analyse-syntaxique.tex | Le problème de l'appartenance | cours-s3-analyse-lexicale-2026-27 p. 6 |
| arbre de dérivation | derivation tree | 5-grammaires-analyse-syntaxique.tex | Arbre de dérivation | cours-s3-analyse-lexicale-2026-27 p. 9 |
| non-ambiguë | unambiguous | 5-grammaires-analyse-syntaxique.tex | Arbre de dérivation | cours-s3-analyse-lexicale-2026-27 p. 9 |
| associativité | associativity | 5-grammaires-analyse-syntaxique.tex | Gérer la précédence des opérateurs | cours-s3-analyse-lexicale-2026-27 p. 19 |
| point fixe | fixpoint | 5-grammaires-analyse-syntaxique.tex | Algorithme de reconnaissance | cours-s3-analyse-lexicale-2026-27 p. 61 |
| test linéaire | linear test | 5-grammaires-analyse-syntaxique.tex | Utilisation en pratique | cours-s3-analyse-lexicale-2026-27 p. 44 |
| descendante | top-down | 5-grammaires-analyse-syntaxique.tex | Analyse syntaxique descendante | cours-s3-analyse-lexicale-2026-27 p. 45 |
| factorisation à gauche | left factoring | 5-grammaires-analyse-syntaxique.tex | Pourquoi cela marche et peut-on généraliser ? | not in source |
| Suivant | follow | 5-grammaires-analyse-syntaxique.tex | Pourquoi cela marche et peut-on généraliser ? | cours-s3-analyse-lexicale-2026-27 p. 49 |
| Premier | first | 5-grammaires-analyse-syntaxique.tex | Pourquoi cela marche et peut-on généraliser ? | cours-s3-analyse-lexicale-2026-27 p. 49 |
| langage régulier | regular language | 5-grammaires-analyse-syntaxique.tex | De nombreuses classes\dots | cours-s3-analyse-lexicale-2026-27 p. 55 |
| automate | automaton | 6-langages-reguliers-analyse-lexicale.tex | Automates | cours-s3-analyse-lexicale-2026-27 p. 62 |
| opération rationnelle | rational operation | 6-langages-reguliers-analyse-lexicale.tex | Langages réguliers | cours-s3-analyse-lexicale-2026-27 p. 56 |
| monoïde fini | finite monoid | 6-langages-reguliers-analyse-lexicale.tex | Langages réguliers | cours-s3-analyse-lexicale-2026-27 p. 56 |
| logique | logic | 6-langages-reguliers-analyse-lexicale.tex | Langages réguliers | cours-s3-analyse-lexicale-2026-27 p. 56 |
| langage associé | associated language | 6-langages-reguliers-analyse-lexicale.tex | Le langage associé | cours-s3-analyse-lexicale-2026-27 p. 59 |
| automate fini déterministe | deterministic finite automaton | 6-langages-reguliers-analyse-lexicale.tex | Automates | cours-s3-analyse-lexicale-2026-27 p. 62 |
| état | state | 6-langages-reguliers-analyse-lexicale.tex | Automates | cours-s3-analyse-lexicale-2026-27 p. 62 |
| état final | final state | 6-langages-reguliers-analyse-lexicale.tex | Automates | cours-s3-analyse-lexicale-2026-27 p. 62 |
| état initial | initial state | 6-langages-reguliers-analyse-lexicale.tex | Automates | cours-s3-analyse-lexicale-2026-27 p. 62 |
| fonction de transition | transition function | 6-langages-reguliers-analyse-lexicale.tex | Automates | cours-s3-analyse-lexicale-2026-27 p. 62 |
| accepté | accepted | 6-langages-reguliers-analyse-lexicale.tex | Automates | cours-s3-analyse-lexicale-2026-27 p. 62 |
| état puits | sink state | 6-langages-reguliers-analyse-lexicale.tex | Automates | not in source |
| plus grand préfixe | maximal munch | 6-langages-reguliers-analyse-lexicale.tex | L'algorithme, formellement | cours-s3-analyse-lexicale-2026-27 p. 84 |
| priorité de la règle | rule priority | 6-langages-reguliers-analyse-lexicale.tex | L'algorithme, formellement | not in source |

## Sans glose

Terms used as they stand, never glossed. The French-alone rule covers the
glossed terms above; in English prose a term below may also appear as its
English equivalent.

| Term | Source |
|---|---|
| binaire | cours-s1-introduction-generale-2026-27 p. 29 — unglossed in the frozen chapters |
| hexadécimal | cours-s1-introduction-generale-2026-27 p. 30 — unglossed in the frozen chapters; differs from hexadecimal only by an accent and a final -e |
| octet | cours-s1-introduction-generale-2026-27 p. 35 — unglossed in the frozen chapters |
| adresse | cours-s1-premiers-pas-x86-2026-27 p. 5 — unglossed in the frozen chapters |
| signé | cours-s1-premiers-pas-x86-2026-27 p. 14 — unglossed in the frozen chapters (with non signé) |
| mémoire | cours-s1-premiers-pas-x86-2026-27 p. 2 — unglossed in the frozen chapters |
| mot | cours-s1-introduction-generale-2026-27 p. 35 — unglossed in the frozen chapters; also the mot of a langage (cours-s3-analyse-lexicale-2026-27 p. 3) |
| quad | cours-s1-introduction-generale-2026-27 p. 35 — the source's own word |
| langage | cours-s1-introduction-generale-2026-27 p. 15 — unglossed in the frozen chapters |
| interpréteur | not in source — unglossed in the frozen chapters |
| AST | cours-s1-introduction-generale-2026-27 p. 20 — the source's own abbreviation |
| optimisation | cours-s1-introduction-generale-2026-27 p. 21 — unglossed in the frozen chapters |
| génération de code | cours-s1-introduction-generale-2026-27 p. 3 — unglossed in the frozen chapters |
| assemblage | not in source — unglossed in the frozen chapters |
| analyse | cours-s1-introduction-generale-2026-27 p. 18 — unglossed in the frozen chapters |
| expression régulière | cours-s1-introduction-generale-2026-27 p. 18 — unglossed in the frozen chapters |
| lexeur | cours-s1-introduction-generale-2026-27 p. 14 — unglossed in the frozen chapters |
| grammaire | cours-s1-introduction-generale-2026-27 p. 19 — unglossed in the frozen chapters |
| dead store | cours-s1-introduction-generale-2026-27 p. 24 — the source's own English |
| synthèse | not in source — unglossed in the frozen chapters |
| code assembleur | cours-s1-introduction-generale-2026-27 p. 25 — unglossed in the frozen chapters |
| directive | not in source — unglossed in the frozen chapters; same word in English |
| assembleur | cours-s1-premiers-pas-x86-2026-27 p. 7 — unglossed in the frozen chapters |
| pipeline | not in source — used as is in the frozen chapters |
| ISA | cours-s1-premiers-pas-x86-2026-27 p. 7 — the source's own abbreviation |
| programme | cours-s1-premiers-pas-x86-2026-27 p. 5 — unglossed in the frozen chapters |
| case | cours-s1-premiers-pas-x86-2026-27 p. 14 — unglossed in the frozen chapters |
| syscall | cours-s1-premiers-pas-x86-2026-27 p. 5 — the source's own word |
| registre général | cours-s1-premiers-pas-x86-2026-27 p. 11 — unglossed in the frozen chapters |
| adressage virtuel | cours-s1-premiers-pas-x86-2026-27 p. 15 — unglossed in the frozen chapters |
| mémoire virtuelle | cours-s1-premiers-pas-x86-2026-27 p. 15 — unglossed in the frozen chapters |
| mémoire physique | cours-s1-premiers-pas-x86-2026-27 p. 15 — unglossed in the frozen chapters |
| label | cours-s1-premiers-pas-x86-2026-27 p. 18 — the source's own word |
| casting | cours-s1-premiers-pas-x86-2026-27 p. 23 — the source's own word |
| prologue | not in source — same word in English |
| epilogue | not in source — the notes write the English form, which differs from épilogue only by an accent |
| libC | cours-s2-rappels-c-2026-27 p. 23 — the source's own word (« pour C library et donc bibliothèque C ») |
| variable | cours-s2-rappels-c-2026-27 p. 5 — same word in English |
| frame | cours-s2-suite-x86-libc-fonctions-2026-27 p. 8 — the source's own word |
| format | cours-s2-rappels-c-2026-27 p. 24 — same word in English |
| LL(1) | cours-s3-analyse-lexicale-2026-27 p. 50 — the source's own notation |
| CFG | cours-s3-analyse-lexicale-2026-27 p. 8 — the source's own abbreviation (Context-Free Grammar) |
| précédence | cours-s3-analyse-lexicale-2026-27 p. 18 — differs from precedence only by accents |
| binarisation | cours-s3-analyse-lexicale-2026-27 p. 20 — same word in English |
| match | cours-s3-analyse-lexicale-2026-27 p. 23 — the source's own name |
| Null | cours-s3-analyse-lexicale-2026-27 p. 49 — the source's own name |
