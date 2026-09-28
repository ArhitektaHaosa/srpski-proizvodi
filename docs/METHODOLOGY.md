# Methodology: what counts as a Serbian product

Last revised: 2026-09-28

## One sentence

A record enters the public catalogue when the **brand or the specific product was first created or first industrially produced on the territory of today's Serbia**, regardless of who owns the trademark today.

## Five fields that must stay separate

Never merge these into one cell.

1. **Brand origin** — where the brand name / identity was first established.
2. **Product origin** — where that SKU / recipe / industrial process was first developed or first produced.
3. **Place of production today** — only if a reliable current source exists.
4. **Current manufacturer**
5. **Current brand owner**

Example used as the editorial test case:

| Field | Bananica |
| --- | --- |
| Product origin | Beograd / Zemun area, then Yugoslavia |
| Year (company claim) | 1938 |
| Historical manufacturer | Štark line (Louit / La Cigogne / Soko-Nada Štark) |
| Current manufacturer / owner | Atlantic Štark / Atlantic Grupa (Zagreb group, plant in Serbia) |

Current ownership does not rewrite 1938.

## Inclusion

- Food, drink, confectionery, snacks, dairy, meat, spices, household, cosmetics, OTC brands with cultural weight
- Textile, footwear, tools, furniture, bicycles, appliances, industrial design
- Products of factories that no longer exist, if the factory stood on today's Serbian territory
- Discontinued products
- Brands that changed owner
- Modern products created in Serbia
- Licensed local production **only** with status `SERBIAN_PRODUCTION_ONLY` (example: Jaffa cakes — McVitie's concept 1927, Crvenka factory 1975/76)

## Exclusion

- Sold in Serbia ≠ Serbian
- Produced in Serbia today under a foreign brand ≠ Serbian origin
- Regional group portfolio item with origin in Croatia, Slovenia, BiH, North Macedonia, etc. stays `REGIONAL_BRAND` or `FORMER_YUGOSLAV_PRODUCT`
- Fructal, Cedevita, Cockta, Argeta, Donat, Barcaffè: do not list as Serbian origin without a product-level proof that *that SKU* was created in Serbia
- Weapons marketing. Prvi Partizan and historical Zastava industrial products may appear only as industrial-history records, never as a shop or promotion

## Source ladder (descending)

1. Official manufacturer / brand site
2. Archived official company materials (Internet Archive)
3. Intellectual Property Office of the Republic of Serbia
4. Business and historical registers
5. National Library of Serbia / digital collections
6. Museum and university collections
7. Specialist publications
8. Reliable media archives
9. Books and monographs
10. Internet Archive copies of old official sites

Wikipedia is a research door, not a dating authority.

Every important fact needs:

- `fact_text`
- `source_url`
- `source_type`
- `verified_at`
- `confidence` (`high` / `medium` / `low`)

## Confidence

- `high` — official company history or primary register / archive, independently consistent
- `medium` — serious secondary source, or official site without a primary scan
- `low` — press retelling, oral history, Wikipedia-only

A `low` fact never appears in the hero "quick facts" box.

## Editorial voice

Factual. Warm. Readable. No corporate slogan tone. No fake superlatives. No "more than just a candy" filler.

Good:

> Bananica se proizvodi od 1938. godine. Prepoznatljivi penasti slatkiš sa ukusom banane i čokoladnim prelivom postao je jedan od dugovečnijih proizvoda beogradske konditorske industrije.

Bad:

> Bananica is more than just a candy...

Do not invent ratings, reviews or prices for SEO.

## Image rights

A file on a brand media page is **not** a free licence.

Track for every image:

- source URL
- copyright status
- allowed use
- author if known
- licence
- attribution
- retrieved_at

Generated editorial art: `generated=1`, generator, generation_date, prompt_version.

Never mark a photo `free to use` without evidence.

## Growth model

Not "complete on day one".

`candidate` → `researching` → `fact_checked` → `published`  
plus `needs_review` and `draft`.

Target path: 100+ candidates → 300 → 500+, with verification status visible on the public page.
