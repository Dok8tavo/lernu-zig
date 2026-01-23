# Enkonduko

Saluton kara leganto,

La celo de ĉi tiu libro estas instrui programadon kaj la [programlingvon] "[Zig]". Ĝi enhavos tri
partojn kun malsamaj celo, publiko, kaj uzo.

La unua parto *lecionaro* estas orda vico de lecionoj por lerni programadon. Vi ne bezonas iun ajn
sperton por legi ĝin. Vi nur bezonas komputilon kun interreto, klavaro, muso (nedeva), kaj vian
cerbon. Ĉi tiu parto plej taŭgas por senspertaj programontoj. Ĝi enhavas detalojn pri multaj
bazaĵoj kiel kodredaktilo, kodtradukilo, komandlinio, rulado, ktp, kies klarigo estus malnecesa
por spertaj programantoj.

La dua parto *artikolaro* estas senorda kolekto da artikoloj pri specifaj temoj ĉirkaŭ Zig kaj
programado. Ili necesas sperton je almenaŭ unu programlingvo. Ili ne klarigas la sintakson de Zig
kaj ĝeneralajn programajn konojn, krom kiam ili specife temas pri tio. Senspertulo legu
*lecionaro*n antaŭ *artikolaro*n.

La tria parto *vortaro* estas... Vortaro. Ĝi enhavas mallongajn difinojn de teknikaj vortoj, ilian
anglan tradukon, kelkajn ekzemplojn, ktp. Mi esperas ke ĉi tiu vortaro utilu se vi verkas pri
programado esperante. Mi volonte aldonu al ĝi laŭ peto, ne hezitu fari peton ĉe [GitHub].


## Pri Zig

[Zig] estas ĝeneraluza programlingvo kaj ilĉeno por ellabori kaj daŭrigi fortikajn, optimumajn
[^optimumajn] programaĵojn. Ĝi estas publikigita en 2015, kaj daŭre malferme kodata de senprofita
korporacio [ZSF].


Mi elektis ĝin kiel lerna programlingvo pro la jenaj kialoj:

- La fundamenta principo "kune ni servu la uzantojn", la malfermeco kaj senprofiteco, igas Zig
"esperanteca".

- La fasono de Zig estas ideala kompromiso por lerni. Ĝi donas plenan kontrolon al la programanto,
kiel C aŭ C++, samtempe devigas malsekuraĵojn esti malimplica[^implica], kiel Rust, samtempe resti
simpla, kiel C aŭ Go aŭ Python. Tia fasono lernigas programanton pri malsimplaĵoj kutime kaŝitaj,
plej sekure kaj simple kiel eble.

- Mi plej ŝatas programi per Zig. Mi ĉiam scias kaj komprenas tion, kio okazas. Zig juste gratulas
miajn sukcesojn, kaj malgratulas miajn malsukcesojn.


Mi ankaŭ elektis ĝin malgraŭ la jenaj punktoj:

- Pro ĝia noveco, ekzistas malmulte da lernorimedoj. Ĉi tiu lernolibro estu plena.

- Zig estas daŭre ellaborata kaj daŭre ŝanĝas. La libro estu ĝisdatigata.


## Pri Mi

Saluton! Mi estas Dok8tavo (Dok Oktavo)! Mi ne estas programisto (*ŝokita vizaĝo*). Programado estas
por mi simpla sed kara ŝatokupo. Mi ja pensas, ke mi havas sufiĉan sperton por paroli pri kelkajn
programajn subjektojn ---ĉefe tiujn pri kiuj mi artikolumos--- sed mi verŝajne malpravos, fuŝos,
misos, dum la verkado. Se vi trovas eraron, bonvole diru al mi, plejŝatate per [GitHub].

Mia celoj verkante *Lernu Zig* ĉefe estas:

- diskonigi kaj instrui programadon,
- diskonigi kaj instrui Zig,
- riĉigi la esperantan verkaron,
- praktiki Esperanton,

Mia pronomo estas "li" aŭ "ĝi". Mi uzas ĝiismon[^ĝiismo] kaj iĉismon[^iĉismo] tra la tuta libro.
Mi deziras al vi bonan legon, kaj ĝojan vojaĝon dum la lernado de programado.


## Pri AI

Ĉi tiu sekcio flanktemas pri *Artefaritaj Inteligentoj* (AI), kaj pli specife 
*Larĝaj Lingvaj Modeloj* (LLM) kiel [ChatGPT], [Claude], [Llama] aŭ [Copilot], kiuj nove famiĝis
kaj koniĝis de la publiko, pro subita kaj spektinda pliboniĝo. Iliaj uzkazoj multobligis kaj la 
programkomunumo naskis ideon antaŭe nekredeblan: anstataŭi homajn programistojn per LLMaj
programiloj.

Mi tute ne estas kontraŭ-LLMa. Mi pensas ke ili estas mirindaj iloj, kapablaj de grandaj ŝanĝoj
al programado, al homaro. Mi ankaŭ opinias ke la plejparto de entuziasmaj ideoj pri anstataŭi
programistojn, forigi fontkodon ---eĉ parte---[^longstriko] ktp, estas misciaj kaj danĝeraj.

Mi ne klarigu plene kial mi pensas tion. Mi nur volas diri, ke *Lernu Zig* estas nek pri, nek por,
nek per[^per-llm] LLMoj. Ĝi estas verko de homo, kies celpubliko estas homoj, kies temo estas
programado sen LLMaj iloj. Mi ne planas nek kontraŭas la ideon de artikolo pri LLMoj kiel
programiloj, iliaj uzkazoj, kaj danĝeroj.


[Zig]:https://ziglang.org
[ZSF]:https://ziglang.org/zsf
[ChatGPT]:https://chatgpt.com
[Claude]:https://claude.ai
[Copilot]:https://copilot.microsoft.com
[GitHub]:https://github.com/Dok8tavo/lernu-zig
[Llama]:https://llama.com

[artiklaro]:artikolaro/
[lecionaro]:lecionaro/
[vortaro]:vortaro/_index.md
[programlingvon]:vortaro/_index.md#programlingvo

[^optimumajn]: Optimuma: plej bonkvalita, laŭ difinaj kriterioj, en difinaj limoj kaj
cirkonstancoj.

[^longstriko]: Se vi kredas, ke longstrikoj kiel "---" indikas, ke mi uzis LLMon por skribi aŭ
verki la libron, vi malpravas. Jen kiel ili aspektas por mi en la fontkodo de la libro: `---` 😉
[^miensimbolo].

[^miensimbolo]: Se vi kredas, ke miensimboloj kiel "😉" indikas, ke mi uzis LLMon por skribi aŭ
verki la libron, vi malpravas. Jen kiel ili aspektas por mi en la fontkodo de la libro: `:wink:` 👅.

[^ĝiismo]: Tio signifas, ke kiam mi ne konas ies pronomo, mi uzas "ĝi". Tio **ne** signifas, ke mi
traktas tiun personon aŭ pensas pri tiu persono kiel objekto. Kaj mi kompreneble ne uzas "ĝi" por
personoj kiuj sciigis min iamaniere, ke ili malŝatas tion.

[^iĉismo]: Tio signifas, ke mi esprimas masklecon per sufiksado de "-iĉ", anstaŭ prefiksado de
"vir-" aŭ per defaŭlta formo. Kiam mi uzas defaŭltan formon, tiam mi esprimas ajnan genron. Kiam mi
prefiksas "ge-", tiam mi esprimas almenaŭ maslkan kaj femalan genrojn.

[^per-llm]: Mi ja uzas LLMon verkante la libron, ekzemple por sugesti subjekton de artikolo aŭ
paragrafo. Mi ankaŭ uzas ĝin kiel korektilo: ĝi trovu mistajpojn, akuzativforgesojn, ktp. Sed ĉiu
teksta kaj koda linio estas homverkita.

[^simpla]: Laŭ la vidpunkto, ke la lingvo malkovras malsimplaĵojn per facadoj. 
