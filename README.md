# WaitCart Catalog

Public source-attributed product reference catalog for **WaitCart: Zero Shopping**.

## Live endpoints

- Manifest: https://vshia98.github.io/waitcart-catalog/manifest.json
- Current catalog: https://vshia98.github.io/waitcart-catalog/catalog-v3.json
- Previous catalog: https://vshia98.github.io/waitcart-catalog/catalog-v2.json
- Legacy catalog: https://vshia98.github.io/waitcart-catalog/catalog-v1.json
- Image attribution: https://vshia98.github.io/waitcart-catalog/ATTRIBUTION-v3.md

## v3 scope

- 690 distinct product records and 690 verified HTTPS product images
- 22 country storefronts
- 30 shared products plus 30 country-observed products per storefront
- Product data from Open Food Facts, Open Beauty Facts, Open Products Facts, and Open Pet Food Facts under ODbL 1.0
- Product images from Open Facts contributors under CC BY-SA 3.0
- Marketplace ranking and category pages are dated demand signals only; no retailer image is copied or rehosted
- Prices, merchants, inventory, reviews, orders, and logistics remain simulated; no retailer or brand affiliation is claimed

## Editing

1. Run `node scripts/build-real-catalog.mjs` in the WaitCart app project.
2. Validate every product ID, source URL, license field, and image response.
3. Upload the new versioned catalog and matching attribution document.
4. Update this README to describe the active catalog.
5. Update `manifest.json` last with the same version, GitHub Pages URL, and SHA-256 checksum.

The app ignores catalogs whose version is not newer, whose JSON is invalid, or whose SHA-256 does not match the manifest.
