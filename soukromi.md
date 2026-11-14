---
title: TaSchránka — Zásady ochrany soukromí
---

# TaSchránka — Zásady ochrany soukromí

*Platné od 14. listopadu 2026* · [English](privacy)

**Stručně:** všechno, co aplikace ukládá, zůstává na vašem počítači. Autor aplikace z toho nedostává nic. Žádný účet, žádný cloud, žádná reklama, žádná analytika. Jediné, co aplikace kdy pošle po síti, je název domény webu kvůli stažení jeho ikony; podrobnosti níže.

## Co aplikace čte

Aplikace má dvě úlohy a každá potřebuje něco číst:

- **Historie schránky.** Když něco zkopírujete, aplikace si uloží kopii: text, obrázky a další obsah schránky.
- **Automatické ukládání textových polí.** Zatímco píšete do textového pole v jiné aplikaci, ukládá jeho text, aby se dal obnovit, když se okno zavře nebo spadne. Text čte přes **Windows UI Automation**, rozhraní pro přístupnost, které Windows k tomuto účelu poskytují.

U každé uložené položky si aplikace pamatuje i odkud pochází: název a cestu aplikace, titulek okna, popisek pole a u webových prohlížečů adresu stránky.

## Co aplikace nečte

- **Žádné zachytávání kláves.** Aplikace neinstaluje žádné háčky na klávesnici a nezaznamenává jednotlivé úhozy. Čte jen text, který pole samo zpřístupňuje.
- **Pole s hesly nikdy.** Pole, která Windows označují jako heslo, aplikace úplně vynechává.
- **Krátký text se neukládá.** Text kratší než nastavená délka se ignoruje.
- **Zablokované aplikace**, které si zvolíte, se nesledují vůbec. Automatické ukládání lze kdykoli pozastavit nebo vypnout.

## Kde jsou data uložená

Všechno je uložené na vašem počítači, ve vašem uživatelském profilu, ve složce `%LOCALAPPDATA%\CLIPBOARD`: databáze uložených položek, obrázky, místní zálohy, ikony webů, nastavení, diagnostické záznamy a hlášení o pádech.

Aplikace databázi nešifruje; chrání ji váš uživatelský účet ve Windows stejně jako ostatní vaše soubory. Knihovnu můžete zamknout přes **Windows Hello** a okna aplikace jsou skrytá před snímky obrazovky, nahráváním a sdílením obrazovky. To chrání to, co je vidět na obrazovce, ne soubory před jinými programy běžícími pod vaším účtem.

## Co opouští váš počítač

**Ikony webů.** Když se web objeví ve vaší historii poprvé, aplikace si vyžádá jeho ikonu od veřejné služby DuckDuckGo (`icons.duckduckgo.com`). Požadavek obsahuje jen **název domény**, například `example.com`, nikdy adresu stránky, text ani nic dalšího. Každá doména se žádá jen jednou, ikona pak zůstává na vašem počítači. Na tyto požadavky se vztahují [zásady soukromí DuckDuckGo](https://duckduckgo.com/privacy).

**Nic jiného.** Aplikace nikam neposílá historii schránky, uložený text, statistiky používání ani hlášení o pádech. Při pádu se hlášení zapíše jen na váš počítač; autorovi se dostane jen tehdy, když mu ho sami pošlete.

## Vaše kontrola

- Jednotlivé položky, celé složky i všechno najednou smažete přímo v aplikaci.
- Automatické ukládání můžete pozastavit nebo vypnout, změnit minimální délku a blokovat aplikace.
- **Odinstalace aplikace datovou složku nemaže.** Chcete-li odstranit všechno, smažte po odinstalaci složku `%LOCALAPPDATA%\CLIPBOARD`.

## Děti

Aplikace je obecný nástroj pro práci a není určena dětem.

## Změny

Pokud se tyto zásady změní, nové znění bude zveřejněno na této adrese s novým datem. Předchozí verze zůstávají ve veřejné historii tohoto webu.

## Kontakt

Dotazy k ochraně soukromí: [kafka.enterprise@gmail.com](mailto:kafka.enterprise@gmail.com)
