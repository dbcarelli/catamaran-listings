# catamaran-listings

Structured database of Daniel Beltri Carelli's used sailing-catamaran hunt.

## Criteria

- Daggerboard sailing cats (Outremer, Catana, Seawind daggerboard models, and others)
- Length ≥ 37 ft (prefer ~45 ft)
- Target under $500k; search up to $750k
- On or near US East or West Coast

## For apps (Grok / other)

| Path | Purpose |
|------|---------|
| `data/listings.json` | Active consolidated listings |
| `data/price_history.json` | Asking-price snapshots over time |
| `data/criteria.json` | Search rules |
| `data/rejected.json` | Boats Daniel rejected, with reasons |
| `schema/listing.schema.json` | JSON Schema for one listing |

Fetch raw JSON from GitHub, e.g.:

```
https://raw.githubusercontent.com/dbcarelli/catamaran-listings/main/data/listings.json
```

## Deduping

Match boats across sites by brand, model, year, location, price, and HIN when available. Prefer broker/YachtWorld prices when SailboatListings disagrees.
