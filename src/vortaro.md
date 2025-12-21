# Vortaro

| Esperanto       | Angla                | Difino                                                                    | Ekzemplo                           |
|-----------------|----------------------|---------------------------------------------------------------------------|------------------------------------|
| amaso           | heap                 | Nefiksa parto de la memoro de ekzekutaĵo.                                 |                                    |
| apo             | app, application     | Programo aŭ kolekto da kunlaborantaj programoj, rekte uzata de homoj.     |                                    |
| bajto           | byte                 | Plej eta grupo de bitoj kiun la maŝino traktas kiel unuon.                | Kutime okbito                      |
| bito            | bit                  | Plej eta ero de informacio. Kutime esprimata per aŭ 0 aŭ 1 nombro.        |                                    |
| ĉefprocesoro    | Central Process Unit | Ĉefa procesoro kiu regas la ekzekuton de la vico da instrukcioj.          |                                    |
| ekzekuto        | execution            | Plenumo de programo.                                                      |                                    |
| flankaparato    | peripheral           | Aparato por enigi aŭ eligi datenojn de komputilo.                         | muso, klavaro, ekrano, ...         |
| grafikprocesoro | Graphic Process Unit | Procesoro kiu regas ekzekuton de instrukcioj specaj por grafikoj          |                                    |
| instrukcio      | instruction          | Nedividebla simpla tasko kiun la maŝino povas plenumi.                    | Adicii du nombrojn, ...            |
| kodo            | code                 | Pura teksto en programlingvo, tradukota al ekzekutebla lingvo.            |                                    |
| kodredaktilo    | code editor          | Apo por redakti kodon.                                                    | VSCode, Emacs, vim, Helix, ...     |
| kodtradukilo    | compiler, transpiler | Apo por traduki kodon el programlingvo al ekzekutebla lingvo.             | Zig, clang, gcc, Go, CPython, PyPy |
| komputilo       | computer             | Fizika maŝino kun procesoro kaj skribebla memoro.                         | Ofickomputilo, smartfono, ...      |
| lingvoservilo   | language server      | Programo uzata de kodredaktilo por provizi taŭgan helpon por la kodo.     | ZLS                                |
| operaciumo      | operating system, OS | Superprogramo kiu regas komputilon, ĝiaj programojn, flankaparatojn, ktp. | Windows, MacOS, Android...         |
| procesoro       | processor            | Fizika maŝinero kiu interpretas la instrukciojn.                          | ĉefprocesoro, grafikprocesoro      |
| programo        | programo             | Vico de instrukcioj, kune farante nesimpla ago.                           | Apo, sito, operaciumo, ...         |
| programlingvo   | programming language | Formala lingvo tajpebla kaj legebla de homo por esprimi programon.        | Zig, C, Go, Java, Python, ...      |
| stako           | stack                | Fiksa parto de la memoro de ekzekutaĵo.                                   |                                    |

## Apo vs Programo

La malsameco inter apo kaj programo ne estas bone difinita. Ĝenerale apo rekte interagas kun homaj
uzantoj. Ne necesas ke programo interagu kun homaj uzantoj, ĝi povas esti uzata de aliaj programoj
ekzemple.

Ĉiu apo estas programo aŭ kolekto da programoj, sed ne ĉiu programo estas apo.

Oni kutime ne kondsideras operaciumoj kiel apoj.

## Programlingvo vs Kodtradukilo

Kodtradukiloj kutime tradukas el nur unu programlingvo. Kaj ili foje estas la ununura kodtradukilo
por ilia programlingvo. Ili tiam ofte nomiĝas same kiel la programlingvo.

Ekzemploj:
- Zig programlingvo: `zig`,
- Go programlingvo: `go`,

Kontraŭ-ekzemploj:
- C programlingvo: `clang` , `gcc`, `tcc`, ...
- Python programlingvo: `CPython`, `PyPy`, ...
- Rust programlingvo: `rustc`
