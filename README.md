# WaitCart Catalog

Public fictional product catalog for **WaitCart: Zero Shopping**.

## Live endpoints

- Manifest: https://vshia98.github.io/waitcart-catalog/manifest.json
- Current catalog: https://vshia98.github.io/waitcart-catalog/catalog-v2.json
- Previous catalog: https://vshia98.github.io/waitcart-catalog/catalog-v1.json

## Editing products

1. Copy the current catalog to a new versioned file, for example `catalog-v3.json`.
2. Increase the top-level `version` value.
3. Add or edit products while keeping every `id` unique.
4. Set `marketCodes` to ISO country codes such as `["JP", "KR"]`; omit it for globally available products.
5. Set `requiresPro` to `true` only for Pro catalog items.
6. Validate the JSON and calculate its SHA-256 checksum.
7. Update `manifest.json` last with the same version, the new Pages URL, and checksum.

The app ignores catalogs whose version is not newer, whose JSON is invalid, or whose SHA-256 does not match the manifest. Product listings, prices, merchants, inventory, reviews, and logistics are fictional; do not copy retailer listings or claim live popularity data.
