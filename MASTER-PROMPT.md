# Master prompt — procvičení sebevědomé komunikace (Seduo)

> **Použití:** zkopíruj celý blok v sekci „Copy-paste“ do nové Cursor session.  
> Před spuštěním doplň cesty a přílohy (@ soubory). Po implementaci reviduj texty v `TEXTY-K-REVIZI.md`.

---

## Copy-paste (celý prompt)

```
# Úkol: Doladit / znovu postavit procvičení sebevědomé komunikace (Seduo)

## Kontext produktu

- Složka projektu: /Users/maya.kopecka/Documents/Cursor/PACT/Projekty/test-sebevedoma-komunikace
- Zdroj obsahu: microkurzy Lenky Dědicové — transcripty v `microkurzy Dedicova/transcripty-microkurzy-dedicova.md`
- Publikace: statický web na GitHub Pages (Seduo branding: fialová #321C3D, zelená #30B99B, logo `Logo Seduo CZ bile.png`)
- Na začátku každé stránky: **Upozornění: Tento test byl vytvořen ve spolupráci s AI.**
- Zpětná vazba: pouze Typeform https://lmc4.typeform.com/to/emV4D50T (odkaz v patičce, ne embed povinný)

## Produktová definice (co stavíme)

**Hlavní produkt = procvičení role-play** (ne kvíz znalostí v menu).

1. **Úvodní stránka** (`index.html`) — dvě karty:
   - Vlastní odpovědi (`roleplay-free.html`) — doporučeno
   - Výběr z možností (`roleplay.html`)
2. **Kvíz znalostí** (`test-sebevedoma-komunikace.html`) — volitelný, mimo hlavní menu; pokud existuje, musí sdílet stejný obsahový model (microkurzy M1–M11) se scénáři.

**Cíl učení:** student po session umí v reálné situaci použít konkrétní techniku z daného microkurzu (ne jen „znát správnou odpověď“).

## Povinné vstupy (přečti před návrhem)

@PACT/Projekty/test-sebevedoma-komunikace/role-play-design-podklad.md
@PACT/Projekty/test-sebevedoma-komunikace/deep-research-report-best-practices for AI role-play.md
@PACT/Projekty/test-sebevedoma-komunikace/microkurzy Dedicova/transcripty-microkurzy-dedicova.md
@PACT/Projekty/test-sebevedoma-komunikace/scenarios.json (aktuální stav)
@PACT/Projekty/test-sebevedoma-komunikace/TEXTY-K-REVIZI.md (pokud existuje — texty k revizi)

## Metodické požadavky (nezpochybnitelné)

Vycházej z `role-play-design-podklad.md` a deep-research reportu:

1. **Expert judgment zakódovaný** — u každého scénáře/otázky pole `sourcePrinciple` = 1 věta citace principu z transkriptu daného microkurzu.
2. **Jedna mikrodovednost na scénář** (Lemov) — ne „obecná asertivita“, ale např. „opakovat ne bez výmluv (M2)“.
3. **Feedback: 1 pozitiv + 1 delta** — při chybě krátký princip + „Pusť si M{n} {název}“; žádný seznam 5 rad najednou.
4. **Správná volba** = splní techniku z M{n} (3 kroky asertivity / gramofon / otevřené dveře / … dle transkriptu).
5. **Distractory** = typické chyby z transkriptu: pasivita, agresivita/útok na osobu, výmluva, obhajoba místo otevřených dveří.
6. **Microlearning cap:** max 3 scénáře doporučené na jednu návštěvu; jeden scénář max 2 kroky (krátké).
7. **Transfer (Vrstva D):** na konci každé cesty (oba role-play módy) mini-krok — volitelné pole: „Koho tento týden oslovím a jakou větu použiju?“ + tlačítko Typeform.
8. **Jazyk:** jednotné tykání; gender-neutrální formulace studenta kde možné; konzistentní rod partnera v rámci scénáře.

## Architektura obsahu (kritické)

- **Jediný zdroj pravdy pro scénáře:** `scenarios.json`
- `roleplay.html` i `roleplay-free.html` **načítají scénáře přes fetch** — žádné embedded kopie `SCENARIOS_DATA` v HTML.
- Texty UI a scénářů udržuj v `TEXTY-K-REVIZI.md` (ID řádky neměnit) pro budoucí revizi.
- Po změně obsahu aktualizuj `TEXTY-K-REVIZI.md` ze `scenarios.json`.

## Pokrytí microkurzů

Každý microkurz M1–M11 musí mít **alespoň 1 scénář** v `scenarios.json` (dnes chybí M5, M8, M11 — doplň).

Struktura scénáře v JSON:

```json
{
  "id": "slug",
  "microkurz": 2,
  "title": "...",
  "context": "...",
  "goal": "...",
  "sourcePrinciple": "Citace principu z transkriptu M2.",
  "steps": [{
    "partnerLine": "...",
    "options": [
      { "type": "assertive", "label": "Asertivní reakce", "text": "...", "feedback": "..." },
      { "type": "passive", "label": "Pasivní reakce", "text": "...", "feedback": "..." },
      { "type": "aggressive", "label": "Agresivní reakce", "text": "...", "feedback": "..." }
    ]
  }]
}
```

## Vlastní odpovědi (`roleplay-free.html`)

Nahraď čistou heuristiku klíčových slov **rubrikou 0–2** na dimenze (z transkriptů):

| Dimense | 0 | 1 | 2 |
|---------|---|---|---|
| Popis situace (co se stalo) | chybí | částečně | jasně |
| Já-sdělení (co to se mnou dělá) | chybí | částečně | jasně |
| Žádost / hranice / technika M{n} | chybí | slabě | splněno |

- Součet ≥ 4 → asertivní; pasivní/agresivní podle signálů (útok, výmluva, mlčení) s vysvětlením.
- U každého scénáře uveď v JSON `exampleAssertive` pro inspiraci po vyhodnocení.
- Feedback vždy odkazuje na `microkurz` scénáře.

## Úvodní texty (Seduo)

- H1: Procvičení sebevědomé komunikace
- Popis: Procvičte si asertivní reakce v reálných situacích. Vyberte si způsob: buď napíšete vlastní odpověď a dostanete vyhodnocení, nebo zvolíte z nabízených reakcí.
- Badge na kartě výběru: počet scénářů = skutečný počet v JSON.

## Volitelný kvíz (pokud zůstane v repu)

- Banka 25 otázek, 2–3 na M1–M11; session = 11 (1× každý MK) + 4 náhodné = 15.
- Pole: `microkurz`, `whyCorrect`, `whyWrongHint`, `sourcePrinciple`.
- Card „Co si pustit znovu“ po skóre (top 3 MK podle chyb).
- **Není** v `index.html` menu.

## Co NEIMPLEMENTOVAT v této iteraci

- Google Analytics (připrav jen hook / placeholder soubor, ne aktivní měření)
- Voice / avatar role-play
- Backend, účty, spaced repetition napříč návštěvami
- Duplicitní embed scénářů v HTML

## Postup práce

1. **Audit** — porovnej `scenarios.json`, oba roleplay HTML a `TEXTY-K-REVIZI.md`; vypiš mezery (MK, duplicity, texty).
2. **Návrh** — tabulka: které scénáře doplnit/změnit, 1 věta `sourcePrinciple` na scénář; počkej na schválení POUZE pokud měníš pedagogický model více než 30 % obsahu.
3. **Implementace** — JSON → fetch v HTML → rubrika free mode → transfer krok → sync `TEXTY-K-REVIZI.md`.
4. **Kontrola** — checklist:
   - [ ] 11 microkurzů má scénář
   - [ ] žádný embedded SCENARIOS_DATA v HTML
   - [ ] chybná volba → feedback + M{n}
   - [ ] Seduo CSS + AI banner na všech stránkách
   - [ ] Typeform odkaz funguje

## Výstupy

- Aktualizované: `scenarios.json`, `roleplay.html`, `roleplay-free.html`, `index.html`, `site.css`, `TEXTY-K-REVIZI.md`
- Krátký `CHANGELOG.md` — co se změnilo metodicky oproti předchozí verzi
- Necommituj: `microkurzy Dedicova/*.mp4`, interní .docx, secrets

Začni auditem a stručným návrhem doplnění M5, M8, M11 a sjednocení zdroje scénářů.
```

---

## Rychlá varianta (jen role-play, bez kvízu)

Pokud nechcete vůbec řešit kvíz, přidej na konec promptu:

```
Ignoruj test-sebevedoma-komunikace.html — neupravuj, neodkazuj z menu.
```

---

## Checklist před odesláním promptu

- [ ] Přiloženy @ soubory (podklad, deep-research, transcripty)
- [ ] `TEXTY-K-REVIZI.md` existuje nebo agent ho vytvoří po první implementaci
- [ ] Rozhodnuto: kvíz ano/ne (výchozí = ne v menu)
- [ ] Typeform URL je aktuální

---

## Související soubory v projektu

| Soubor | Účel |
|--------|------|
| `PROMPT-ZDROJ.md` | Historie původních promptů |
| `TEXTY-K-REVIZI.md` | Revize textů (ID pro sync) |
| `role-play-design-podklad.md` | Metodický framework |
| `deep-research-report-best-practices for AI role-play.md` | Best practices |
