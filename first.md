# Synopsis

<small>FællesOffentlig ReferenceArkitektur (FORA)?</small>

en opsummering af eksisterende referencearkitekturer med fornyet forkus på sikkerhed. Vægt på at beskrive eksisterende kendte mønstre, deres fordele og ulemper, samt hvilke områder det er vigtigt at standardisere/regulerer/aftale.

## Indledning

- Formål, anvendelse og målgruppe
- Scope
- Centrale begreber
- Tilblivelse og governance
- Anvendt metode, notation og signsturforklsring
- Releation til rammearkitektur og andre referencearkitekturer

## Juridiske rammer....
GDPR, NIS?, PSI og eIDAS.

Ridse de vigtigste principper op.

### Principper

- GDPR (lovlighed, rimeligehed og gennemsigtighed; formålsbegrænsning; dataminimering; rigtighed; opbevaringsbegrænsninger; integritet og fortrolighed; ansvarlighed)


- Der er forskel på persondata og ikke persondata.
- Data kan være kristiske og følsomme
- Sikkerhed og privacy

### Udvalgt bestemmelser/paragraffer

#### GDPR
Kun retlig forpligtigelse; samfunds interesse og myndighedsopgave er relevant for myndigheder. Vitale interesser?

Ved viderebehandling bør det vurderes: 4 + fornødne garantier ex kryptering og pseudonymisering (fra id-er, men stadig muligt ved sammenstilling

##### Den registrerede rettigheder
*Meddelelser*
Uden forsinkelse, maks en måned + to pga kompleksitet eller antal. Pligt til at angive klagemulighed. Gerne elektronisk. Overdrevne eller grundløse henvendelser kan der opkræve gebyr eller afvise (med bevisbyrde). Maskinlæsbare ikoner leveret eaf EU?

*Oplysning?*
På det tidspunkt hvor oplysninger indsamles. (sammenhæng og effektiv bør udpege portal løsning). 'Agter at viderebehandle'. Men hvis den registrede er bekendt med disse, bortfalder krav. Eller hvis det er udtrykkeligt fastsat i lov.

*Indsigt*
Bekræftigelse, indhold, vidergivelse, tidsrum, kilder (hvis ikke den registrede), automatiske afgørelser? Underretningspligt om garantier ved overførsel til 3land eller international org (15.1.a).

*Berigtigelse*
ingen unødig forsinkelse, ret til fuldstændiggørelse, 'fremlægge en supplerende erklæring'. Underretningspligt til dem som har fået data (hvis det ikke for svært). Ret til den registrede til at få at vide om underretningen er sket.

*Sletning?*
Undtagelse for retslig forpligtigelse. Undtagelse for arkivformål i samfundets interesse, vidensksbelige og historisk forskning og statistisk - under passende foranstaltninger.

*Begrænsning*
Bestride. Ved ulovlig behandling og den registrede modsætter sig sletning?. Forsvare retskrav. Under afvejning af legitime interesser. Krav om samtykke hvis de behandles udover opbevaring.

*Dataportabilitet*
Gælder ikke myndighedsudøvelse, men kan indgå i transmission fra ikke-myndighed. Ex fitbit.

*Indsigelse*
21.1 (profilering baseret på disse bestemmelser)  21.6 (den pågældendes særlige situation)

*Automatisering*
Ret til afgørelser ikke er alene baseret på automatisk behandling. Undtaget behandling er hjemlet i lov og hvis den registredes rettigheder beskyttes af passende foranstaltninger (list rettigheder! og beskriv krav til foranstaltninger)

##### Dataansvarlig og databehandlers forpligtigelser
*Ansvar*
Risici baseret... men den fysiske persons konsekvens.
Adfærdskodeks og certificering kan bruges til at påvise ansvarlighed

*By design and defaults*
Integration af de fornødne garantier. Mængde, behandling, periode og tilgængelig begrænses. Defaults skal sikre at data ikke stilles til rådighed til for et ubegrænset antal personer.

*Fælles dataansvar?*

*Databehandler*
Krav til at databehandler kan stille fornødne garantier for opfyldelse af GDPR krav og sikre beskyttelse. Ret til indsigelse mod ændringer i generelle aftaler. Krav til retsligt dokuments indhold (det må være her hunden ligger begravet i forhold til public gloud). Revision og inspektion. Databehandler skal underrette ansvarlig hvis instruks vurderes ulovlig. Standardbestemmelser fra kommissionen eller myndighed? Behandler må ikke fastlægge formål og hjælpemidler 28.10.

*Fortegnelse*
Både hos ansvarlig og behandler. Og kan rekvirers af tilsynsmyndighed. Kategorierne af registrede? 30.1.c. Er det muligt at beskrive sikkerhedsforanstaltninger? <250 personer (nok ikke for myndigheder)

##### Personoplysningssikkerhed
*Behandlingssikkerhed* pseudonymisering, kryptering. vedvarende informationssikerhed. genoprettelse. vurdering af foranstaltninger. Begrænsning af instruks.

*Anmeldelse til Tilsynsmyndighed* 72 timers frist efter brud på sikkerhed. Tilsynsmyndighed skal kunne kontrollere.

*Underetning til den registrede* Ingen forsinkelse, krav om forståelighed. Kontakt, sandsynlig konsekvens og dataansvarligs foranstaltninger. Undtagelse ved uforståelighed (kryptering), efterfølgende foranstalninger, offentlig meddelelse. Tilsynsmyndighed kan vurdere.




## Strategi

- Forretningsmæssige tendenser (regulering af datadeling GDPR, PSI mm)
- Teknologiske tendenser
- Vision:  ***Sammenhængende, sikker og effektiv*** Den fra FODS. (tillidsikring)

Beskriv at vi holder os til det tværgående, men at lokal risiko vurdering kan overse det fællesoffentlige. Derfor må vi også kigge på de lokale processer og tjenester der understøtter visionen.

- Forretningsmæssige mål
- Strategiske principper
- Værdiskabelse
- Sikkerhed?
- Rauls model

## Forretningsarkitektur
- Opgaver, aktører, roller og ansvar
- Tværgående processer.
- Forretningsfunktioner
- Tjenester og Forretningsobjekter.

(tillidstjenester og basisregistre findes i hver af nedenstående)

### Brugerstyring
Borger/Virksomheder (Controlled -> Federated)
Ansatte i myndigheder (Normativt -> Federated)

### Selvbetjening
Normative -> Controlled (særligt mit overblik/tværgående brugeroplevelser)
          -> Subsidiary (Kommuner vil selv)
          -> Federated (Regioner)

### Deling af data og dokumenter
Normativt -> Controlled (persondata og grunddata)
          -> Normativ (PSI)

### Forvaltning af Services, Application og Data
(Subsidiary -> Normative)


## Teknik
- Foretrukne Implementeringsmønstre for hver af de ovenstående funktioner
- Områder for standardisering og identificerede standarder
