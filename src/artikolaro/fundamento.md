# Fundamento - *The Zen of Zig*

Ĉi tiu artikolo esploras la kernajn principojn de Zig nomatajn "Zen of Zig". Ili ĉefe gvidas la
ellaboron de Zig mem, kaj povas agi kiel "fundamento" por ziguzantoj. Vi povas vidi ilin per la
komando `zig zen`:

```
$ zig zen

 * Communicate intent precisely.
 * Edge cases matter.
 * Favor reading code over writing code.
 * Only one obvious way to do things.
 * Runtime crashes are better than bugs.
 * Compile errors are better than runtime crashes.
 * Incremental improvements.
 * Avoid local maximums.
 * Reduce the amount one must remember.
 * Focus on code rather than style.
 * Resource allocation may fail; resource deallocation must succeed.
 * Memory is a resource.
 * Together we serve the users.

```

Esperante:

```
 * Precize komuniku la intencon.
 * Randkazoj gravas.
 * Zorgu pri kodlegado pli ol kodskribado.
 * Estu nur unu evidenta maniero por fari ion.
 * Rultempa halto pli bonas ol cimo.
 * Traduktempa halto pli bonas ol rultempa halto.
 * Iom-post-iomaj plibonigoj.
 * Evitu lokalajn maksimumojn.
 * Reduktu kiom oni memoru.
 * Kodkvalito gravas pli ol kodstilo.
 * Akiro povu erari; malakiro sukcesu.
 * Memoro estas provizo.
 * Kune ni servu la uzantojn.
```

Ĉiu principo havas dediĉan sekcion, kiu klarigas ĝin, donas ekzemplojn de kiel Zig aplikas ĝin aŭ
kiel ziguzantoj povas fasoni iliajn programojn laŭ ĝi, kaj komparas ĝin al principoj de aliaj
programlingvoj.

## Precize Komuniku Intencon

Ĉi tiu principo signifas, ke gravas ne nur la funkcio de kodo sed ankaŭ ĝia intenco estu klare
komunikata. Estas multaj ekzempletoj en la fasono de Zig.

### Tipoj de funkcio

La tipoj de funkcio en Zig estas bonaj ekzemploj de klareco kaj formala komunikado de intenco. Ili
sole klarigas:

- ĉu la funkcio povas erari (ĉu ĝi donas erarunuiĝon),

```zig
// ĉi tia funkcio sukcesu
fn function1(parameter: Parameter) Result {
   // ...
}

// ĉi tia funkcio povas erari
fn function2(parameter: Parameter) Error!Success {
   // ...
}
``` 

- ĉu la funkcio uzas paŭzajn operaciojn (ĉu ĝi bezonas `std.Io` parametron),

```zig
// ĉi tia funkcio verŝajne ne uzas paŭzajn operaciojn
fn function1(parameter: Parameter) Result {
   // ...
}

// ĉi tia funkcio povas uzi paŭzajn operaciojn
fn function2(pameter: Parameter, io: std.Io) Result {
   // ....
}
```

- ĉu la funkcio asignas memoron (ĉu ĝi bezonas `std.mem.Allocator` parametron),

```zig
// ĉi tia funkcio verŝajne ne asignas memoron
fn function1(parameter: Parameter) Result {
   // ...
}

// ĉi tia funkcio povas asigni memoron
fn function2(parameter: Parameter, allocator: std.mem.Allocator) Result {
   // ...
}
```

### Nestruktura Tipado

Zig uzas nestruktura tipadon por `enum`, `opaque`, `struct` kaj `union` tipoj. Tio signifas, ke eĉ
kiam ili havas tute similan difinon, du tiaj tipoj ne estas la samaj. Ekzemple:

```zig
const Enum1 = enum(u8) {
   variant_1,
   variant_2,
};

const Enum2 = enum(u8) {
   variant_1,
   variant_2,
};

comptime {
   @import("std").debug.assert(Enum1 != Enum2);
}
```

Tio devigas la programanton uzi malsamajn tipojn por malsamaj uzoj, eĉ kiam ili hazarde similas.

### Dokumentaro

Zig permesas al komentoj esti "dokumentaj". Dokumentaj komentoj aperas en aŭtoproduktita
dokumentaro. La [dokumentaro de la standarda libraro] estas bona ekzemplo, de kiel aperas
aŭtoproduktita dokumentaro. Vi ankaŭ povas vidi ĝin lokale per la komando `zig std`.

Por aŭtoprodukti dokumentaron, iru al la `build.zig` de via projekto, en la `build(b: *std.Build)`
funkcio. Elektu kies `std.Build.Step.Compile` dokumentaron vi volas produkti, kaj skribu tion:

```zig
    ...
    const doc = b.addInstallDirectory(.{
        .install_dir = .prefix,
        .install_subdir = "doc",
        .source_dir = my_compile.getEmittedDocs(),
    });

    const doc_step = b.step("doc", "The step to emit the documentation about `my_compile`");
    doc_step.dependsOn(&doc.step);
    ...
```

Tiam vi povas uzi `zig build doc` por produkti la dokumentaron en `zig-out/doc/`. La dokumentaro
ankoraŭ ne estas facila por legi. Mi uzas `python -m http.server -d zig-out/doc` por tio.

FAROTA: pli bona klarigo pri kiel uzi aŭtoprodukton de dokumentaro.

[dokumentaro de la standarda libraro]:https://ziglang.org/documentation/master/std/


## Randkazoj Gravas

Randkazo estas aparta kazo, kiam iu valoro estas ekstrema aŭ valorkombino igas la programkonduton
speciala.

Plej programlingvoj 

## Zorgu pri Kodlegado pli ol Kodskribado

FAROTA

## Estu nur Unu Evidenta Maniero por Fari Ion

FAROTA

## Rultempa Halto pli Bonas ol Cimo

FAROTA

## Traduktempa Halto pli Bonas ol Rultempa Halto

FAROTA

## Iom-post-iomaj plibonigoj

FAROTA

## Evitu lokalajn maksimumojn

FAROTA

## Reduktu kiom Oni Memoru

FAROTA

## Kodkvalito Gravas pli ol Kodstilo

FAROTA

## Akiro Povu Erari; Malakiro Sukcesu

FAROTA

## Memoro Estas Provizo

FAROTA

## Kune Ni Servu la Uzantojn

FAROTA


