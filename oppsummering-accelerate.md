# Oppsummering: _Accelerate, The science of lean software and DevOps_

_Building and scaling high performing technology organizations.  
Bok av Gene Kim, Jez Humble, og Nicole Forsgren._

---
## Publisert på Smidigalliansens blogg
Oppsummeringa har blitt publisert på https://medium.com/smidigalliansen/oppsummering-av-accelerate-the-science-of-lean-software-and-devops-c575cabbbb38. Les den heller der.
---

Boka handler om hva som skal til for å bli en mer leveransedyktig og høytpresterende IT-organisasjon, som leverer mer verdi på kortere tid. Den baserer seg på [_State of DevOps_-rapportene](https://puppet.com/resources/whitepaper/state-of-devops-report) (global undersøkelse) fra 2014-2018. Forfatterne går vitenskapelig til verks i å forklare hva, hvorfor og hvordan rundt både ledelse og tekniske metoder og praksiser.

Boka er tredelt: 

1. Resultater fra undersøkelsene. 
2. Vitenskapen bak undersøkelsene (hvordan stille riktige spørsmål på riktig måte, jobbe med statistikken osv). 
3. Case studie fra ING (bank i Nederland), som har gjennomgått en smidig transformasjon. 

Denne oppsummeringen tar for seg resultatene fra undersøkelsene.

---

**TL;DR**: Lean management, kultur og kontinuerlig leveranse har alt å si. For å være konkurransedyktig, holder det ikke lenger med _business as usual_. Store prosjekter med lang ledetid (tid fra start til kunde har noe kjørende) er avleggs. I stedet bør man ha små teams som jobber i korte iterasjoner, med løpende feedback fra brukere, for å lage produkter og tjenester som brukerne liker og som skaper verdi. Kontinuerlig forbedring, i måten å jobbe på, er viktig. 

--- 

Måling av prestasjon er brutt ned til fire separate målepunkter:

1. **Delivery lead time (Lean)**  
Her er ledetid målt som tiden det tar fra kode committes, til den kjører i produksjon / release. Kort ledetid er bra da det muliggjør korte _feedback loops_ (kjapp tilbakemelding fra brukere) på det som lages, slik at vi kan korrigere kursen tidlig og ofte. 

2. **Deployment frequency / batch size (Lean)**  
Å levere få endringer i slengen (_small batch size_), gjør at en får de ut raskere. Det gir bedre flyt, reduserer risiko og overhead, forbedrer effektiviteten, øker motivasjonen og reduserer kostnader. I boka er _deployment frequency_ brukt som en proxy for _batch size_, da _batch size_ er relativt og vanskelig å måle på tvers av de man undersøker.

3. **Time to restore service**  
Hvor lang tid tar det å gjenopprette når noe feiler eller går ned?

4. **Change fail rate**  
Hvor stor andel av endringene som gjøres, forårsaker feil?

Høytpresterende organisasjoner scorer bra på alt dette. Det viser at man ikke nødvendigvis må velge mellom hastighet, kvalitet og stabilitet. Man _kan_ få alt. De siste årene har de høyest presterende organisasjonene rykket fra røkla, slik at forskjellen øker. De beste forbedrer seg kontinuerlig. 

Høytpresterende organisasjoner har:  
- 46 ganger hyppigere deploy av kode.
- 440 ganger kortere ledetid fra commit til deploy.
- 170 ganger raskere gjenoppretting etter feil og nedetid.
- 5 ganger lavere change/failure rate.

---

Boka avdekker 24 nøkkelegenskaper og drivere for høy prestasjon. Egenskapene er delt opp i fem kategorier:

- Kontinuerlig leveranse
- Arkitektur
- Produkt og prosess
- Lean management og monitorering
- Kultur


## Kontinuerlig leveranse
Kontinuerlig leveranse er sett med egenskaper og teknikker som gjør det mulig å få alle slags endringer ut i produksjon på en kjapp, trygg og kontrollert måte. Prodsetting / release bør være en enkel rutine, som kan utføres når som helst og innenfor vanlig arbeidstid.

Kontinuerlig leveranse betyr at programvaren alltid er i en releasebar tilstand, og at teamet prioriterer releasebarhet over nye features. Informasjon om kvalitet og releasebarhet bør være tilgjengelig for alle teammedlemmer hele tiden. Når systemet ikke er i en releasebar tilstand, blir det fikset med en gang.

Disse fem prinsippene er selve kjernen av kontinuerlig leveranse:

- **Innebygget kvalitet**. Reduserer behovet for manuell testing og inspeksjon. Feil bør oppdages tidlig (gode automatiserte tester), slik at de kan fikses der og da, mens de fortsatt er billige å fikse.

- **Arbeide med små bolker om gangen**. Gir raskere gir målbar verdi (_business outcomes_) for kundene. Muliggjør også korte feedback loops (tidlig tilbakemelding fra brukere), som muliggjør tidlig kursendring for å lage et bedre produkt.

- **Datamaskiner gjør repeterende arbeid – mennesker løser problemer**. Repeterende og tidkrevende arbeid, som regresjonstesting og deployment / installering, bør i størst mulig grad automatiseres, slik at kapasitet frigjøres til mer verdiskapende arbeid.

- **Kontinuerlig forbedring**. Ikke vær fornøyd, men press på for å forbedre og jobbe smartere hele tiden.

- **Felles ansvar**. En må samarbeide på tvers av avdelinger for å nå organisasjonens overordnede mål (_system level outcomes_). Det er et lederansvar å sørge for at alle til enhver tid vet hvordan organisasjonen ligger an mht ønsket overordnet utfall, samt jobbe med hele organisasjonen for å få definert målbare, oppnåelige og tidsbegrensede mål, slik at alle drar i samme retning. Typisk for byråkratiske organisasjoner, er at avdelinger måles på ulike og motstridende ting, slik at de i stedet ender med å motarbeide hverandre (f.eks drift vs utvikling).

De som er gode på kontinuerlig leveranse..  

- Bruker mindre tid på ikke-planlagt arbeid og dobbeltarbeid, som kunne vært ungått, enn andre. 
- Oppnår høyere prestasjon (lead time, deploy frequency, time to restore service)
- Har lav change / fail rate
- Har en bedre og mer positiv og utforskende (generativ) kultur
- Identifiserer seg sterkt med organisasjonen de jobber for.
- Har uproblematiske og enkle deploys. Ingen _deployment pain_ (frykt og ubehag knyttet til deploy / release).
- Opplever mindre utbrenthet 

Innføring av kontinuerlig leveranse krever imidlertid ofte at en må tenke helt nytt – fra hvordan teams fungerer og hvordan de samhandler med hverandre, til hvilke verktøy og prosesser de bruker. Resultatet er at det skapes et miljø hvor de i større grad tar ansvar for globale utfall som høy kvalitet og stabilitet.


**Følgende er viktige drivere og egenskaper for kontinuerlig leveranse:**

### Nesten alt i versjonskontroll
Undersøkelsene viser at konfigurasjon i versjonskontroll, er sterkere korrelert til høy prestasjon enn kode i versjonskontroll. Miljøer bør kunne provisjoneres, og kode bør kunne bygges, testes og deployes automatisk fra versjonskontroll. Legg alt, bortsett fra data, i versjonskontroll.

### Automatisert deploy
Deploy bør ikke kreve manuelle steg.

### Continuous integration
Første steg på veien mot kontinuerlig leveranse. Det er en praksis hvor kode merges ofte til et delt repository. Hver endring trigger en bygge-, test- og deployprosess (til testmiljø e.l). Dersom noe feiler, fikses det der og da.  Kortlevde brancher (under en dags arbeid) er enklere å merge / integrere enn brancher som lever i flere dager og uker, og det skaper mindre overhead.

### Trunk-based development
Undersøkelsene viser at kortlevde brancher er sterkt korrelert til høy prestasjon. De beste teamene har som regel færre enn tre aktive brancher på samme tid, og branchene lever typisk kortere enn en dag før de merges til master. Videre opplever disse teamene sjelden eller aldri kodefrysperioder. Dette er uavhengig av team- eller organisasjonsstørrelse og type industri.   

### Automatisiert testing
Automatiserte tester bør kjøres kontinuerlig gjennom hele utviklingsløpet, og trigges automatisk ved commit / push (som del av deployment pipeline). De må være pålitelige og finne reelle feil, slik at bare releasebar kode godkjennes. Utviklere bør også kunne kjøre automatiske tester lokalt på / fra maskinene sine, for å være i stand til å vurdere, rangere og fikse defekter.

Slike tester bør skrives og vedlikeholdes av utviklere. Da oppnår en to viktige ting;
- Koden blir mer testbar. TDD tvinger frem mer testbar kode.
- Utviklerne bryr de seg mer om testene – og investerer dermed også mer tid og innsats i å vedlikeholde de.

Automatiske tester som lages og vedlikeholdes av QA-avdeling eller annen tredjepart har ingen korrelasjon til bra leveransetakt og -evne. Testere spiller fortsatt en viktig rolle. De bør gjøre manuell og utforskende testing / akseptansetesting, samt jobbe sammen med utviklere om å lage / definere automatiske tester. Siste bygg bør alltid være tilgjengelig for testere (manuell utforskende testing).

### Test data management
En må ha nok testdata til å kjøre alle automatiske tester. Testdata, eller mangel på det, må ikke danne føringer / begrensninger for hvilke tester en kan kjøre. Samtidig er det poeng å ikke ha for mye testdata også (effektivitet, vedlikehold osv). Testdata må være tilgjengelig på forespørsel / ved behov.

### Test sikkerhet tidlig (Shift left on security)
Å integrere sikkerhet tidlig i utviklingsprosessen og gjennom hele livssyklusen til et produkt, er viktig for leveranseevne og kvalitet. Det gir mindre brannslukking. 

Sikkerhetseksperter må være proaktive og bidra i applikasjonsdesign, gi feedback underveis i utviklingen, samt sørge for at sikkerhet inngår i den automatiserte testriggen. De må gjøre det enkelt for utviklere med flere å gjøre de rette tingene mtp sikkerhet. 

Det er motsatt fra den mer tradisjonelle tilnærmingen, hvor en gjør sikkerhetsgjennomgang på tampen – når det er både dyrt og vanskelig å gjøre endringer. 

_Det samme kan sies om f.eks universell utforming også_.


## Arkitektur
Høy leveransetakt og -evne er mulig med alle slags systemer, så fremt både systemene og teamene, som bygger og vedlikeholder de, er løst koblet. Det muliggjør at man enkelt kan teste og deploye individuelle komponenter og tjenester, selv om organisasjonen og antall systemer skaleres. 

Følgende egenskaper (_deployability and testability_) er viktige for høy leveransetakt:

1. Teamet må kunne endre, deploye og release applikasjoner uten avhengigheter til andre applikasjoner og teams.
2. Teamet kan gjøre større endringer i design av et system uten å måtte innhente godkjenning fra eksterne (noen utenfor teamet).
3. Teamet kan ferdigstille arbeid uten å koordinere med utenforstående.
4. Teamet kan release et produkt eller tjeneste ved behov og på forespørsel.
5. Teamet kan gjøre det meste av testing på sparket, uten behov for et integrert testmiljø (integrated test environment).
6. Deploy kan gjøres innenfor vanlig arbeidstid, uten nevneverdig nedetid.
7. Teamene kan velge verktøyene sine selv.

Der en scorer høyt på slike arkitekturegenskaper, kreves lite kommunikasjon mellom ulike teams for å få jobben gjort. Arkitekturen er designet for at teamene skal kunne jobbe (endre, teste, deploye) selvstendig og uavhengig av andre. Både teamene og arkitekturen er da **løst koblet**. 

En løst koblet og velfungerende IT-arkitektur med en matchende organisasjonsstruktur, muliggjør to ting:
1. Bedre leveranseevne med økt tempo og stabilitet, mens utbrenthet og _deployment pain_ reduseres.
2. Organisasjonen kan vokse, mens produktiviteten samtidig øker lineært, eller bedre. 

Det motsatte er gjerne tilfelle for _low performers_. Flere utviklere = færre deploys per tidsenhet per utvikler.

For å oppnå dette må vi ha **kryssfunksjonelle teams**, som besitter all nødvendig kompetanse for å designe, utvikle, teste, deploye og drifte systemene.

### Arkitektur gjenspeiler organisasjonsstruktur
Conways lov sier at IT-arkitekturen gjenspeiler organisasjonsstrukturen. Forskningen, som gjennomgås i boka, underbygger det som ofte kalles _Inverse Conway maneuver_; Organisasjons- og teamstruktur må designes etter den arkitekturen en ønsker å oppnå. Målet med IT-arkitekturen er å støtte teamene i å få jobben gjort – fra design til utrulling – med lav båndbredde på kommunikasjonen mellom teamene. Kommunikasjon mellom systemer løses med mikrotjenester og veldefinerte API-er.

Teams bør snakke sammen, men de bør bruke “båndbredden” til å snakke om felles overordnede mål og hvordan de kan nås, fremfor implementasjonsdetaljer.


## Lean og smidig produktutvikling
Har smidig utvikling positiv innvirkning på organisasjonens prestasjon, målt i produktivitet, markedsandel og profitt? Ja.

Smidig er jevnt over den foretrukne utviklingsmetoden, men blir ofte mangelfullt implementert. Organisasjonskultur og mer overordnede samarbeidsprosesser blir ikke tatt tak i. Det er fortsatt vanlig at bedrifter bruker lang tid på budsjettering, analyser og innhenting av krav før utviklingsarbeidet starter, for så å release i store bolker og ved ujevne mellomrom. Tilbakemeldinger fra kunder er uten innvirkning på sluttresultatet, og blir bare til ettertanke.

**Lean / smidig produktutvikling** står for det motsatte; Eksperimentell tilnærming med hyppig brukertesting av både design og forretningsmodell, fra starten av produktets livssyklus. Arbeidet deles opp i mindre bolker som leveres fortløpende.

Effektivisering av leveranseprosessen gjør det enklere å jobbe med mindre bolker om gangen, samt innhente bruker-feedback underveis. Å levere i mindre bolker gir raskere _feedback loops_.

**Følgende er viktige egenskaper for en effektiv prosess:**

### Innhente og dra nytte av tilbakemelding fra brukere
Et poeng i smidig utvikling er å involvere brukerne tidlig i utviklingsløpet, for å få nyttig input og tilbakemeldinger. Disse tilbakemeldingene brukes så videre i neste steg av prosessen, før man jakter nye tilbakemeldinger igjen (_feedback loop_).

Forskningen viser at å aktivt søke tilbakemeldinger fra brukere, samt inkorporere lærdommen i produktet, er viktig for prestasjonen.

### Visualisering av oppgaveflyt og verdikjede
Visualisering av prosess og gjennomstrømming av oppgaver, samt oversikt over og forståelse av verdikjeden (hele veien fra forretning til kunde), har betydning for leveranseevnen.

Visualisering (f.eks Kanban) av arbeidsflyten og gjennomstrømming av oppgaver gjør det enkelt for alle å se hvem som jobber med hva, hva som er status på ulike oppgaver, hvor mange baller som er i lufta og hvorvidt noe er blokkert – som i at involvering av utenforstående og / eller eskalering er nødvendig. Det får igang viktig kommunikasjon.

### Arbeide med små bolker om gangen
En bør dele opp arbeidet i små biter som kan ferdigstilles på en uke eller mindre. Det gir hurtigere og mer effektiv utvikling enn å jobbe med store og komplekse features på egne brancher over lang tid. Det gir kortere ledetid og raskere feedback loops.

### Eksperimentering
Hvis teamet ikke får lov til å reagere på læringen fra tilbakemeldingene, uten godkjenning fra noen utenfor teamet, reduseres innovasjonsevnen drastisk. Organisasjonens prestasjon (profitt, produktivitet og markedsandel) reduseres også.

En forutsetning for effektiv eksperimentering er at det jobbes med små bolker om gangen, at arbeidsflyten gjennom leveranseprosessen er visualisert og at at bruker-feedback inkorporeres i produktets design. Det gir gjennomtenkte beslutninger, som kommuniseres ut i organisasjonen (visualisering av prosess og oppgaver). Det øker også sannsynligheten for fornøyde brukere og at det skapes verdi.

## Lean management
Lean management fører til bedre kultur (generativ), bedre leveranseevne og redusert utbrenthet.

*Følgende er viktige egenskaper ved lean management:*
 
### Enkel prosess for godkjenning av endringer
Parprogrammering og pull request internt i teamet, kombinert med deploy pipeline (push - bygg - test - deploy / release) for å bl.a oppdage og avslå endringer av lav kvalitet, er effektivt. Deploy / release bør være en helautomatisert prosess, som trigges gjennom deployment pipeline.

Teams som må ha code review og godkjenning av noen utenfor teamet (f.eks _change advisory board_), presterer dårligere. Det gir heller ikke bedre stabilitet. 

Ekstern godkjenning gir lengre ledetid, tregere leveransetakt og har ingenting å si for change/failure-rate. Det er verre enn å ikke ha en godkjenningsprosess i det hele tatt. I boka blir det blir beskrevet som “**risk management theater**”. Det er teamet som kjenner systemet og som best forstår effekten av endringene.

### Overvåking av applikasjoner og infrastruktur
Data og lærdom fra overvåking av applikasjoner og infrastruktur kan brukes til å treffe bedre beslutninger. I tillegg til overvåking for varsling feil, bør man kjøre helsesjekker som kan varsle basert på terskelverdier og rate-of-change warnings, f.eks om CPU har økt med 25% de siste 10 minuttene.

Synligheten og gjennomsiktigheten som oppnås ved effektiv overvåking er uvurderlig. Proaktiv monitorering er sterkt relatert til høy prestasjon og medarbeidertilfredshet, og er en viktig del av en teknisk rigg.

### WIP-limits og visualisering av arbeid
_Work in progress (WIP) limit_ definerer hvor mange oppgaver teamet kan håndtere samtidig. Meningen med _WIP-limits_ er å optimalisere flyt (gjennom å f.eks unngå _context switching_) ved å begrense antall samtidige oppgaver. Det øker gjennomstrømningen av oppgaver og synliggjør flaskehalser.

Et interessant funn er at _WIP-limits_ alene ikke har stor betydning for leveranseevne. Det er først når det kombineres med visuelle oversikter (f.eks kanban-tavler / skjermer, som viser _work in progress_) og feedback loops fra produksjon, at WIP-limits gir stor verdi. Det hindrer at teamet har for mange oppgaver, som vil gi lengre ledetid.

 
## Kultur
En bedre kultur bygges gjennom kryssfunksjonelt samarbeid, å skape rom og tradisjon for læring, samt sørge for effektiv bruk av verktøy.

**Følgende egenskaper er viktige egenskaper i en god kultur:**

### Generativ kultur
En generativ kultur kjennetegnes av god informasjonsflyt, høy grad av samarbeid og tillit, brobygging mellom teams, felles ansvar, nye ideer ønskes velkommen, man oppfordres til å si fra om feil og mangler (_messenger not shot_) og man holder såkalte _blameless postmortems_ hvor man lærer av feil fremfor å plassere skyld.

En slik kultur er prestasjonsfremmende for organisasjonen. Det gir bedre leveranseevne og reduserer utbrenthet.

### Rom for læring og forbedring
Man kan stimulere til innovasjon og initiativer gjennom å investere i teamene:
 
- Ha et eget kompetansebudsjett, og oppfordre til å bruke det. La folk bestemme selv hvilke kurs, konferanser e.l de vil delta på, ut fra egne interesser og behov.
- Oppmuntre til deltagelse på minst en konferanse i året, og å i etterkant oppsummere hva man har lært for teamet / organisasjonen.
- Arranger hackathon / hack days, hvor tverrfaglige teams kan skape og prøve ut nye ideer.
- Arranger “yak days”, hvor det jobbes med teknisk gjeld (ikke nødvendigvis bugs) og forbedringer som ellers ikke prioriteres.
- Hold jevnlige interne minikonferanser (foredrag, lyntaler, workshops, open space etc)
- Sett av tid (google kjører 20%) til å eksperimentere med nye verktøy og teknologier.
- Gjør det trygt å feile. Represalier gjør at folk ikke tør prøve nye ting. Feiling må ses på som en mulighet til læring. Kjør _blameless postmortems_ for å finne ut hvordan prosesser og systemer kan forbedres. Det bidrar til innovasjon og kultur.

### Samarbeid mellom teams
En kan stimulere til kryssfunksjonelt samarbeid ved å

- Bygge tillit mellom teamene (åpen kommunikasjon, lovnader holdes, forutsigbar opptreden selv under stress). 
- Tilrettelegge for flytting mellom avdelinger og teams. Om noen bytter til en annen rolle et annet sted i organisasjonen, kan det være av verdi for begge teams. Medarbeideren har med seg nyttig info om prosesser og utfordringer til det nye teamet, og det gamle får et naturlig kontaktpunkt for samarbeid.
- Aktivt søke, oppfordre til og belønne arbeid som krever kryssfunksjonelt samarbeid.

### Gjør arbeidet meningsfylt
Drivere for medarbeidertilfredshet:

- La teamene velge verktøyene sine selv. Om de har verktøy til å gjøre jobben slik de vil, blir de mer engasjerte (og effektive), og de gjør en bedre jobb. 
- Kultur for eksperimentering og læring gjennom utnytting av teknologi (f.eks automatisering) kombinert med prinsipper fra lean management.
- Ansatte har innflytelse på egen hverdag

Bedre medarbeidertilfredshet gir bedre prestasjon, som gir konkurransefortrinn. Høy prestasjon og leveransetakt har dessuten en selvforsterkende effekt; Teamene får validert ideene sine oftere, som gir høyere tilfredshet, som gir høyere prestasjon.

Det motsatte er fortsatt ofte tilfelle. Teams får overlevert kravspesifikasjoner, og må levere arbeid i store bolker om gangen. Det fører til liten kontroll over produktet som lages og hvilken effekt det har for kunder. Det er demotiverende, og de ansatte distanserer seg dermed mer fra organisasjonen, fremfor å identifisere seg med den. Det gir dårligere organisasjonskultur og dårligere prestasjon.

### Transformasjonsledelse
En god leder forsterker teamets evne til å levere høy kvalitet i høyt tempo. Høytpresterende organisasjoner har engasjerte ledere som er gode på teknologi- og transformasjonsledelse, noe som er essensielt for en vellykket omstilling (til smidig / lean, DevOps e.l).

Transformasjonsledelse driver frem og forsterker effekten av de tekniske og organisatoriske praksisene som korrelerer med høy prestasjon (kontinuerlig leveranse, lean management osv). Det går ut på å jobbe sammen med teamene for å identifisere nødvendig endring, samt skape og presentere en visjon for hvordan komme i havn. 

**For å lykkes med omstilling, bør en leder**
- Være visjonær. Ha klare meninger om hvilken retning organisasjonen skal bevege seg, og hvor den skal være fem år frem i tid.
- Inspirere og motivere til engasjement for organisasjonens mål og visjoner.
- Gi intellektuell stimulans. Utfordre positivt. Oppfordre til nytenkning og å utfordre status quo.
- Være støttende. Bry seg om personlige behov og følelser.
- Gi personlig anerkjennelse. Legge merke til hva som oppnås og presteres, og gi personlig skryt når noen gjør noe bra.


**Mer overordnet må man**
- Utvikle riktig mindset gjennom å skape et miljø for læring.
- Utvikle egne coacher.
- Gjøre transformasjonen på sin egen måte
    - Man kan la seg inspirere og lære av andre, men man bør ikke kopiere det andre gjør. Eksperimentering og tilpassing etter hva som funker for sin organisasjon, er det riktige å gjøre.
    - Ikke sette ut transformasjonen (lean, smidig etc) til en ekstern partner. Teamene vil da føle at det blir gjort mot de. Evne til forbedring, tilpasning og utvikling av prosesser og metoder osv nås via å ha eierskap til transformasjonen.

---

## Bærekraftig arbeidsliv
Grad av utbrenthet og _deployment pain_ ble målt for å forsikre at høy rapportert leveranseprestasjon ikke ble oppnådd gjennom tvang og på bekostning av teamets mentale helse.

### Deployment pain
_Deployment pain_: Frykten man føler når kode dras ut i produksjon eller når en release skal installeres.

Der hvor _deployment pain_ er verst, finner man også den dårligste leveranseevnen, dårligst kultur og dårligst presterende organisasjon.

Microsoft: **Før Bing-teamet implementerte kontinuerlig leveranse, scoret de 38% på life/work balance blant de ansatte. Etterpå spratt det opp til 75%**.

De fleste deployment-problemer skjer på grunn av en krøkkete deployment-prosess med avhengigheter til en bestemt konfigurasjon osv. Sannsynligheten for feil i deploy / release _øker betraktelig_ når prosessen krever manuelle endringer.

Alt det som øker evnen til å levere kjapt og stabilt (kontinuerlig leveranse), reduserer stress og angst forbundet med deploy / release.

Vi bør derfor
- Sørge for enkel deploy til ulike miljøer.
- Bygge robuste systemer som kan detektere og tolerere feil i miljøer.
- Sørge for at komponenter kan oppdateres uavhengig av hverandre.
- Sørge for at alt, bortsett fra data, kan gjenopprettes fra versjonskontroll.

### Utbrenthet
Disse fem faktorene er sterkt forbundet med utbrenthet:

- Dårlig organisasjonskultur (maktorientert, frykt, tilbakeholding av informasjon, plassering av skyld osv).
- Deployment pain.
- Lite effektivt lederskap (teamet har for mange oppgaver samtidig, hindere fjernes ikke osv).
- Lite investering i og utvikling av ansatte.
- Dårlig kollektiv prestasjon (_organizational performance_).
