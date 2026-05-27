# Texty procvičení – k revizi

> **Jak pracovat s tímto souborem**
> 1. Upravte texty přímo pod nadpisy (ponechte `ID:` řádky beze změny – slouží k automatické aktualizaci webu).
> 2. Uložte soubor.
> 3. Napište mi: *„Aplikuj texty z TEXTY-K-REVIZI.md“* – přenesu změny do HTML a `scenarios.json`.
>
> **Poznámka:** Scénáře v sekci 5 jsou zdroj pravdy pro **Výběr z možností** (`roleplay.html` + `scenarios.json`).  
> **Vlastní odpovědi** (`roleplay-free.html`) má zatím jen 6 scénářů vložených v HTML – po revizi je sjednotíme se `scenarios.json` (8 scénářů).

---

## 1. Společné texty (všechny stránky)

| ID | Text |
|----|------|
| `common.ai_notice` | **Upozornění:** Tento test byl vytvořen ve spolupráci s AI. |
| `common.logo_alt` | Seduo CZ |
| `common.back_home` | ← Zpět na hlavní stránku |
| `common.feedback_link` | Poslat zpětnou vazbu |
| `common.feedback_url` | https://lmc4.typeform.com/to/emV4D50T |
| `common.partner_label` | Kolega |
| `common.goal_label` | Cíl: |
| `common.btn_start` | Začít |
| `common.btn_back_select` | Zpět na výběr |
| `common.btn_next_step` | Další krok |
| `common.btn_end_scenario` | Konec scénáře |
| `common.btn_pick_other` | Vybrat jiný scénář |
| `common.your_answer_label` | Vaše odpověď |
| `common.how_react` | Jak zareagujete? |
| `common.click_scenario` | Klikněte na scénář, který chcete procvičit. |
| `common.replay_hint` | Pusť si znovu: |

### Typy reakcí (štítky možností)

| ID | Text |
|----|------|
| `type.assertive` | Asertivní reakce |
| `type.passive` | Pasivní reakce |
| `type.aggressive` | Agresivní reakce |
| `type.closure` | Uzavření |
| `type.excuse` | Reakce s výmluvou |
| `type.defensive` | Obranná reakce |

### Vlastní odpovědi – vyhodnocení

| ID | Text |
|----|------|
| `free.evaluate_btn` | Vyhodnotit |
| `free.reply_label` | Vaše reakce (napište, co byste řekli): |
| `free.reply_placeholder` | Napište svou odpověď… |
| `free.eval_prefix` | Vyhodnocení: |
| `free.eval_assertive` | Asertivní |
| `free.eval_passive` | Pasivní |
| `free.eval_aggressive` | Agresivní |
| `free.eval_unclear` | Nejasná / smíšená |
| `free.unclear_feedback` | Vaše reakce nebyla jednoznačně zařaditelná. Zkuste příště: popsat situaci (co se stalo), říct, co to s vámi dělá, a jasně požádat o změnu – nebo naopak v klidu odmítnout bez výmluv. |
| `free.example_prefix` | **Pro inspiraci – příklad asertivní reakce:** |

---

## 2. Úvodní stránka (`index.html`)

| ID | Text |
|----|------|
| `index.title_page` | Procvičení sebevědomé komunikace – Seduo |
| `index.h1` | Procvičení sebevědomé komunikace |
| `index.intro` | Procvičte si asertivní reakce v reálných situacích. Vyberte si způsob: buď napíšete vlastní odpověď a dostanete vyhodnocení, nebo zvolíte z nabízených reakcí. |
| `index.card_free_title` | Vlastní odpovědi |
| `index.card_free_desc` | Napište vlastní reakci v dané situaci a dostanete vyhodnocení (asertivní / pasivní / agresivní) a zpětnou vazbu. |
| `index.badge_recommended` | Doporučeno |
| `index.badge_own_text` | Vlastní text |
| `index.card_choice_title` | Výběr z možností |
| `index.card_choice_desc` | Vyberte jednu ze tří připravených reakcí a přečtěte si k ní zpětnou vazbu. Ideální pro rychlé procvičení. |
| `index.badge_scenarios_count` | 8 scénářů |
| `index.footer_feedback` | Poslat zpětnou vazbu k procvičení |

---

## 3. Výběr z možností (`roleplay.html`)

| ID | Text |
|----|------|
| `choice.title_page` | Výběr z možností – Sebevědomá komunikace |
| `choice.list_h2` | Sebevědomá komunikace – Vyberte scénář |
| `choice.list_p1` | Přečtěte si repliku kolegy a vyberte jednu ze tří reakcí. Ke každé uvidíte zpětnou vazbu. |

---

## 4. Vlastní odpovědi (`roleplay-free.html`)

| ID | Text |
|----|------|
| `free.title_page` | Vlastní odpovědi – Sebevědomá komunikace |
| `free.list_h2` | Sebevědomá komunikace – Vyberte scénář |
| `free.list_p1` | Napište vlastní reakci v dané situaci. Po odeslání dostanete vyhodnocení (asertivní / pasivní / agresivní) a zpětnou vazbu. |

---

## 5. Microkurzy (doporučení při chybě)

| ID | Název | Focus (krátká věta) |
|----|-------|---------------------|
| `mk.1.title` | M1 Asertivita | Tři kroky: popis situace → co to s vámi dělá → návrh řešení. |
| `mk.2.title` | M2 Gramofon | Klidně opakovat stanovisko bez výmluv — ty otvírají prostor k vyjednávání. |
| `mk.3.title` | M3 Otevřené dveře | Souhlasit s částí sdělení, ale držet vlastní rozhodnutí. |
| `mk.4.title` | M4 Emoce | Rozpoznat spouštěč (red flag), říct si o pauzu, dýchat. |
| `mk.5.title` | M5 Žádost | Konkrétní žádost, ne tichá naděje. Žádost dává prostor i pro ne. |
| `mk.6.title` | M6 Odmítnutí | Krátké jasné ne bez omluvy za rozhodnutí. |
| `mk.7.title` | M7 Feedback | Popis chování + já-sdělení + návrh, ne nálepka osoby. |
| `mk.8.title` | M8 Mindset | Asertivita stojí na rovnosti a asertivních právech. |
| `mk.9.title` | M9 Výčitky | Pojmenovat pasivní agresivitu klidně, nepřijímat vinu. |
| `mk.10.title` | M10 Zůstat u sebe | Empatie k emoci druhého + držení vlastního rozhodnutí. |
| `mk.11.title` | M11 Techniky | Asertivita je střed mezi pasivitou a agresí. |

---

## 6. Scénáře (8×) – `scenarios.json` + výběr z možností

U každého scénáře upravte: název, situaci, cíl, repliky kolegy, texty možností a zpětnou vazbu.

---

### Scénář 1: Úkol na poslední chvíli

**ID scénáře:** `ukol-posledni-chvile`  
**Microkurz:** M1 Asertivita

| ID | Text |
|----|------|
| `s1.title` | Úkol na poslední chvíli |
| `s1.context` | Kolega vám právě poslal e-mail s úkolem, který potřebuje mít zítra. Jste v časovém presu a podobné požadavky už několikrát přišly pozdě. |
| `s1.goal` | Asertivně požádat o dřívější zadávání úkolů, aniž byste druhého obviňovali. |

**Krok 1**

| ID | Text |
|----|------|
| `s1.s0.partner` | Hele, potřebuju to mít hotový do zítřka, můžeš na tom zapracovat? |
| `s1.s0.opt_a.text` | Když mi to přijde tak pozdě, nestihnu to kvalitně do zítřka. Můžeš mi příště posílat úkoly alespoň o den dřív? |
| `s1.s0.opt_a.feedback` | Výborně. Popisujete dopad na sebe, žádáte konkrétní změnu a nespadáte do kritiky ani útoku. Druhá strana ví, co má příště udělat. |
| `s1.s0.opt_b.text` | No… dobře, zkusím to. |
| `s1.s0.opt_b.feedback` | Tím jste nesdělili svůj limit. Kolega neví, že vám to vadí, a situace se může opakovat. Zkuste říct, co potřebujete a co je pro vás reálné. Pusť si M1 Asertivita — tři kroky popis → dopad → návrh. |
| `s1.s0.opt_c.text` | Tohle mi práci dost zkomplikuje. Takto to opravdu nejde. |
| `s1.s0.opt_c.feedback` | Kritizujete situaci bez konkrétní žádosti. Druhá strana neví, co má změnit. Zkuste popsat dopad na sebe a jasně požádat o změnu. Pusť si M1 Asertivita. |

---

### Scénář 2: Odmítnutí pozvánky

**ID scénáře:** `odmitnuti-pozvanky`  
**Microkurz:** M6 Odmítnutí

| ID | Text |
|----|------|
| `s2.title` | Odmítnutí pozvánky |
| `s2.context` | Kolega vás zve na firemní večírek v pátek večer. Jste unavení a víte, že byste si měli odpočinout. Nechce se vám jít, ale bojíte se, že to bude vypadat nevděčně. |
| `s2.goal` | Asertivně odmítnout s respektem k sobě i k pozvání. |

**Krok 1**

| ID | Text |
|----|------|
| `s2.s0.partner` | Přijdeš v pátek na ten večírek? Bude to super! |
| `s2.s0.opt_a.text` | Díky, že jsi na mě myslel, ale tentokrát nemůžu – potřebuju si odpočinout. |
| `s2.s0.opt_a.feedback` | Dobře. Oceňujete pozvání, říkáte jasné ne a krátce vysvětlujete bez zbytečného omlouvání. Hranice jsou jasné a vztah zůstává v pohodě. |
| `s2.s0.opt_b.text` | Jé, já bych strašně rád, ale víš, bolí mě hlava a musím ještě volat babičce… |
| `s2.s0.opt_b.feedback` | Vymýšlíte výmluvy místo upřímného ne. Když to vyjde najevo, může to poškodit důvěru. Zkuste říct jednoduše, že teď ne. Pusť si M6 Odmítnutí — krátké jasné ne bez omluv. |
| `s2.s0.opt_c.text` | Na takové akce nemám čas ani náladu. |
| `s2.s0.opt_c.feedback` | Zní to odmítavě a může to působit útočně. Druhá strana neví, že to nemyslíte zle. Zkuste poděkovat za pozvání a říct krátce, proč tentokrát ne. Pusť si M6 Odmítnutí. |

---

### Scénář 3: Nedodržený termín

**ID scénáře:** `nedodrzeny-termin`  
**Microkurz:** M7 Feedback

| ID | Text |
|----|------|
| `s3.title` | Nedodržený termín |
| `s3.context` | Kolega měl odevzdat podklady včera. Kvůli tomu jste nemohli dokončit svou část včas. Vidíte ho u kafe a chcete to s ním probrat. |
| `s3.goal` | Popsat dopad na vás a jasně říct, co potřebujete příště – bez útoků na osobu. |

**Krok 1**

| ID | Text |
|----|------|
| `s3.s0.partner` | Jo, promiň, včera jsem to nestihl. Bude to do zítra, to stačí, ne? |
| `s3.s0.opt_a.text` | Když se nedodrží termín, mám potíže s navazující prací. Potřebuju, abychom příště termíny opravdu drželi, nebo abychom je včas upravili. |
| `s3.s0.opt_a.feedback` | Výborně. Popisujete dopad na svou práci a jasně říkáte, co potřebujete. Kritika směřuje na situaci a na chování, ne na člověka. |
| `s3.s0.opt_b.text` | No… doufám, že příště to vyjde. |
| `s3.s0.opt_b.feedback` | Nesdělujete, jak vás to ovlivnilo ani co potřebujete. Druhý nemá důvod cokoli měnit. Zkuste popsat dopad a říct konkrétní očekávání. Pusť si M7 Feedback. |
| `s3.s0.opt_c.text` | Ty jsi zase všechno pokazil. Kvůli tobě jsem v průšvihu. |
| `s3.s0.opt_c.feedback` | Útočíte na osobu („ty jsi pokazil"). Druhá strana se bude bránit místo spolupráce. Zkuste popsat situaci a dopad na vás, bez obviňování. Pusť si M7 Feedback. |

**Krok 2**

| ID | Text |
|----|------|
| `s3.s1.partner` | Máš pravdu, příště to pohlídám. Díky, že jsi to řekl přímo. |
| `s3.s1.opt_a.text` | Díky za pochopení. |
| `s3.s1.opt_a.feedback` | Scénář ukončen. Hezky jste situaci uzavřeli a druhá strana ví, co od ní očekáváte. |

---

### Scénář 4: Opakovaný tlak na přesčas

**ID scénáře:** `gramofon-prescas`  
**Microkurz:** M2 Gramofon

| ID | Text |
|----|------|
| `s4.title` | Opakovaný tlak na přesčas |
| `s4.context` | Kolega vás po druhé tlačí, abyste s ním zůstali přes čas a pomohli mu dodělat prezentaci. Vy jste už řekli, že nemůžete, ale on opakovaně zkouší. |
| `s4.goal` | Klidně a vytrvale držet ne, bez výmluv (technika poškrábané gramofonové desky). |

**Krok 1**

| ID | Text |
|----|------|
| `s4.s0.partner` | Hele, vážně bych to ocenil, jen na hodinku. Pomůžeš mi? |
| `s4.s0.opt_a.text` | Vím, že je to pro tebe důležité, ale dneska zůstat opravdu nemůžu. |
| `s4.s0.opt_a.feedback` | Přesně technika gramofonu: krátké, klidné stanovisko bez výmluv. Druhý nemá za co zatáhnout. |
| `s4.s0.opt_b.text` | Hmm, no, tak možná na chvíli, jestli to nepůjde jinak… |
| `s4.s0.opt_b.feedback` | Ustoupil/a jste. Zkuste klidně zopakovat svoje stanovisko, jako „jehla v gramofonu". Pusť si M2 Gramofon. |
| `s4.s0.opt_c.text` | Nemůžu, hlídám děti a slíbil jsem ženě, že přijdu včas, a ještě mám doktora. |
| `s4.s0.opt_c.feedback` | Výmluva otevírá prostor pro vyjednávání („tak si zavolej babičku"). Krátké „dnes to nejde" nemá kam pokračovat. Pusť si M2 Gramofon. |

**Krok 2**

| ID | Text |
|----|------|
| `s4.s1.partner` | No tak fajn, příště ti to oplatím, jo? Jen dneska, prosím. |
| `s4.s1.opt_a.text` | Dneska to opravdu nejde. |
| `s4.s1.opt_a.feedback` | Stejné stanovisko, klidně, znovu. To je síla gramofonu — nemusíte vysvětlovat ani omlouvat. |
| `s4.s1.opt_b.text` | No tak dobře, jen pár minut. |
| `s4.s1.opt_b.feedback` | Pod opakovaným tlakem jste ustoupil/a. Síla gramofonu je v tom, že na třetí pokus říkáte to stejné. Pusť si M2 Gramofon. |

---

### Scénář 5: „Dřív jsi byla ochotnější"

**ID scénáře:** `otevrene-dvere-vycitka`  
**Microkurz:** M3 Otevřené dveře

| ID | Text |
|----|------|
| `s5.title` | „Dřív jsi byla ochotnější" |
| `s5.context` | Známá vás žádá o pomoc s velkým stěhováním v sobotu. Když odmítnete, řekne dotčeně: „Dřív jsi byla ochotnější. Vůbec tě nepoznávám." |
| `s5.goal` | Použít techniku otevřených dveří — souhlasit s částí sdělení, ale zůstat u svého. |

**Krok 1**

| ID | Text |
|----|------|
| `s5.s0.partner` | Dřív jsi byla ochotnější. Vůbec tě nepoznávám. |
| `s5.s0.opt_a.text` | Možná máš pravdu, dřív jsem pomáhala víc. Dneska to ale opravdu nevezmu. |
| `s5.s0.opt_a.feedback` | Otevřené dveře: souhlasíte s částí, ale rozhodnutí zůstává vaše. Nebojujete ani neustupujete. |
| `s5.s0.opt_b.text` | Není to pravda, já se snažím pořád stejně, jen teď mám hodně práce. |
| `s5.s0.opt_b.feedback` | Obhajujete se a tím přijímáte pravidla hry druhé strany. Otevřete dveře — uznejte část a držte rozhodnutí. Pusť si M3 Otevřené dveře. |
| `s5.s0.opt_c.text` | Když ti to nevyhovuje, můžeš si poradit sama. |
| `s5.s0.opt_c.feedback` | Protiútok zavře dveře pro dohodu. Otevřené dveře = klidné uznání + držení rozhodnutí. Pusť si M3 Otevřené dveře. |

---

### Scénář 6: Pauza pod emočním tlakem

**ID scénáře:** `pauza-pod-tlakem`  
**Microkurz:** M4 Emoce

| ID | Text |
|----|------|
| `s6.title` | Pauza pod emočním tlakem |
| `s6.context` | Šéf vám během porady řekne před ostatními: „Tohle jsi zase zvoral, jako vždycky." Cítíte, jak se vám zvedá hladina a chcete reagovat hned. |
| `s6.goal` | Rozeznat spouštěč, vyžádat si pauzu, vrátit se klidný/á. |

**Krok 1**

| ID | Text |
|----|------|
| `s6.s0.partner` | Tohle jsi zase zvoral, jako vždycky. |
| `s6.s0.opt_a.text` | Slyším, co říkáš. Potřebuju chvíli na rozmyšlenou, ozvu se ti během hodiny. |
| `s6.s0.opt_a.feedback` | Pauza je vědomá volba. Necháváte emoci usadit, ne útěk. To je mistrovský tah, ne slabost. |
| `s6.s0.opt_b.text` | (Mlčíte, polknete a přejdete to bez komentáře.) |
| `s6.s0.opt_b.feedback` | Mlčení nechává hranici nepojmenovanou. Pauza není totéž co potlačení. Pusť si M4 Emoce. |
| `s6.s0.opt_c.text` | Tak si to udělej sám, jestli to umíš líp! |
| `s6.s0.opt_c.feedback` | Vybouchnutí stojí na spouštěči, ne na vašem rozhodnutí. Dejte si pauzu, dech, a vraťte se. Pusť si M4 Emoce. |

---

### Scénář 7: „Někdo má víc času"

**ID scénáře:** `pasivni-agresivita-kolegyne`  
**Microkurz:** M9 Výčitky

| ID | Text |
|----|------|
| `s7.title` | „Někdo má víc času" |
| `s7.context` | V pondělí jste odmítli vzít víkendovou službu navíc. V úterý kolegyně u kávy řekne sarkasticky: „No jasně, někdo má pořád víc času než ostatní." |
| `s7.goal` | Pojmenovat pasivní agresivitu klidně a otevřít přímý dialog. |

**Krok 1**

| ID | Text |
|----|------|
| `s7.s0.partner` | No jasně, někdo má pořád víc času než ostatní. |
| `s7.s0.opt_a.text` | Zní to, jako by tě to mrzelo. Je něco, co bys mi chtěla říct napřímo? |
| `s7.s0.opt_a.feedback` | Pojmenováním vytahujete věc na povrch. Pasivní agresivita ztrácí sílu, dialog se otevírá. |
| `s7.s0.opt_b.text` | Promiň, no… asi to vzít budu muset. |
| `s7.s0.opt_b.feedback` | Omluva za rozhodnutí přijímá vinu, kterou si druhý chtěl, abyste cítila. Pojmenujte, co se děje. Pusť si M9 Výčitky. |
| `s7.s0.opt_c.text` | Tobě je teda nějak hodně do mě, viď? |
| `s7.s0.opt_c.feedback` | Vracíte ironii a roztáčíte tu hru dál. Pojmenujte klidně, co se děje. Pusť si M9 Výčitky. |

---

### Scénář 8: „Fakt mě zklamáváš"

**ID scénáře:** `tvrde-emoce-druheho`  
**Microkurz:** M10 Zůstat u sebe

| ID | Text |
|----|------|
| `s8.title` | „Fakt mě zklamáváš" |
| `s8.context` | Odmítli jste kolegovi pomoct s jeho úkolem. Reaguje silně a osobně: „Fakt mě tím zklamáváš. To bych do tebe neřekl." |
| `s8.goal` | Přijmout emoci druhého, ale neměnit vlastní rozhodnutí (mistrovství asertivity). |

**Krok 1**

| ID | Text |
|----|------|
| `s8.s0.partner` | Fakt mě tím zklamáváš. To bych do tebe neřekl. |
| `s8.s0.opt_a.text` | Rozumím, že tě to mrzí. I přesto to teď nemůžu udělat. |
| `s8.s0.opt_a.feedback` | Mistrovství asertivity: empatie + držení rozhodnutí. Slyšíte druhého, ale vaše hranice zůstává. |
| `s8.s0.opt_b.text` | No tak dobře, něco vymyslím, ať tě v tom nenechávám. |
| `s8.s0.opt_b.feedback` | Změnil/a jste rozhodnutí jen proto, že druhý je zklamaný. Váš kompas nejsou jeho emoce. Pusť si M10 Zůstat u sebe. |
| `s8.s0.opt_c.text` | Ty se zase taháš za růžky, vždycky stejný! |
| `s8.s0.opt_c.feedback` | Útok na osobu zavírá dialog a navíc vás vtáhne do emoční pasti. Zůstaňte u sebe — přiznejte emoci, držte rozhodnutí. Pusť si M10 Zůstat u sebe. |

---

## 7. Scénáře navíc ve „Vlastní odpovědi" (zatím jen 6 – ke sjednocení)

Tyto scénáře jsou v `roleplay-free.html` a **nejsou** v `scenarios.json`. Po revizi je doporučuji buď doplnit do sekce 6, nebo smazat tuto sekci.

### Scénář A: Opakované pozdní příchody

**ID:** `pozde-prichody`

| ID | Text |
|----|------|
| `sa.title` | Opakované pozdní příchody |
| `sa.context` | Kolega dorazil na vaši společnou pracovní schůzku o 15 minut později. Není to poprvé a vám to narušuje další program dne. |
| `sa.goal` | Asertivně reagovat na pozdní příchod a vyjádřit potřebu začínat příště včas. |
| `sa.s0.partner` | Promiň, že jdu pozdě, měl jsem zpoždění. Pojďme začít. |
| `sa.s0.opt_a.text` | Když schůzka začne později, dostávám se pak v celém dni do skluzu. Potřebuju, abychom příště začínali přesně včas. |
| `sa.s0.opt_a.feedback` | Správně. Popisujete objektivní dopad na vaši práci a vyjadřujete jasnou potřebu do budoucna, aniž byste na kolegu útočili. |
| `sa.s0.opt_b.text` | To je v pohodě, hlavně že jsi tady. Pojďme rychle začít, ať to stihneme. |
| `sa.s0.opt_b.feedback` | Tímto přístupem nesdělujete svůj limit. Kolega získá dojem, že pozdní příchody nevadí, a situace se bude pravděpodobně opakovat. |
| `sa.s0.opt_c.text` | Takhle se nedá pracovat, když chodíš pořád pozdě. Je to od tebe nezodpovědné vůči ostatním. |
| `sa.s0.opt_c.feedback` | Hodnotíte charakter druhého a kritizujete místo hledání řešení. To obvykle vede k defenzivě. Zkuste popsat dopad na sebe a jasně požádat o změnu. |

### Scénář B: Potřeba pomoci s projektem

**ID:** `potreba-pomoci-s-projektem`

| ID | Text |
|----|------|
| `sb.title` | Potřeba pomoci s projektem |
| `sb.context` | Pracujete na důležité prezentaci a cítíte, že jste časově přetížení. Potřebujete, aby se na to s vámi někdo podíval, abyste se vyhnuli chybám. |
| `sb.goal` | Asertivně požádat kolegu o pomoc – přímo a s konkrétním návrhem. |
| `sb.s0.partner` | Hele, jak to máš s tou prezentací na středu? Potřebuješ něco? |
| `sb.s0.opt_a.text` | Potřebuju pomoc s prezentací, jsem teď časově přetížený. Měl bys zítra čas to se mnou projít? |
| `sb.s0.opt_a.feedback` | Správně. Žádost je přímá, srozumitelná a obsahuje konkrétní návrh. Respektujete své potřeby i čas kolegy. |
| `sb.s0.opt_b.text` | Asi bych potřeboval pomoct, ale nechci tě tím zdržovat, určitě máš dost své práce. |
| `sb.s0.opt_b.feedback` | Působíte nejistě a svou žádost v podstatě hned sami zpochybňujete. Kolega vás pravděpodobně odmítne, protože mu dáváte „východisko". |
| `sb.s0.opt_c.text` | Měl bys mi s tím pomoct, je to přece i tvoje vizitka a sám to všechno prostě neudělám. |
| `sb.s0.opt_c.feedback` | Používáte nátlak a vyčítáte. Tento styl komunikace vyvolává v druhém spíše odpor než ochotu pomoci. Zkuste požádat přímo a s respektem k jeho času. |

### Scénář C: Pozdní odevzdání podkladů

**ID:** `pozdi-odevzdani-podkladu`

| ID | Text |
|----|------|
| `sc.title` | Pozdní odevzdání podkladů |
| `sc.context` | Kolega vám odevzdal podklady pro vaši analýzu o dva dny později, než bylo domluveno. Kvůli tomu jste museli pracovat přesčas, abyste stihli finální termín. |
| `sc.goal` | Jasně popsat dopad na vás a definovat, co potřebujete příště. |
| `sc.s0.partner` | Promiň, že to přišlo o něco později. Stihl jsi to? |
| `sc.s0.opt_a.text` | To, že podklady přišly o dva dny později, mě donutilo pracovat přesčas. Příště potřebuji, abychom dodrželi domluvený termín. |
| `sc.s0.opt_a.feedback` | Správně. Jasně popisujete negativní důsledek jeho chování na váš čas (přesčas) a definujete, jak má spolupráce vypadat příště. |
| `sc.s0.opt_b.text` | (Nic neřeknete a podklady zpracujete bez komentáře.) |
| `sc.s0.opt_b.feedback` | Vyhýbáte se nepříjemné konverzaci, ale dáváte tím tichý souhlas k tomu, aby se termíny porušovaly i příště. |
| `sc.s0.opt_c.text` | Kvůli tvému zpoždění jsem tu musel tvrdnout do noci. Příště by ses měl víc snažit dodržet, co slíbíš. |
| `sc.s0.opt_c.feedback` | Zaměřujete se na obviňování a dáváte kolegovi najevo jeho selhání, což uzavírá cestu k věcné dohodě do budoucna. Zkuste popsat dopad a jasně říct, co potřebujete příště. |

---

## Kontrolní seznam po úpravě

- [ ] Úvodní text sedí s tím, co chcete studentům říct
- [ ] Počet scénářů v badge (`8 scénářů`) odpovídá skutečnosti
- [ ] Scénáře 1–8 jsou kompletní a konzistentní (ty/vy, ženský/mužský rod u partnera)
- [ ] Rozhodnuto: scénáře A–C doplnit do společné databáze, nebo ponechat jen 8 v sekci 6
- [ ] Texty „Pusť si M{n} …" v feedbacku – ponechat / zkrátit / odstranit
