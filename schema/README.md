Draft MariaDB schema is in the working copy as `schema/001_init.sql`.

Tables planned: categories, locations, companies, brands, products, product_categories, brand_owners, manufacturers, factories, product_history, brand_history, sources, facts, fact_sources, images, licenses, translations, aliases, tags, product_tags, related_products, candidate_products, users.

`facts` + `fact_sources` keep one URL per claim. Origin status lives on both brands and products and is never inferred from current_owner_id.
