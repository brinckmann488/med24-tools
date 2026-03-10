# Botanicals "on hold" i EU-regulering

## Juridisk baggrund

Siden 2012 har EU-Kommissionen sat vurderingen af sundhedsanprisninger for plantebaserede stoffer (botanicals) "on hold". Det betyder at EFSA ikke har afsluttet sin videnskabelige vurdering af disse claims.

### Status-kategorier for sundhedsanprisninger

| Status | Betydning | Compliance-klassifikation |
|--------|-----------|--------------------------|
| **Godkendt** | EFSA har vurderet og godkendt anprisningen | COMPLIANT |
| **Afvist** | EFSA har vurderet og afvist anprisningen | NON_COMPLIANT (HIGH) |
| **On hold** | EFSA har IKKE afsluttet vurderingen | NEEDS_REVIEW (LOW) |

**Vigtigt**: "On hold" betyder hverken godkendt eller afvist. Anprisningerne er stadig indsendt og afventer vurdering. De fleste EU-lande, inkl. Danmark, tillader forsat brug af on-hold claims under forudsætning af at de ikke er vildledende.

## Compliance-klassifikation

Botanicals on-hold klassificeres som:

```json
{
  "type": "BOTANICAL_ON_HOLD",
  "severity": "LOW",
  "status": "NEEDS_REVIEW"
}
```

Dette adskiller sig fra:
- **Afviste claims** → `NON_COMPLIANT`, severity `HIGH`
- **Sygdomsanprisninger** → `NON_COMPLIANT`, severity `CRITICAL`
- **Godkendte claims** → `COMPLIANT`

## Almindelige on-hold botanicals

### Eksempler med typiske claims

| Botanical | Typisk claim | Status |
|-----------|-------------|--------|
| Ginkgo biloba | Hukommelse og kognitiv funktion | On hold |
| Valeriane (Valeriana officinalis) | Søvn og afslapning | On hold |
| Echinacea | Immunforsvar | On hold |
| Kurkuma (Curcuma longa) | Ledfunktion, inflammation | On hold |
| Ginseng (Panax ginseng) | Energi og vitalitet | On hold |
| Hvidløg (Allium sativum) | Hjerte-kar, kolesterol | On hold |
| Artiskok (Cynara scolymus) | Fordøjelse, leverfunktion | On hold |
| Grøn te (Camellia sinensis) | Antioxidant, metabolisme | On hold |
| Tranebær (Vaccinium macrocarpon) | Urinveje | On hold |
| Ingefær (Zingiber officinale) | Fordøjelse, kvalme | On hold |
| Salvie (Salvia officinalis) | Overgangsalder, kognition | On hold |
| Passionsblomst (Passiflora incarnata) | Afslapning, søvn | On hold |

### Bemærk: Guarana (koffein)

Guarana-claims relateret til koffeinindhold er IKKE on hold — koffein har godkendte claims. Kun guarana-specifikke claims ud over koffein er on hold.

## Hvad er tilladt med on-hold botanicals

### Tilladt
- Brug af on-hold claims i markedsføring (med forbehold)
- Henvisning til botanicalens traditionelle brug
- Faktuelle ingrediensbeskrivelser

### IKKE tilladt (uanset on-hold status)
- Sygdomsanprisninger ("forebygger diabetes", "kurerer gigt")
- Vildledende overdrivelser ("mirakelkur", "vidundermiddel")
- Claims der er specifikt AFVIST af EFSA
- Uspecifikke sundhedsanprisninger uden kobling til on-hold claim

## Dynamisk datakilde

On-hold-listen opdateres løbende. Den autoritative kilde for Med24 er:

**SharePoint Knowledge Bank** → indeholder den aktuelle liste over godkendte, afviste og on-hold claims fra EU Health Claims-registeret, filtreret per ingrediens.

Den automatiserede compliance-checker (n8n workflow `YZQ3vFdVtp9WhKMH`) slår op i Knowledge Bank for at klassificere claims korrekt baseret på produktets specifikke ingredienser.
