# Safarispill 🦁

Et læringsspill for 3. trinn med matte, norsk og engelsk, og safari som ramme.
Hver fullført safari (12 oppgaver) låser opp et nytt dyr i safariboka. Antall riktige svar
bestemmer hvilken fotball-liga økta havner i: OBOS-ligaen, Eliteserien, Premier League, Europa League
eller Champions League. Streaken teller hvor mange dager på rad det er spilt.

* Én fil: `index.html` med CSS og JS inni. Det trengs ikke noe byggesteg, ingen API-nøkler, og spillet virker uten nett.
* Fremgangen lagres i nettleserens `localStorage` (nøkkel `kari-safari-v1`) på enheten det spilles på.
* Vanskelighetsgraden tilpasser seg i hvert fag (nivå 1–5): tre riktige på rad gir høyere nivå.
* Hele innholdet står i `innhold-oversikt.md`.

## Ukens tema
Øverst i `<script>` ligger `WEEK_CONTENT`, med én nøkkel per ISO-uke. Den inneholder bare temaer og egne
spørsmål (første svaralternativ er riktig) og aldri detaljer fra ukeplaner. Spillet velger uka som passer med dagens dato.
Under ⚙️ kan man velge en annen uke.

## Ukens gloser
Hver uke i `WEEK_CONTENT` kan ha `gloser: { tema, words:[{e, en, no}], phrases:[{en, no}] }`. Se `GLOSER_CLOTHES` for et eksempel.
Da vises knappen «💬 Ukens gloser» på forsiden. Den gir en ordliste med 🔊, flashcards og en glosequiz med 8 spørsmål.
Quizen gir poeng og stjerner, men påvirker ikke ligaen, streaken eller nivået.
