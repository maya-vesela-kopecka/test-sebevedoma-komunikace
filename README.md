# Test – Sebevědomá komunikace

Interaktivní test a role-play k microsérii **Sebevědomá komunikace** (Lenka Dědicová, Seduo). Studenti ověří znalosti ze 11 microkurzů, vyberou výzvy k akci a mohou procvičit reakce ve scénářích.

## Co je v balíčku

| Stránka | Popis |
|---------|--------|
| [index.html](index.html) | Úvodní stránka – výběr způsobu procvičení |
| [roleplay.html](roleplay.html) | Výběr z možností (8 scénářů) |
| [roleplay-free.html](roleplay-free.html) | Vlastní odpovědi |
| [scenarios.json](scenarios.json) | Data scénářů pro role-play |

## Publikace na GitHub Pages

1. Vytvořte na GitHubu **veřejné** repo `test-sebevedoma-komunikace`.
2. V této složce (pokud ještě není git):

   ```bash
   git init
   git add .
   git commit -m "Publikovatelná verze testu sebevědomé komunikace"
   git branch -M main
   git remote add origin https://github.com/VASE_UZIVATELSKE_JMENO/test-sebevedoma-komunikace.git
   git push -u origin main
   ```

3. Na GitHubu: **Settings → Pages → Build and deployment → Source**: Deploy from branch → **main** → folder **/ (root)** → Save.
4. Po ~1 minutě bude test na adrese:

   `https://VASE_UZIVATELSKE_JMENO.github.io/test-sebevedoma-komunikace/`

## Zpětná vazba (Typeform)

Po dokončení testu studenti uvidí odkaz na dotazník:

[https://lmc4.typeform.com/to/emV4D50T](https://lmc4.typeform.com/to/emV4D50T)

Odpovědi se sbírají v Typeform dashboardu.

## Google Analytics (později)

Měření zatím není zapnuté. Až budete mít GA4 Measurement ID (`G-XXXXXXXXXX`), lze doplnit soubor `analytics.js` a načíst ho ze všech HTML stránek.

## Poznámka k AI

Na všech stránkách je upozornění, že test byl vytvořen ve spolupráci s AI.

## Licence / použití

Materiál je určen pro vzdělávací účely v rámci microsérie Seduo. Logo a obsah microkurzů patří příslušným držitelům práv.
