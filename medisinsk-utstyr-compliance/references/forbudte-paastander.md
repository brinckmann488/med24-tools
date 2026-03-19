# Forbudte påstander for medisinsk utstyr (MDR Art. 7)

## Hovedregel — MDR Artikkel 7

I merking, bruksanvisning, tilgjengeliggjøring, ibruktaking og **reklame** for medisinsk utstyr er det **forbudt** å bruke tekst, navn, varemerker, bilder og andre tegn som kan villede brukeren eller pasienten med hensyn til utstyrets tiltenkte formål, sikkerhet og ytelse.

## De fire forbudene (Art. 7 a-d)

### (a) Tilskrive egenskaper utstyret ikke har
**Severity: CRITICAL**

Forbudt å påstå at utstyret har funksjoner eller egenskaper det faktisk ikke har.

**Eksempler:**
- "Antibakteriell" (bandasje uten dokumentert antibakteriell effekt)
- "Smertelindrende" (støttebandage uten dokumentert smertelindrende effekt)
- "Temperaturregulerende" (uten dokumentasjon)
- "Allergivennlig" (uten dokumentert hypoallergenisitet)

### (b) Skape falskt inntrykk av behandling/diagnose
**Severity: CRITICAL**

Forbudt å skape falskt inntrykk av at behandling eller diagnose med utstyret vil lykkes, eller at utstyret har funksjoner det mangler.

**Eksempler:**
- "Garantert resultat" / "Garantert effekt"
- "Helbreder [tilstand]"
- "Kurerer [sykdom]"
- "Diagnostiserer pålitelig [sykdom]" (for hjemmeutstyr beregnet på screening, ikke diagnostikk)
- "Du slipper å gå til legen" (impliserer at utstyret erstatter medisinsk vurdering)

### (c) Unnlate å informere om risiko
**Severity: CRITICAL**

Forbudt å unnlate å informere brukeren om en sannsynlig risiko forbundet med bruk i henhold til tiltenkt bruksområde.

**Eksempler på utelatt risikoinformasjon:**
- Utelate kontraindikasjoner (f.eks. at kompresjonsstrømper ikke skal brukes ved alvorlig perifer arteriell sykdom)
- Utelate advarsler fra bruksanvisningen (f.eks. "Ikke bruk på skadet hud")
- Skjule at utstyret krever opplæring
- Utelate at måleresultater krever legevurdering for diagnose

### (d) Antyde bruk utenfor tiltenkt bruksområde
**Severity: CRITICAL**

Forbudt å antyde bruk utover det tiltenkte bruksområdet samsvarsvurderingen ble gjennomført for.

**Eksempler:**
- Bandasje sertifisert for "mindre sår" markedsført for "alle typer sår"
- Blodsukkermåler for "egenkontroll" markedsført som "klinisk diagnostikkverktøy"
- Termometer for "kroppstemperatur" markedsført for "overvåking av fertilitetsvindu" (annet formål)
- Støttebandasje markedsført for "rehabilitering etter operasjon" uten at dette er tiltenkt bruk

## Andre forbudte formuleringer

### Superlativer og absolutte påstander
**Severity: HIGH**

| Forbudt | Begrunnelse |
|---------|-------------|
| "Det beste produktet" | Udokumentert superlativ |
| "Markedsledende" | Udokumentert komparativ påstand |
| "100% sikker" | Intet medisinsk utstyr er 100% sikkert |
| "Ingen bivirkninger" | Villeder om risiko (Art. 7c) |
| "Mirakel-" / "Revolusjonerende" | Udokumentert og villedende |
| "Anbefalt av leger" | Kun tillatt med dokumentasjon for spesifikk anbefaling |
| "Klinisk bevist" | Kun tillatt med referanse til spesifikk klinisk evaluering |

### Sykdomspåstander (ulovlig utvidelse av bruksområde)
**Severity: CRITICAL**

Medisinsk utstyr har et definert tiltenkt bruksområde. Påstander om sykdom er bare tillatt innenfor dette.

| Forbudt (med mindre del av tiltenkt bruk) | Begrunnelse |
|-------------------------------------------|-------------|
| "Forebygger [sykdom]" | Utvidet bruksområde |
| "Behandler [sykdom]" | Utvidet bruksområde |
| "Kurerer [tilstand]" | Absolutt påstand + utvidet bruksområde |
| "Reduserer risiko for [sykdom]" | Medisinsk påstand utenfor de fleste utstyrs tiltenkte bruk |

**Viktig unntak:** Noen medisinsk utstyr HAR sykdomsrelatert tiltenkt bruksområde (f.eks. "kompresjonsstrømpe for behandling av venøs insuffisiens"). Da er sykdomsreferansen tillatt — men KUN innenfor det dokumenterte bruksområdet.

### Uautoriserte sammenligninger
**Severity: HIGH**

| Forbudt | Begrunnelse |
|---------|-------------|
| "Bedre enn [konkurrent]" | Kun tillatt med produsentens komparative data |
| "Mest nøyaktig på markedet" | Udokumentert komparativ |
| "Overlegen teknologi" | Vag og udokumentert |
| "Foretrukket av fagfolk" | Kun med dokumentasjon |

### Falsk autoritet
**Severity: HIGH**

| Forbudt | Begrunnelse |
|---------|-------------|
| "Legeranbefalt" (uten dokumentasjon) | Falsk autoritetspåstand |
| "Godkjent av [helsemyndighet]" (feilaktig) | CE-merking ≠ godkjenning fra DMP |
| Bruk av legebilder/hvite frakker i markedsføring uten reelt grunnlag | Villedende autoritet |
| "Forskningsbasert" (uten å referere til spesifikk forskning) | Vag autoritetspåstand |

## Grensetilfeller (NEEDS_REVIEW)

Disse krever faglig vurdering:

| Tekst | Vurdering | Begrunnelse |
|-------|-----------|-------------|
| "Kan bidra til bedre komfort" | NEEDS_REVIEW | Vagt — avhenger av produsentens claims |
| "Populær blant idrettsutøvere" | NEEDS_REVIEW | Kan implisere ytelsesegenskaper |
| "Brukt på sykehus" | NEEDS_REVIEW | Kan oppfattes som autoritetsargument — verifiser om korrekt |
| "Lett å bruke" | LOW | Generelt ufarlig, men sjekk at det ikke bagatelliserer nødvendig opplæring |

## Klassifikasjon i compliance-rapporten

| Funn | Type | Severity |
|------|------|----------|
| Tilskriver egenskaper utstyret ikke har | `ULOVLIG_PASTAND` | CRITICAL |
| Falskt inntrykk av behandling/diagnose | `ULOVLIG_PASTAND` | CRITICAL |
| Utelatt risikoinformasjon | `MANGLENDE_RISIKOINFO` | CRITICAL |
| Off-label bruksforslag | `OFF_LABEL_BRUK` | CRITICAL |
| Udokumentert superlativ/komparativ | `VILLEDENDE_MARKEDSFORING` | HIGH |
| Falsk autoritetspåstand | `VILLEDENDE_MARKEDSFORING` | HIGH |
| Vag effektpåstand | `USPESIFISERT_YTELSE` | MEDIUM |
| Grensetilfelle som krever fagvurdering | — | NEEDS_REVIEW |
