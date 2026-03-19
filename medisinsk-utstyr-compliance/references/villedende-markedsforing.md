# Villedende markedsføring for medisinsk utstyr

## Regulatorisk grunnlag

Markedsføring av medisinsk utstyr i Norge reguleres av:

1. **MDR Art. 7** — Forbud mot villedende påstander (EU-forordning, direkte gjeldende)
2. **Markedsføringsloven** — Generell norsk markedsføringslov (Forbrukertilsynet)
3. **DMP-retningslinjer** — All reklame skal være objektiv, sannferdig og saklig
4. **Apotekforskriften §46** — Pålitelig, forsvarlig medisinsk informasjon

## DMP-krav til reklame

DMP (Direktoratet for medisinske produkter) stiller følgende krav:

- All reklame for medisinsk utstyr skal være **objektiv, sannferdig og gi saklig informasjon**
- Reklame skal alltid **samsvare med produsentens bruksanvisning** hva gjelder formål, korrekt bruk og forsiktighetsregler
- Reklame for medisinsk utstyr er tillatt rettet mot både helsepersonell og allmennheten
- DMP overvåker reklame aktivt og har **sanksjonsmuligheter** (overtredelsesgebyr, tvangsmulkt)

## Kategorier av villedende markedsføring

### 1. Superlativer og absolutte påstander
**Severity: HIGH**

Udokumenterte superlativer og absolutte påstander er villedende.

| Forbudt | Tillatt alternativ |
|---------|-------------------|
| "Det beste blodtrykksmåleren" | "Blodtrykksmåler med [spesifikk funksjon]" |
| "Markedsledende nøyaktighet" | "Målenøyaktighet ±3 mmHg (iht. produsentdata)" |
| "100% sikker å bruke" | "Designet for sikker hjemmebruk" |
| "Ingen bivirkninger" | Angi faktiske advarsler fra bruksanvisningen |
| "Revolusjonerende teknologi" | Beskriv teknologien konkret |
| "Mirakelprodukt" | Aldri tillatt |

### 2. Falsk autoritet
**Severity: HIGH**

| Forbudt | Tillatt alternativ |
|---------|-------------------|
| "Anbefalt av leger" (udokumentert) | "CE-merket medisinsk utstyr" |
| "Godkjent av DMP" (feilaktig — DMP godkjenner ikke utstyr) | "I samsvar med EU-forordningen for medisinsk utstyr" |
| "Forskningsbasert" (uten referanse) | "Klinisk evaluert iht. MDR" (hvis korrekt) |
| Legebilder/hvite frakker uten reelt grunnlag | Fjern autoritetsbilder |
| "Brukt på norske sykehus" (udokumentert) | Kun hvis verifiserbart |

**Viktig:** CE-merking er IKKE en godkjenning fra DMP eller noen myndighet. CE-merking betyr at produsenten erklærer samsvar. Formuleringer som "godkjent av myndigheter" er villedende.

### 3. Misvisende bilder og illustrasjoner
**Severity: HIGH**

MDR Art. 7 dekker også **bilder og figurative tegn**. Bilder på produktsiden kan villede.

| Forbudt | Begrunnelse |
|---------|-------------|
| Bilde som viser klinisk bruk når utstyret er for hjemmebruk | Antyder profesjonell bruk/nøyaktighet |
| Bilde som viser bruk på tilstand utenfor tiltenkt bruk | Visuell off-label antydning |
| "Før/etter"-bilder som impliserer behandlingseffekt utstyret ikke har | Falskt inntrykk av effekt |
| Overdrevent profesjonelle/kliniske omgivelser | Kan gi falskt inntrykk av utstyrets klasse |

### 4. Pris- og kampanjevilledning
**Severity: MEDIUM**

| Forbudt | Begrunnelse |
|---------|-------------|
| "Tilbud — kjøp nå!" på medisinsk utstyr | Apotekforskriften §49: Ikke fremme impulskjøp |
| Aggressiv nedtelling/hastemarkering | Kan presse til uoverveid kjøp av helseutstyr |
| "Kjøp 3, betal for 2" uten medisinsk begrunnelse | Kan fremme unødig forbruk |

### 5. Utelatt eller nedtonet risikoinformasjon
**Severity: CRITICAL**

| Forbudt | Begrunnelse |
|---------|-------------|
| Utelate kontraindikasjoner fra bruksanvisningen | MDR Art. 7(c) |
| Bagatellisere nødvendig opplæring | Kan føre til feilbruk |
| Skjule at resultat krever profesjonell tolkning | Villeder om utstyrets begrensninger |
| "Passer for alle" når kontraindikasjoner finnes | Direkte villedende |

### 6. Testimonials og brukeranmeldelser
**Severity: MEDIUM**

| Risikosone | Begrunnelse |
|------------|-------------|
| Brukeranmeldelser som inneholder sykdomspåstander | Kan utgjøre ulovlig helsepåstand |
| Testimonials som antyder effekt utover tiltenkt bruk | Off-label antydning |
| "Reddet livet mitt" / sterke personlige påstander | Kan skape falskt inntrykk av effekt |
| Selektiv publisering av kun positive anmeldelser | Kan være villedende i kontekst |

**Anbefaling:** Brukeranmeldelser bør modereres for å fjerne ulovlige helsepåstander.

## Trygge formuleringer

### Generelle produktbeskrivelser
- "CE-merket medisinsk utstyr"
- "Tiltenkt bruksområde: [gjengi produsentens tekst]"
- "[Produktnavn] er beregnet for [tiltenkt bruk]"
- "Les bruksanvisningen nøye før bruk"
- "Kontakt lege hvis du er usikker på om produktet passer for deg"

### Egenskapsbeskrivelser (innenfor produsentdokumentasjon)
- "Med [spesifikk funksjon] for enkel hjemmebruk"
- "Måleområde: [spesifikt område iht. produsent]"
- "Kompatibel med [spesifikt tilbehør]"
- "Vekt: X g, dimensjoner: X cm" (fysiske fakta)

### Anbefalte standardtekster
- "Dette er et CE-merket medisinsk utstyr. Les bruksanvisningen før bruk."
- "Ved tvil, kontakt lege eller apotek."
- "Produktinformasjonen er basert på produsentens dokumentasjon."

## Klassifikasjon i compliance-rapporten

| Funn | Type | Severity |
|------|------|----------|
| Udokumentert superlativ | `VILLEDENDE_MARKEDSFORING` | HIGH |
| Falsk autoritetspåstand | `VILLEDENDE_MARKEDSFORING` | HIGH |
| Villedende bilde/illustrasjon | `VILLEDENDE_MARKEDSFORING` | HIGH |
| Utelatt risikoinformasjon | `MANGLENDE_RISIKOINFO` | CRITICAL |
| Impulskjøp-fremmende pris | `VILLEDENDE_MARKEDSFORING` | MEDIUM |
| Problematisk testimonial | `VILLEDENDE_MARKEDSFORING` | MEDIUM |
| Generelt misvisende formulering | `VILLEDENDE_MARKEDSFORING` | MEDIUM |
