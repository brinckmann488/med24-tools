# Obligatorisk produktinformasjon på nettside

## Oversikt

Når medisinsk utstyr selges online (fjernssalg), gjelder alle MDR-krav fullt ut — ingen lettere regime for netthandel (MDR Art. 6). Denne sjekklisten dekker informasjon som MÅ eller BØR være på produktsiden.

## Standardelementer på med24.no (skal IKKE sjekkes)

Følgende er alltid til stede som standard plattformkomponenter og skal ikke rapporteres som manglende:

- **CE-merke med forklaringstekst** — vises automatisk i høyre sidebar på alle medisinsk utstyr-produktsider. Teksten forklarer at CE-merket betyr at produktet oppfyller EUs krav til sikkerhet, helse og miljø.
- **Virksomhetsinformasjon** — Med24 Apotek AS med org.nr. og kontaktinfo i footer
- **Språk** — plattformen er på norsk
- **Leveringsinformasjon** — alltid synlig i sidebar

Disse er **ikke synlige** via API/MCP tools da de renderes dynamisk av shoppens frontend.

## Lovpålagt informasjon (CRITICAL hvis mangler)

### 1. Tiltenkt bruksområde
- **Krav**: Produktsiden må tydelig angi hva utstyret er beregnet for
- **Kilde**: MDR Art. 7(d), Art. 2(12)
- **Sjekk**: Samsvarer teksten med produsentens tiltenkte bruksområde?

### 2. Produsentinformasjon
- **Krav**: Produsentens navn og adresse skal fremgå
- **Kilde**: MDR Art. 10(11), Art. 14(2)
- **Sjekk**: Er produsent identifisert med navn?

### 3. Språk
- **Krav**: Produktinformasjon skal være tilgjengelig på norsk
- **Kilde**: Forskrift om medisinsk utstyr §6, MDR Art. 10(11)
- **Sjekk**: Er relevant produktinformasjon på norsk (ikke kun engelsk)?

### 4. Risikoinformasjon
- **Krav**: Sannsynlige risikoer ved tiltenkt bruk må ikke utelates
- **Kilde**: MDR Art. 7(c)
- **Sjekk**: Er vesentlige advarsler/kontraindikasjoner fra bruksanvisningen gjengitt?

## Anbefalt informasjon (LOW hvis mangler)

### 5. CE-merke referanse
- **Status**: DEKKET AV PLATTFORM — CE-merke med forklaringstekst vises automatisk i sidebar
- **Kilde**: MDR Art. 14(2)(a)
- **Sjekk**: Ikke nødvendig — håndteres av shoppens standard produktside-layout

### 6. Risikoklasse
- **Krav**: Ikke lovpålagt å vise på nettside, men anbefalt for transparens
- **Kilde**: —
- **Sjekk**: Er risikoklassen angitt (Klasse I, IIa, IIb, III)?

### 7. UDI (Unique Device Identifier)
- **Krav**: Ikke lovpålagt for distributør å vise på nettside, men forbedrer sporbarhet
- **Kilde**: MDR Art. 14(2)(d)
- **Sjekk**: Er UDI-DI tilgjengelig?

### 8. Importørinformasjon
- **Krav**: Hvis produktet er importert (utenfor EØS), bør importørens kontaktinfo fremgå
- **Kilde**: MDR Art. 13(3), Art. 14(2)(d)
- **Sjekk**: Er importør identifisert (hvis relevant)?

### 9. Bruksanvisning-tilgjengelighet
- **Krav**: Bruksanvisningen (IFU) skal følge produktet — anbefalt å gjøre tilgjengelig digitalt
- **Kilde**: MDR Art. 10(11)
- **Sjekk**: Er bruksanvisning tilgjengelig eller referert til?

## Apotekspesifikke krav (Med24 Apotek)

### 10. Saklig medisinsk informasjon
- **Krav**: Produktinformasjon skal være utarbeidet i samsvar med gjeldende reklameregler og ha pålitelig, forsvarlig innhold
- **Kilde**: Apotekforskriften §46
- **Sjekk**: Er informasjonen saklig og faglig forsvarlig?

### 11. Prismarkedsføring
- **Krav**: Priser skal ikke presenteres slik at de fremmer impulskjøp
- **Kilde**: Apotekforskriften §49
- **Sjekk**: Er prispresentasjonen nøktern?

## Sjekkliste for compliance-rapport

```
LOVPÅLAGT (severity: HIGH/CRITICAL hvis mangler):
[ ] Tiltenkt bruksområde angitt og korrekt
[ ] Produsentinformasjon tilgjengelig
[ ] Risikoinformasjon ikke utelatt

DEKKET AV PLATTFORM (skal IKKE sjekkes):
[x] CE-merke med forklaringstekst (automatisk i sidebar)
[x] Virksomhetsinformasjon (footer)
[x] Produktinformasjon på norsk (plattformspråk)

ANBEFALT (severity: LOW hvis mangler):
[ ] Risikoklasse angitt
[ ] UDI tilgjengelig
[ ] Importørinformasjon (hvis relevant)
[ ] Bruksanvisning tilgjengelig/referert

APOTEKKRAV (severity: MEDIUM hvis brudd):
[ ] Saklig og faglig forsvarlig informasjon
[ ] Nøktern prispresentasjon
```

## Klassifikasjon i compliance-rapporten

| Funn | Type | Severity |
|------|------|----------|
| Tiltenkt bruksområde mangler | `MANGLENDE_OBLIGATORISK_INFO` | HIGH |
| Tiltenkt bruksområde feil/utvidet | `UTVIDET_BRUKSOMRADE` | CRITICAL |
| Produsentinfo mangler | `MANGLENDE_OBLIGATORISK_INFO` | MEDIUM |
| Ikke på norsk | `MANGLENDE_OBLIGATORISK_INFO` | HIGH |
| Risikoinformasjon utelatt | `MANGLENDE_RISIKOINFO` | CRITICAL |
| CE-merke ikke referert | `MANGLENDE_OBLIGATORISK_INFO` | LOW |
| Risikoklasse mangler | `MANGLENDE_OBLIGATORISK_INFO` | LOW |
| Uforsvarlig prisinformasjon | `VILLEDENDE_MARKEDSFORING` | MEDIUM |

## Spesielle hensyn for IVD-utstyr (In Vitro Diagnostikk)

For selvtester (f.eks. graviditetstester, blodsukkermålere) gjelder IVDR 2017/746 med parallelle bestemmelser. Ekstra krav:
- Tydelig angi at utstyret er en **selvtest** beregnet for hjemmebruk
- Angi at resultater **kan kreve bekreftelse av helsepersonell**
- Ikke antyd at selvtesten erstatter klinisk diagnostikk
