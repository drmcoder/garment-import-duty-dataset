# Garment import duty by origin and destination

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24444291.svg)](https://doi.org/10.5281/zenodo.24444291)

Import duty on three knitwear products, from five producing countries into ten markets, with the preference scheme and the official source for every row. Free to reuse under CC BY 4.0.

**Browse it online:** [trishaktiapparel.com/tools/duty-rates/](https://trishaktiapparel.com/tools/duty-rates/) · **Compare landed cost:** [duty comparison chart](https://trishaktiapparel.com/duty-comparison/)

## Coverage (version 2026-09-25)
- **Products:** cotton knit T-shirts (HS 6109.10), cotton knit polo shirts (HS 6105.10), cotton sweatshirts & hoodies (HS 6110.20)
- **Origins:** Nepal, Bangladesh, India, China, Vietnam
- **Destinations:** European Union, United Kingdom, United States, Canada, Japan, South Korea, Australia, China, India, United Arab Emirates
- **144 rows**, each checked against the official tariff source on 25–27 September 2026

## Files
- `data/garment-duty-rates.csv`: one row per destination × origin × product
- `data/garment-duty-rates.json`: the same rows with metadata (version, licence, citation) and structured source links

| Column | Meaning |
|---|---|
| `destination`, `destination_key` | Importing market |
| `duty_basis` | Value the duty is charged on (e.g. CIF, FOB) |
| `origin`, `origin_key` | Country where the garment is made |
| `product`, `hs_code` | Product and its HS code |
| `rate_percent` | Ad valorem duty rate in % |
| `scheme` | Tariff treatment applied (e.g. Everything But Arms, MFN) |
| `conditional` | `true` when the rate depends on meeting rules of origin or other conditions |
| `verified` | Date the row was checked |
| `source_urls` / `sources` | Official tariff source(s) for the row |

## Important
Rates change. Preferential rates apply only when the goods meet that scheme's rules of origin and the right proof of origin is provided. Taxes such as VAT, GST or IGST are not included. This dataset is not customs or legal advice: confirm your HS code and origin with a licensed customs broker. The live copy at <https://trishaktiapparel.com/data/garment-duty-rates.json> is updated when rates change.

## Licence and citation
Data: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Credit: *Trishakti Apparel, trishaktiapparel.com*. Please cite it: Trishakti Apparel (2026). *Garment import duty by origin and destination* [Dataset]. Zenodo. [doi:10.5281/zenodo.24444291](https://doi.org/10.5281/zenodo.24444291) (all versions; see `CITATION.cff`).

Made by [Trishakti Apparel](https://trishaktiapparel.com), a knitwear factory in Gaindakot, Nepal. Also part of our [open tools for knitwear buyers](https://github.com/SAHARA-Labs-Nepal/nepal-knitwear-sourcing-tools). Corrections welcome: open an issue.
