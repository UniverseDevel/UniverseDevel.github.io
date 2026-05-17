# Kinkred shop catalogue

`v1.json` is the affiliate shop catalogue the Kinkred app fetches from
`https://universedevel.github.io/kinkred/shop/v1.json`. Edit it to add, change,
or expire affiliate links — no app update is needed; the app picks up changes
within about a day. An empty `entries` array means the app shows no shop links.

## Format

```json
{
  "version": 1,
  "entries": [
    {
      "kinkId": "rope_bondage",
      "regions": ["GB", "US"],
      "shop": "Lovehoney",
      "label": "rope",
      "url": "https://www.lovehoney.co.uk/bondage/rope/?aff=YOURCODE",
      "validFrom": "2026-05-01",
      "validUntil": "2026-12-31"
    }
  ]
}
```

## Fields

- `kinkId` — the kink id exactly as defined in the app's catalogue
  (`KinkSeed.kt`). A kink may have several entries; they all appear together
  in that kink's shop popup.
- `regions` — ISO-3166 alpha-2 country codes, uppercase, that the entry
  serves. Use `["*"]` for all regions.
- `shop` — retailer name shown under the popup row (e.g. `Lovehoney`).
- `label` — short gear word used as the popup row title (e.g. `rope`,
  `plugs`, `wax candles`).
- `url` — the complete affiliate URL, with your affiliate code already
  embedded. Link to a category page, not a single product.
- `validFrom` / `validUntil` — inclusive ISO dates (`YYYY-MM-DD`). An entry is
  shown only while the device date falls inside this window, so a time-limited
  affiliate deal drops out on its own when it lapses.

Favour consumables (candles, etc.) over one-off purchases (cuffs) — repeat
purchases mean repeat commission.
