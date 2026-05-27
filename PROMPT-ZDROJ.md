# Prompt(y), ze kterých vzniklo procvičení

> Rekonstrukce z konverzace [Doladění testu sebevědomé komunikace](f21fafec-45b5-4a0f-a40d-99e61191c654) (19. 5. 2026).  
> Plán implementace: `.cursor/plans/doladění_testu_sebevědomé_komunikace_5a1c04f1.plan.md`

---

## 1. Váš původní prompt (start)

```
Chci doladit testování modelových situací na sebevědomou komunikaci, které je připraveno ve složce
/Users/maya.kopecka/Documents/Cursor/PACT/Projekty/test-sebevedoma-komunikace.

Ve složce '.../microkurzy Dedicova' jsou transcripty k microkurzům ze kterých test vychází.

Než začneš, projdi si poznatky k role-play v dokumentech:
- deep-research-report-best-practices for AI role-play.md
- role-play-design-podklad.md
a zvaž, co se hodí pro náš případ.

Pak si projdi, jak by se dali transcripty využít k vylepšení testu:
- přidat další situace,
- zajistit, že se správná odpověď vždy drží v rámci daného microkurzu,
- pokud student odpoví špatně, doporučit mu, ve kterém microkurzu se dozví víc.

Pokud je potřeba pro vylepšení testu ještě něco dalšího, řekni si o to.

Nejprve navrhni, jak test vylepšit a co bys případně přidala za otázky.
```

**Implicitní vstupy (přiložené @ soubory):** oba design podklady + existující HTML/JSON ve složce projektu.

---

## 2. Upřesnění rozsahu (odpovědi na doplňující otázky)

Před plánem jste vybrala:

| Otázka | Vaše volba |
|--------|------------|
| Rozsah úprav | **Test + scenarios.json + výzvy k akci** (propojit i závěrečné kroky s microkurzy) |
| Stávající 12 otázek | **Větší banka ~25 otázek**, z níž se náhodně vybírá 12–15 na session |

---

## 3. Implementační plán (= syntetický „master prompt“ pro AI)

Toto je plán, který agent následně implementoval (po schválení):

### Cíl a rámec

Doladit test tak, aby:

1. **pokrýval všech 11 microkurzů Dědicové** (dnes jen 4 ze 11),
2. **každá správná odpověď byla zakotvená v konkrétním slovníku/principu microkurzu** (encode expert judgment — princip 2.2 z `role-play-design-podklad.md`),
3. **při chybě student dostal doporučení, který microkurz si pustit** (hybridní feedback z deep-research: immediate cue + specifická behaviorální zpětná vazba),
4. **každá session byla krátká** (microlearning, princip 2.6) — z banky ~25 otázek se vybere 12–15.

### Vrstva A — Otázky (`test-sebevedoma-komunikace.html`)

- Banka **25 otázek**, 2–3 na microkurz M1–M11.
- Struktura otázky: `microkurz`, `whyCorrect`, `whyWrongHint`, `skill`.
- Feedback při chybě: **jeden princip + odkaz „Pusť si M{n} …“** (Lemov: jeden pozitiv + jeden delta).
- Výběr na session: **1 otázka z každého microkurzu (11) + 4 náhodné = 15**.

Rozpis nových otázek podle microkurzů (M2–M4, M8–M11 nově; M1, M5–M7 audit/ponechat) — viz plán v `.cursor/plans/...`.

### Vrstva B — Po skóre

- Card **„Co si pustit znovu“**: top 3 microkurzy podle počtu chyb + focus věta.

### Vrstva C — Role-play (`scenarios.json`)

- +5 scénářů: `gramofon-prescas` (M2), `otevrene-dvere-vycitka` (M3), `pauza-pod-tlakem` (M4), `pasivni-agresivita-kolegyne` (M9), `tvrde-emoce-druheho` (M10).
- Každý scénář: jedna izolovaná mikrodovednost + `microkurz` + feedback s odkazem na microkurz.

### Vrstva D — Výzvy k akci

- `linkedMicrokurzy` u výzev + zobrazení v summary (transfer trigger).

### Vědomě vynechano v 1. iteraci

- Voice/avatar role-play
- Měření transferu v reálné práci (Tier 5–7)
- Spaced repetition napříč návštěvami (backend/localStorage)
- Volitelný návrh: pole *„Kdy a s kým to plánujete vyzkoušet?“* ve summary — **neimplementováno**

### Referenční dokumenty (povinné čtení pro agenta)

- `role-play-design-podklad.md` — 4 vrstvy, 6 principů, Lemov drill
- `deep-research-report-best-practices for AI role-play.md` — scaffolding, hybrid feedback, rubrika
- `microkurzy Dedicova/transcripty-microkurzy-dedicova.md` — slovník a principy M1–M11

---

## 4. Prompt na implementaci

```
Implement the plan as specified, it is attached for your reference.
Do NOT edit the plan file itself.
To-do's from the plan have already been created. Do not create them again.
Mark them as in_progress as you work, starting with the first one.
Don't stop until you have completed all the to-dos.
```

---

## 5. Navazující prompty (po první verzi)

### Publikace + měření

```
Test budu chtít publikovat na githubu, aby šel sdílet se studenty.
Chci jej napojit na Google Analytics, abych viděla, kolik lidí na něj přišlo a kam studenti dojdou,
pokud test nedokončí, a přidat na konec krátký feedback, kterým zjistím, jak se jim procvičení líbilo
a zda něco takového chtějí na Seduo.
Na začátku testu by také mělo být upozornění, že: Tento test byl vytvořen ve spolupráci s AI.
```

### Publikace bez GA (Typeform)

```
Chci připravit pro nasazení do GitHubu zatím verzi bez google analytics.
Co se týče dotazníku na konci, použiju jen typeform:
https://lmc4.typeform.com/to/emV4D50T
Připrav prosím vše pro publikaci.
```

### Seduo branding + zúžení produktu

```
V testu chybí Seduo branding a Seduo barevnost, tak jak to bylo v původní verzi.
Je tam zbytečně Test ověření znalostí, ten prosím celý odstranit.

Úvodní text má být:
Procvičení sebevědomé komunikace
Procvičte si asertivní reakce v reálných situacích. Vyberte si způsob: buď napíšete vlastní odpověď
a dostanete vyhodnocení, nebo zvolíte z nabízených reakcí.
```

*(Kvíz znalostí zůstal v repu jako `test-sebevedoma-komunikace.html`, ale byl odstraněn z menu.)*

---

## 6. Co prompt **neříkal** explicitně (důsledky pro metodologii)

| Oblast | Co se stalo | Riziko / mezera |
|--------|-------------|------------------|
| **Jeden zdroj scénářů** | `scenarios.json` + duplikát v `roleplay.html` + jiný subset v `roleplay-free.html` | Rozbité scénáře při úpravě jen jednoho souboru |
| **Vlastní odpovědi** | Klasifikace heuristikou (klíčová slova), ne LLM | Falešně pozitivní/negativní vyhodnocení |
| **Kvíz vs. role-play** | Kvíz pokrývá M1–M11; role-play jen 8 situací | Student může projít procvičení bez M5, M8, M11 v praxi |
| **Transfer** | Výzvy k akci jen u kvízu; po odstranění z menu chybí | Slabší „co udělám tento týden“ u hlavního produktu |
| **Validace obsahu** | AI generovala otázky/scénáře z transkriptů bez expertní revize | Metodická přesnost závisí na vaší revizi (`TEXTY-K-REVIZI.md`) |
| **Rod / tykání** | Mix v replikách partnera | Nekonzistence pro studenty |
| **Microkurz u scénáře M4** | Scénář „pauza“ tagován M4, plán zmiňoval M4+M10 | Hranice techniky vs. „zůstat u sebe“ může být matoucí |

---

## 7. Návrhy metodologického vylepšení promptu (pro příští iteraci)

Pokud budete prompt přepisovat, doporučuji doplnit:

1. **Jedna pravda pro obsah:** „Všechny scénáře pouze v `scenarios.json`; HTML jen načítá JSON (fetch), žádné embedded kopie.“
2. **Povinná expertní kontrola:** „Každá otázka/scénář musí mít `sourceMicrokurz` + citaci principu z transkriptu (1 věta).“
3. **Kritéria správné odpovědi:** „Správná volba = splní 3 kroky asertivity / konkrétní techniku z M{n}; špatné distractory = typické chyby z transkriptu (výmluva, útok, pasivita).“
4. **Produktová definice:** Upřesnit, zda je hlavní produkt **jen role-play** nebo **kvíz + role-play**; pokud jen role-play, banka otázek není nutná.
5. **Vlastní odpovědi:** Buď „pravidla + 3 příklady pro každý typ“, nebo „vyhodnocení přes rubriku s bodováním 0–2 na dimenze (popis situace, já-sdělení, žádost).“
6. **Transfer na konci každé cesty:** Jedna povinná mini-výzva: *„Koho tento týden oslovím a jakou větu použiju?“* (volitelné pole, ne Typeform).
7. **Délka session:** Explicitní cap (např. max 10 min, max 3 scénáře za návštěvu).
8. **A11y a jazyk:** Jednotné tykání, gender-neutrální formulace kde to jde.

---

## 8. Ukázka struktury otázky z plánu (referenční prompt pro generování)

```javascript
{
  id: 13,
  microkurz: 2,
  microkurzTitle: "Gramofon",
  skill: "Opakované ne pod tlakem bez výmluv",
  question: "Kolega vás potřetí tlačí: 'No tak fajn, příště ti to oplatím, jen dneska zůstaň.' Která reakce nejlíp drží asertivní hranici?",
  options: [
    "Vím, že je to pro tebe důležité, ale dneska opravdu zůstat nemůžu.",
    "Tak fajn, ale jen na hodinku, jo?",
    "Nemůžu, hlídám děti a slíbil jsem ženě, že přijdu včas, opravdu to nepůjde."
  ],
  correctIndex: 0,
  whyCorrect: "Technika poškrábané gramofonové desky: klidně opakuju stanovisko, nepřesvědčuju, neomlouvám se.",
  whyWrongHint: "Výmluvy ('hlídám děti') otevírají prostor pro vyjednávání ('tak si zavolej babičku'). Krátké 'dneska to nejde' nemá kam pokračovat. Pusť si M2 Gramofon."
}
```
