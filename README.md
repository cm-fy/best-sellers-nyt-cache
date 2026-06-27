# Best-Sellers NYT Cache

Static cached New York Times bestseller list data, updated weekly via GitHub Actions.

## Data format

- `nyt/overview.json` — full overview response from the NYT Books API
- `nyt/meta.json` — lightweight metadata (list slugs, display names, update frequency)
- `nyt/{slug}.json` — individual list data (e.g. `hardcover-fiction.json`)

## Usage

Raw GitHub Pages URL pattern:

```
https://raw.githubusercontent.com/cm-fy/best-sellers-nyt-cache/main/nyt/{slug}.json
```

Or via GitHub Pages (once enabled):

```
https://cm-fy.github.io/best-sellers-nyt-cache/{slug}.json
```

## Data freshness

Lists are fetched every Thursday at 00:30 UTC (shortly after NYT publishes new lists Wednesday ~7pm ET).
Manual triggers are also available via the Actions tab.
