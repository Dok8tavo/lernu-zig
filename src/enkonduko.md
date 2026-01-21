# Enkonduko

Saluton kara leganto,

La celo de ĉi tiu libro estas instrui programadon kaj la programlingvon "Zig". Ĝi enhavos tri
partojn kun malsamaj celo, publiko, kaj uzo.

La unua parto *lecionaro* estas orda vico de lecionoj por lerni programadon. Vi ne bezonas iun ajn
sperton por legi ĝin. Vi nur bezonas komputilon kun interreto, klavaro, muso (nedeva), kaj vian
cerbon. Ĉi tiu parto plej taŭgas por senspertaj programontoj. Ĝi enhavas detalojn pri multaj
bazaĵoj kiel kodredaktilo, kodtradukilo, komandlinio, rulado, ktp, kies klarigo estus malnecesa
por spertaj programantoj.

La dua parto *artikolaro* estas senorda kolekto de artikoloj pri specifaj temoj ĉirkaŭ Zig kaj
programado. Ili necesas sperton en almenaŭ unu programlingvo. Ili plejparte ne klarigos la
sintakson de Zig kaj ĝeneralajn programajn konojn. Senspertulo legu *lecionaro*n antaŭ
*artikolaro*n.

La tria parto *vortaro* estas... Vortaro. Ĝi enhavas mallongajn difinojn de teknikaj vortoj, ilian
anglan tradukon, kelkajn ekzemplojn, ktp. Mi esperas ke ĉi tiu vortaro utilu se vi verkas pri
programado esperante. Mi volonte aldonu al ĝi laŭ peto, ne hezitu fari peton ĉe [GitHub].


## Pri Zig

Zig estas nova programlingvo, publikigita en 2015. Ĝi estas malferme kodata de senprofita
korporacio. Male al multaj programlingvoj, ĝi valoras malkovri ĉion por la programanto. Tio
signifas, ke la programanto pli bone kontrolas kiel programo agas, sed estas pli


## Pri Mi

Saluton! Mi estas Dok8tavo (Dok Oktavo)! Mi ne estas programisto (*ŝokita vizaĝo*). Programo estas
por mi simpla sed kara ŝatokupo. Mi ja pensas, ke mi havas sufiĉan sperton por paroli pri kelkajn
programajn subjektojn ---ĉefe tiujn pri kiuj mi artikolumos--- sed mi verŝajne malpravos, fuŝos,
misos, dum la verkado. Se vi trovas eraron, bonvole diru al mi, plejŝatate per [GitHub].

Mia celoj verkante *Lernu Zig* ĉefe estas:

- diskonigi kaj instrui programadon,
- diskonigi kaj instrui Zig,
- praktiki Esperanton,

Mia pronomo estas "li" aŭ "ĝi". Mi uzas ĝiismon[^ĝiismo] kaj iĉismon[^iĉismo] tra la tuta libro.
Mi deziras al vi bonan legon, kaj ĝojan vojaĝon dum la lernado de programado.


## Pri AI

Se ĉi tiu sekcio ŝajnas kiel flanktemon kaj vi ne kuriozas pri ĝi, tiam vi ne bezonas legi tion.
Ĝi ja estas flanktemo, kaj mi ne plu mencias AI dum la tuta libro, krom eventuala artikolo specife
pri ĝi.

*Artefaritaj Inteligentoj* (AI), kaj pli specife *Larĝaj Lingvaj Modeloj* (LLM) kiel [ChatGPT],
[Claude], [Llama] aŭ [Copilot], nove famiĝis kaj koniĝis de la publiko, pro subita kaj spektinda
pliboniĝo. Iliaj uzkazoj multobligis kaj la programkomunumo naskis ideon antaŭe nekredeblan:
anstataŭi homajn programistojn per LLMaj programiloj.

Mi tute ne estas kontraŭ-LLMa. Mi pensas ke ili estas mirindaj iloj, kapablaj de grandaj ŝanĝoj
al programado, al homaro. Mi ankaŭ opinias ke la plejparto de entuziasmaj ideoj pri anstataŭi
programistojn, forigi fontkodon ---eĉ parte---[^longstriko] ktp, estas misciaj kaj danĝeraj.

Mi ne klarigu plene kial mi pensas tion. Mi nur volas diri, ke *Lernu Zig* estas nek pri, nek por,
nek per[^per-llm] LLMoj. Ĝi estas verko de homo, kies celpubliko estas homoj, kies temo estas
programado sen LLMaj iloj. Mi ne planas nek kontraŭas la ideon de artikolo pri LLMoj kiel
programiloj, iliaj kazuzoj, kaj danĝeroj.



[ChatGPT]:https://chatgpt.com
[Claude]:https://claude.ai
[Copilot]:https://copilot.microsoft.com
[GitHub]:https://github.com/Dok8tavo/lernu-zig
[Llama]:https://llama.com

[artiklaro]:artikolaro/
[lecionaro]:lecionaro/
[vortaro]:vortaro/_index.md

[^longstriko]: Se vi kredas, ke longstrikoj kiel "---" indikas, ke mi uzis LLMon por skribi aŭ
verki la libron, vi malpravas. Jen kiel ili aspektas por mi en la fontkodo de la libro: `---` 😉
[^miensimbolo].

[^miensimbolo]: Se vi kredas, ke miensimboloj kiel "😉" indikas, ke mi uzis LLMon por skribi aŭ
verki la libron, vi malpravas. Jen kiel ili aspektas por mi en la fontkodo de la libro: `:wink:` 👅.

[^ĝiismo]: Tio signifas, ke kiam mi ne konas ies pronomo, mi uzas "ĝi". Tio **ne** signifas, ke mi
traktas tiun personon aŭ pensas pri tiu persono kiel objektoj. Kaj mi kompreneble ne uzas "ĝi" por
personoj kiuj sciigis min iamaniere, ke ili ne ŝatas tion.

[^iĉismo]: Tio signifas, ke mi esprimas masklecon per sufiksado de "-iĉ", anstaŭ prefiksado de
"vir-" aŭ per defaŭlta formo. Kiam mi uzas defaŭltan formon, tiam mi esprimas ajnan genron. Kiam mi
prefiksas "ge-", tiam mi esprimas almenaŭ maslkan kaj femalan genrojn.

[^per-llm]: Mi ja uzas LLMon verkante la libron. Ekzemple por sugesti subjekton de artikolo aŭ
paragrafo. Mi ankaŭ uzas ĝin kiel korektilo: ĝi trovu mistajpojn, akuzativforgesojn, ktp. Sed ĉiu
teksta kaj koda linio estas homverkita.

[^simpla]: Laŭ la vidpunkto, ke la lingvo malkovras malsimplaĵojn per facadoj. 
