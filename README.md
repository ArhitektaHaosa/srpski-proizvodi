# Srpski proizvodi

Independent documentary catalogue of products and brands **originating in Serbia**.

> Products we remember. Brands that became part of the culture.  
> Proizvodi koje pamtimo. Brendovi koji su postali deo kulture.

This is **not** a shop, **not** a corporate site, and **not** affiliated with manufacturers, trademark owners or distributors.

Hero line (planned site):

- SR: *Proizvedeno ovde. Zapamćeno svuda.*
- EN: *Made here. Remembered everywhere.*

## Rule that holds the project

**Serbian product ≠ current owner of the company.**

Bananica (1938, Beograd / then Yugoslavia), Smoki (1972), Najlepše želje stay in the catalogue because of origin and history. Current portfolio ownership is a separate field.

Atlantic Grupa is one source, not the taxonomy. Their public brand list mixes:

- brands historically created in Serbia
- brands created elsewhere in the region
- distributed third-party brands

Those three must never collapse into one column.

## Phase status (2026-09-28)

1. Taxonomy — drafted (`docs/TAXONOMY.md`)
2. Origin methodology — drafted (`docs/METHODOLOGY.md`)
3. Seed dataset — 169 research-queue rows / 100+ distinct candidates (`data/candidates.csv`)
4. SQL schema — drafted (`schema/001_init.sql`)
5. PHP application — **not started** (CloudPanel / PHP / MariaDB, same family as `yu-idiom`)
6. First article Bananica SR+EN — outline only (`content/bananica.md`)
7. Hero-art prompt for Bananica — drafted (`content/bananica-hero-prompt.md`)

No record is published as fact until origin is sourced. Wikipedia is a starting point, never the only proof for a dating or origin claim.

## Origin status codes (database)

| Code | Public wording (SR) | Public wording (EN) |
| --- | --- | --- |
| `CONFIRMED_SERBIAN_ORIGIN` | potvrđeno poreklo u Srbiji | confirmed origin in Serbia |
| `LIKELY_SERBIAN_ORIGIN` | verovatno poreklo u Srbiji | likely origin in Serbia |
| `SERBIAN_PRODUCTION_ONLY` | proizvedeno u Srbiji, koncept nastao drugde | produced in Serbia; concept originated elsewhere |
| `FORMER_YUGOSLAV_PRODUCT` | proizvod SFRJ / Kraljevine, poreklo van današnje Srbije ili još nije razdvojeno | Yugoslav-era product; origin outside today's Serbia or still being split |
| `REGIONAL_BRAND` | regionalni brend, nije srpsko poreklo | regional brand, not Serbian origin |
| `ORIGIN_UNCONFIRMED` | poreklo nije potvrđeno | origin unconfirmed |

Never display an uncertain date or city as a fact.

## Stack (planned, not built)

CloudPanel · Debian · Nginx · PHP 8.4 · MariaDB · PDO · Composer · `.env` outside web root · server-side rendering.

No WordPress. Same operational family as [yu-idiom](https://github.com/ArhitektaHaosa/yu-idiom).

## Disclaimer

SR: Ovo je nezavisan dokumentarni projekat posvećen istoriji proizvoda i brendova nastalih u Srbiji. Projekat nije povezan sa prikazanim proizvođačima, vlasnicima robnih marki ili distributerima. Nazivi i žigovi pripadaju njihovim vlasnicima.

EN: This is an independent documentary project dedicated to the history of products and brands originating in Serbia. It is not affiliated with the manufacturers, trademark owners or distributors shown on this website. Brand names and trademarks remain the property of their respective owners.

## License of this repository

Code: MIT (when PHP lands).  
Editorial text in this repo: CC BY 4.0 unless a file says otherwise.  
Brand names, logos, pack shots: **not** licensed by this project. Track each image in `licenses`.
