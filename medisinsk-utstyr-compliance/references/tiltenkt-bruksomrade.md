# Tiltenkt bruksområde og ytelsespåstander

## Hva er tiltenkt bruksområde?

MDR Art. 2(12) definerer **tiltenkt bruksområde** som den bruken et medisinsk utstyr er beregnet for, i henhold til opplysningene fra produsenten på merkingen, i bruksanvisningen, eller i reklame- eller salgsmateriell.

**Dette er den viktigste regelen for produktbeskrivelser:** Alt vi skriver på nettsiden må holde seg innenfor produsentens tiltenkte bruksområde.

## Hovedregel

> Produktbeskrivelsen på nettsiden MÅ samsvare med produsentens tiltenkte bruksområde. Ikke utvid, ikke omfortolk, ikke tilføy.

### Lovgrunnlag
- **MDR Art. 7(d)**: Forbudt å antyde bruk utover det tiltenkte bruksområdet som samsvarsvurderingen ble gjennomført for
- **MDR Art. 16(1)**: Hvis en distributør endrer tiltenkt bruksområde, kan distributøren anses som ny produsent — med alle forpliktelser det medfører

## Regler for produktbeskrivelser

### TILLATT
- Gjengi produsentens tiltenkte bruksområde direkte
- Oversette produsentens bruksområde til norsk (uten å endre betydning)
- Forenkle språket for forbrukerforståelse (uten å utvide omfanget)
- Gjengi ytelsesdata som produsenten selv oppgir

### FORBUDT
- Utvide bruksområdet utover det produsenten angir
- Antyde bruk for andre tilstander enn det utstyret er sertifisert for
- Legge til indikasjoner produsenten ikke har dokumentert
- Reposisjonere produktet for en annen pasientgruppe
- Skape inntrykk av at utstyret kan brukes til diagnostikk/behandling det ikke er godkjent for

## Eksempler

### Tiltenkt bruksområde: "Sårbandasje for mindre kutt og skrubbsår"

| Tekst | Vurdering | Begrunnelse |
|-------|-----------|-------------|
| "Beskytter mindre sår og skrubbsår" | COMPLIANT | Samsvarer med tiltenkt bruk |
| "Ideell for småsår i hverdagen" | COMPLIANT | Forenklet, men innenfor omfanget |
| "Fremskynder sårheling" | NON_COMPLIANT | Ytelsespåstand uten dekning — med mindre produsent dokumenterer dette |
| "Egnet for postoperative sår" | CRITICAL | Utvider til kirurgiske sår — utenfor tiltenkt bruk |
| "Forebygger infeksjon" | NON_COMPLIANT | Medisinsk påstand utenfor tiltenkt bruksområde (med mindre dokumentert) |

### Tiltenkt bruksområde: "Blodtrykksmåler for hjemmebruk"

| Tekst | Vurdering | Begrunnelse |
|-------|-----------|-------------|
| "Mål blodtrykket enkelt hjemme" | COMPLIANT | Direkte fra tiltenkt bruk |
| "Overvåk blodtrykket ditt mellom legebesøk" | COMPLIANT | Innenfor hjemmebruk |
| "Diagnostiser høyt blodtrykk" | CRITICAL | Diagnostisering er legens oppgave — utstyret måler, diagnostiserer ikke |
| "Klinisk nøyaktighet" | NEEDS_REVIEW | Kun tillatt hvis produsenten dokumenterer klinisk validering |

### Tiltenkt bruksområde: "Kompresjonsstrømpe, klasse 2, for behandling av venøs insuffisiens"

| Tekst | Vurdering | Begrunnelse |
|-------|-----------|-------------|
| "Kompresjonsstrømpe klasse 2 for venøs insuffisiens" | COMPLIANT | Gjengir tiltenkt bruk |
| "Lindrer tunge og hovne ben" | NEEDS_REVIEW | Symptombeskrivelse — akseptabelt hvis innenfor tiltenkt bruk |
| "Forebygger blodpropper" | CRITICAL | Utvider til tromboseprofylakse — annet bruksområde |
| "Helbreder åreknuter" | CRITICAL | Sykdomspåstand og utvidet bruksområde |

## Ytelsespåstander

### Hovedregel
Alle ytelsespåstander på nettsiden **må stamme fra produsentens dokumentasjon** (klinisk evaluering, ytelsesevaluering, samsvarserklæring).

### TILLATT
- Gjengi produsentens egne ytelsesdata (f.eks. "målenøyaktighet ±3 mmHg" hvis produsenten oppgir dette)
- Referere til kliniske studier som produsenten selv refererer til
- Bruke produsentens egne sammenligningsdata

### FORBUDT
- Oppfinne eller utbrodere ytelsespåstander
- Lage kvantitative påstander uten kilde i produsentdokumentasjonen (f.eks. "99% nøyaktighet")
- Sammenligne med andre produkter med mindre produsenten har dokumentert dette
- Bruke generelle effektpåstander uten spesifikk dekning ("den mest effektive", "best i test")

## Klassifikasjon i compliance-rapporten

| Funn | Type | Severity |
|------|------|----------|
| Bruksområde utvidet til ny indikasjon | `OFF_LABEL_BRUK` | CRITICAL |
| Bruksområde utvidet til ny pasientgruppe | `UTVIDET_BRUKSOMRADE` | CRITICAL |
| Antydning av diagnostisk evne utstyret ikke har | `OFF_LABEL_BRUK` | CRITICAL |
| Ytelsespåstand uten produsentdekning | `USPESIFISERT_YTELSE` | HIGH |
| Vag effektpåstand | `USPESIFISERT_YTELSE` | MEDIUM |
| Forenklet gjengivelse av tiltenkt bruk | — | COMPLIANT |
