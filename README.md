# Handleiding voor de leraar — Projectles 2: Muziek, tekst en geluid

**Vak:** Toegepaste Informatica · **Klas:** 3MWWE (2de graad Maatschappij- en welzijnswetenschappen, doorstroomfinaliteit)
**Soort les:** projectles 2 van *Dalton @ the movies* (lessenplan MWW § 7), in de plaats van een les uit het lessenplan; `lesnr` is `P2`
**Lesduur:** 1 × 50 minuten: 10 minuten instructie + 40 minuten keuzewerktijd · **Lokaal:** 18, Windows 11, Canva in Chrome + de eigen gsm met de Canva-app + oortjes
**Lesdag:** donderdag 29 oktober 2026, 8ste lesuur (14.35–15.25) · **Evaluatie:** geen punten: een leidraad (het eindproduct volgt in projectles 3)
**Kernleerplandoel:** `BV2_04.02` (toepassen), met `BV2_04.04`, `BV2_04.03` en `BV2_05.01` ondersteunend
**Opdracht in Classroom:** *Projectles 2 — Muziek, tekst en geluid* (onderwerp *Project Dalton @ the movies*), **0 punten, geen deadline**, alleen de link naar de lespagina

<!-- Beginvragen (stap 1 van CONTEXT.md), 25-10-2026. Jonas: "Je mag projectles 2 beginnen!" en koos in de chat telkens
     het voorstel:
     klas 3MWWE · projectles 2 van *Dalton @ the movies* (lessenplan MWW, § 7: "muziek uit de bibliotheek van Canva (met
     licentie), overgangen, titels, het geluid in balans, de voice-over (Engels)"), in de plaats van een les uit het
     lessenplan; `lesnr` `P2` · lesdag do 29 oktober 2026, 8ste uur (14.35–15.25) · vorige les: projectles 1 (Kennismaken
     met de montage), gegeven op do 22-10 → lesstart = ophalen uit projectles 1 · lokaal 18, Windows 11, Canva in Chrome
     (schoolaccount) + de eigen gsm met de Canva-app, zoals projectles 1 · **geen punten**: "Je moet dit niet op punten
     zetten, gewoon informatie dat ze kunnen volgen om een leidraad te hebben is goed" → een opdracht in Classroom zonder
     punten, met alleen de link naar de lespagina, geen werkdocument; de leerling klikt op *Markeren als klaar* ·
     de beginsituatie: hun leerkracht Nederlands was drie weken ziek, dus de groepen hebben nog geen duidelijk plan; ze
     filmden al clips en filmen er nog bij, en zetten ze (hopelijk) vóór de les in Canva (Jonas mailt hen daarvoor) →
     de leidraad begint met een **kort trailerrecept** (opening, personages, probleem, spanning, titel) om de clips in
     een volgorde te leggen; daarna titels, overgangen, muziek en geluid · de **voice-over** (Engels) is een **extra**
     voor wie de tekst al heeft; in projectles 3 kan het nog · context *Dalton @ the movies*, repository
     Muziek-DaltonMovies. -->

## 1. Inhoud van het pakket

```text
W09 - Project 2 - MWW - Muziek tekst en geluid/
├── index.html              de lespagina: startpagina in beelden · route · één stap · checklist
├── presentatie.html        9 dia's; dia 1 is de vaste startdia "Zo start je"
├── css/style.css           lespagina (projectles 1 + .tl3, de tijdlijn met drie lagen, .monteur, .recept, .ov2, .mag)
├── css/slides.css          dia's (projectles 1 + .tl3b, .rec5, .demo2)
├── js/script.js, js/slides.js
├── assets/                 logo "Dalton @ the movies", GO! Dalton Gent, lettertypes (OFL), mascotte Dalton, logo's classroom/docs/lespagina,
│                           stapjes/ (13 + 3 nieuwe schermafbeeldingen van Canva, 6 oude van de gsm en Projecten)
├── lesvoorbereiding.md · dalton-lesfiche.html · lesdoelen.json · classroom.json · README.md
```

**Geen werkdocument, geen zip, geen bronbestanden, geen zelftest, geen codewoord, geen filmpje *Inleveren*** (Jonas, 25-10-2026: "Je moet
dit niet op punten zetten, gewoon informatie dat ze kunnen volgen om een leidraad te hebben is goed"). De map `werkdocument/` van het
sjabloon is weggehaald; `controleer_les.py` meldt er niets over. De verbetertool slaat de les over (`_tools/verbeteren-uitzonderingen.json`).
Wat de groep maakt, staat in haar Canva-ontwerp; de titel en de maker van de muziek staan helemaal achteraan in de tijdlijn (de basis van de
aftiteling in projectles 3).

### 1b. Hoe de lespagina werkt

- **Startpagina**: *Wat heb je nodig?* in drie beelden (de opdracht met **Markeren als klaar**, de lespagina, het Canva-ontwerp met de gsm),
  *Dit maak je vandaag* (de tijdlijn met drie lagen: titel bovenaan, de clips in vijf blokken, muziek met vervaging), *Na deze les kan je*, *Vast?*.
- **Een leidraad voor groepjes van drie in één gedeeld Canva-ontwerp.** Bovenaan elke stap staat **wie monteur is** (`.monteur`): de groep geeft zich
  in stap 1 de letters A, B en C; monteur is A (stap 2), B (3), C (4), A (5), B (6). De anderen zoeken muziek of bedenken de tekst. Met twee of vier: afwisselen.
- **Handelingen met stapjes** zoals projectles 1: start in *Kort* (`data-modus-start="kort"`), *Toon stapjes*, geen knop *Stap voor stap / Kort*.
  Infokaders: *Het trailerrecept* (stap 2), *Waar staat wat in de tijdlijn?* (stap 3), *Harde overgang of Oplossen?* (stap 4), *Welke muziek mag je
  gebruiken?* (stap 5), *Zie je dit in jullie trailer?* (stap 6, groen: *Kijk na*).
- **Stap 6** eindigt met **Markeren als klaar** (een tekening van Classroom, niet gezien: zie § 8). Geen slot, geen codewoord.
- **Extra** (telt niet mee): de voice-over (Engels) voor wie de tekst al heeft, en een animatie op de titel.
- **Dia 8** toont de kloktijden van do 29-10, 8ste uur (14.35–15.25), met stap 1 als *samen ✓*; **T** rekent opnieuw.
- **Mascotte Dalton**: startpagina, stap 6, eindmelding; dia 2, 8 en 9. Niet op dia 3 (vijf blokken in een rij: geen plaats). `data-ai-hulp="uit"`.
- **Route**: stap 1–2 *De trailer opbouwen*, stap 3–6 *Afwerken met tekst en geluid*, *Extra*.

## 2. Klaarzetten

### Stap 1 — Publiceren via GitHub Pages

Repository [`jonasdaltongent/Muziek-DaltonMovies`](https://github.com/jonasdaltongent/Muziek-DaltonMovies), Pages op branch `main`, map `/ (root)`.
Lespagina: <https://jonasdaltongent.github.io/Muziek-DaltonMovies/> · dia's: <https://jonasdaltongent.github.io/Muziek-DaltonMovies/presentatie.html>
(het adres staat ook op dia 8 en in `classroom.json` en `lesdoelen.json`). *Status: zie `_index/lessen.md` en `_index/logboek.md`.*

### Stap 2 — De opdracht in Classroom, met de koppeling

Als **concept** in [3MWWE - Informatica](https://classroom.google.com/c/MjUzNjQyOTk0NDFa), onder het onderwerp **Project Dalton @ the movies**.
Inplannen op do 29-10 om 14.05 doet de hoofdsessie na het nakijken (`_afspraken/publiceren.md`).

| | Opdracht: **Projectles 2 — Muziek, tekst en geluid** |
|---|---|
| **Onderwerp** | Project Dalton @ the movies |
| **Bijlage** | alleen de link naar de lespagina (geen werkdocument) |
| **Punten · deadline** | geen · geen |

Instructietekst (`classroom.json`):

```text
1. Open de lespagina (link): dat is je leidraad voor vandaag. Er staan geen punten op.
2. Je werkt in het Canva-ontwerp van je groep. Je hebt je gsm nodig, met de Canva-app, en oortjes als je die hebt.
3. Klaar? Klik op Markeren als klaar.
```

### Stap 3 — Met de hand, als de koppeling niet werkt

Maak in Classroom een opdracht met het onderwerp *Project Dalton @ the movies*, **zonder punten en zonder uiterste inleverdatum**, en voeg met
**Bijvoegen** › **Link** de lespagina toe.

### Afvinklijst vóór de les

Met een **leerlingaccount** nakijken (zie ook § 8). Je scherm wint van de lespagina.

- [ ] **Oortjes gevraagd in de mail** (zeven groepen die tegelijk muziek afspelen is te veel), samen met: alle clips vóór do 29-10 in het Canva-ontwerp van de groep zetten (met de Canva-app: op de clip tikken).
- [ ] **Demo-ontwerp met twee of drie stockvideo's** in je eigen Canva (Video › Liggende video; bij **+** › **Stockvideo's**), voor de overgang en de muziek (dia 4).
- [x] Knopnamen van tekst, transitie, audio, volume, vervagen en voice-over nagekeken met demoleerling3 (25-10-2026, § 2b).
- [x] De schoolaccounts zien popmuziek (label **EDU**, 1:00); Pro-muziek (kroontje) zagen we niet in de lijsten (25-10-2026).
- [ ] De dia's staan op het bord; de kloktijden kloppen met het lesuur.
- [ ] Het wachtwoord van de computers op het bord (niet op een dia).

### 2b. Nagelezen klikpaden

Gezien op het scherm van het leerlingaccount **demoleerling3** (25-10-2026, Chrome, in het testontwerp *Trailer – De laatste bus* met een
sjabloon vol stockvideo's; er is niets gedeeld, verstuurd of opgenomen). Op de lespagina staan:
**Tekst** › **Voeg een tekstvak toe** (de help schrijft *Een tekstvak toevoegen*), het tekstblok op de bovenste track met zijn rand,
**Animeren**; tussen twee clips het knopje **Transitie toevoegen** (staat er al een overgang: **Overgang wijzigen**), het paneel **Overgangen** met
**Geen** · **Oplossen** · **Schuiven** … en **Duur (seconden)** (de help schrijft *vervaging*; het scherm zegt **Oplossen**);
**Elementen** › **Audio** (een categorie onder *Categorieën doorbladeren*, geen tabblad) met bovenaan **Voice-over opnemen** (daarna een balk met de
knop **opnemen**) en lijstjes als *Film*; het gekozen nummer: het luidsprekertje **Volume** (met een schuif, een getal en **Alles evenwichtig
maken** — de help schrijft *Alles in evenwicht brengen*), **Vervagen** met **Vervaging aan het begin** en **Vervaging aan het einde**; rechtsklik op het nummer:
**Aanpassen** · **Vervagen** · **Beat Sync** · **Volume**. Zie het verslag van de lesbouwer voor het voorstel voor `_afspraken/klikpaden.md`.
**Markeren als klaar** komt uit de Nederlandse Classroom-help ([6020285](https://support.google.com/edu/classroom/answer/6020285?hl=nl), gelezen 25-10-2026: "Afhankelijk van het type opdracht en bijlagen staat er Inleveren of Markeren als klaar"); in de chat van 25-10 stond *voltooid*, maar dat was het woord van de AI. Op een leerlingscherm nog niet gezien (§ 8).

## 3. Het verloop van de les

Zie `lesvoorbereiding.md` § 15–17 en de notities bij elke dia. In het kort: dia 1 (aanmelden; vraag naar de oortjes), dia 2 lesstart (*waar staat mijn
upload?*), dia 3–5 *Ik doe* (het trailerrecept, **demo live in Canva**: overgang en muziek zachter, de tijdlijn met drie lagen), dia 6 controle (*Spotify?*),
dia 7 *Iedereen doet stap 1* (4'), dia 8 keuzewerktijd, dia 9 de exitvraag (wat zet je achteraan?).

- **Eerste rondgang (stap 2):** staan de clips in vijf blokken, en stopt de trailer vóór het einde? Is er één monteur tegelijk?
- **Tweede rondgang (stap 5):** is de muziek zachter dan de stemmen, en komt ze uit Canva? Heeft iedereen oortjes?
- Mondeling op het einde: *klik op Markeren als klaar, ook als jullie niet klaar zijn; in projectles 3 werken jullie verder.*

## 4. Wat je moet zien (geen verbetersleutel)

Er wordt niets ingeleverd en er zijn geen punten: de checklist van stap 6 is de feedback voor de groep. Per groep verwacht je in Canva:

| Stap | Wat je verwacht te zien |
|---|---|
| 2 | de clips in de vijf blokken van het recept; clips in blok 4 kort (1 à 2 s); de clips van het einde zijn weg |
| 3 | een titel op de bovenste track, groot en in een kleur die afsteekt, zo lang in beeld dat je hem twee keer leest |
| 4 | minstens één overgang (**Oplossen**, kort); in de spanning harde overgangen; niet bij elke clip een andere |
| 5 | een nummer uit Canva op een audiotrack, zachter dan de stemmen, met vervaging; titel en maker in een tekstvak helemaal achteraan |
| 6 | de hele trailer afgespeeld; wie herkenbaar in beeld staat, weet dat de trailer getoond wordt; in Classroom op **Markeren als klaar** geklikt |

### Essentiële fouten — geef hier mondeling feedback op

- Een liedje van Spotify of YouTube geüpload in plaats van muziek uit Canva (geen geluid bij het publiceren).
- De muziek even luid als de stemmen.
- De trailer vertelt het einde van de film.
- Twee groepsleden die tegelijk op de tijdlijn slepen.
- Iemand herkenbaar in beeld die niet weet dat de trailer getoond wordt.

## 5. Schermafbeeldingen (optioneel)

`assets/stapjes/canva-*.png` (nieuw, 25-10-2026): `zoom`-opnames van Claude in Chrome met het profiel van demoleerling3 (Profile 8), uitgesneden met
één rood kader met witte rand (Pillow); geen namen, geen e-mailadressen. Opnieuw maken: een testontwerp *Liggende video* openen en dezelfde kaders
opnemen. `canva-met-jou-gedeeld.png`, `canva-stockvideos.png` en `gsm-*.png` komen uit projectles 1 (18-10-2026).

## 6. Het materiaal opnieuw maken

Er is geen script: alles is HTML en CSS. De kloktijden: `python3 _tools/zet_lesmomenten.py "<lesmap>"` (zet `2026-10-29/14.35/15.25/3MWWE/8`).

## 7. Leerplandoelen in je jaaroverzicht

`lesdoelen.json` (`klasgroepen` `3 MWW`): `BV2_04.02` (kern), `BV2_04.04`, `BV2_04.03`, `BV2_05.01` (ondersteunend). De pre-push hook schrijft ze naar het jaaroverzicht.

## 8. Wat nog moet blijken in de klas

Nagekeken op 25-10-2026 met het leerlingaccount demoleerling3 (computer): tekstvak, transitie, het paneel Overgangen, Audio, Volume, Vervagen,
Voice-over opnemen (de balk met **opnemen**; niets opgenomen). Nog niet te testen:

1. **Markeren als klaar** in Classroom bij een opdracht zonder punten en zonder bijlage om in te leveren: de naam komt uit de help (6020285), op de
   lespagina staat een tekening. Staat er op het scherm van de leerling echt *Markeren als klaar*? Krijgt de leerling nog een venster om te bevestigen?
2. **De microfoon**: vraagt Canva of Chrome om toestemming bij **opnemen**, en hebben de computers van lokaal 18 een microfoon? (Niet geklikt: er is niets opgenomen.)
3. **Een titel op een andere plaats dan het begin**: het tekstvak kwam in onze test op de afspeelkop (op 0:00); of het ook elders op de afspeelkop komt, is niet gezien.
4. **De Canva-app op de gsm** (zoals in projectles 1: gezien in de gsm-modus van Chrome, niet in de app).
5. **Luisteren naar een nummer in de lijst** (op het plaatje klikken?) zonder het in het ontwerp te zetten: een klik op de titel zette het wel in het ontwerp.
6. Het label **EDU** (bekende muziek, 1:00) en de melding *Je gebruikt populaire muziek* die verschijnt bij zo'n nummer: begrijpen de leerlingen ze, en kiezen ze liever een nummer zonder?
7. **Het knopje met de naam *Briefje*** in de balk van een gekozen nummer (machinale vertaling; we weten niet wat het doet): staat niet op de lespagina.
8. Clipvolume (*zet ook het volume van de clip lager*): staat als grijze regel in stap 5, voor de clips niet zelf aangeklikt.
9. Heeft elke groep clips in het ontwerp (de mail), oortjes, en lukt het wisselen van monteur? Tijdsduur van de stappen (stap 5 in 11 minuten).
