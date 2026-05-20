<h1 align="center">Ready APIs</h1>

<p align="center">
  <strong>Curated, normalized data for products and AI agents.</strong><br>
  200+ APIs across address, tax, weather, FX, fraud, compliance - one key, one bill, <a href="https://readyapis.com/mcp/connect">MCP-ready</a>.
</p>

<p align="center">
  <a href="https://readyapis.com">readyapis.com</a> ·
  <a href="https://readyapis.com/docs/getting-started">Docs</a> ·
  <a href="https://readyapis.com/pricing">Pricing</a> ·
  <a href="https://readyapis.com/blog">Blog</a>
</p>

---

## Client libraries

Both open-source under MIT, with OIDC/sigstore provenance on PyPI and npm.

### Python SDK - [`readyapis-python`](https://github.com/ReadyAPIs-com/readyapis-python)

[![PyPI](https://img.shields.io/pypi/v/readyapis.svg)](https://pypi.org/project/readyapis/)
[![Python](https://img.shields.io/pypi/pyversions/readyapis.svg)](https://pypi.org/project/readyapis/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/ReadyAPIs-com/readyapis-python/blob/main/LICENSE)

```bash
pip install readyapis
```

```python
from readyapis import Client
client = Client()                        # reads READYAPIS_API_KEY from env
zip_data = client.geo.zip("30301")
print(zip_data.city, zip_data.state)     # "Atlanta" "GA"
```

### Node CLI - [`readyapis-node`](https://github.com/ReadyAPIs-com/readyapis-node)

[![npm](https://img.shields.io/npm/v/readyapis.svg)](https://www.npmjs.com/package/readyapis)
[![Node](https://img.shields.io/node/v/readyapis.svg)](https://www.npmjs.com/package/readyapis)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/ReadyAPIs-com/readyapis-node/blob/main/LICENSE)

One command to scaffold a runnable demo - pick from `geo`, `tax`, `fx`, `email`, `calendar`, or `intel`, plus a target language (Node, Python, or curl). Zero runtime dependencies; resolves in under a second.

```bash
npx readyapis init        # interactive - drops one file in your cwd
npx readyapis whoami      # verify your key
```

## Curated open datasets

When you don't need the live API - just clean source data in a CSV.

### [`curated-us-zips`](https://github.com/ReadyAPIs-com/curated-us-zips)

[![Rows](https://img.shields.io/badge/rows-33%2C100-informational.svg)](https://github.com/ReadyAPIs-com/curated-us-zips#whats-in-the-csv)
[![License](https://img.shields.io/badge/data%20license-CC%20BY%204.0-blue.svg)](https://github.com/ReadyAPIs-com/curated-us-zips#license)

33,100 U.S. ZIP codes with city, state, county, lat/lng, timezone, metro area, and U.S. Census ACS demographic enrichment. One CSV, 3 MB, CC BY 4.0.

```bash
curl -L -o us-zips.csv https://raw.githubusercontent.com/ReadyAPIs-com/curated-us-zips/main/data/us-zips.csv
```

For the live API surface (per-request lookup, batch validation, cross-checks), see [Location Enrichment](https://readyapis.com/apis/location-enrichment).

---

## What lives on readyapis.com

The site has everything that isn't a code distribution:

- [**Catalog**](https://readyapis.com/apis) - every endpoint with live examples
- [**Docs**](https://readyapis.com/docs/getting-started) - quickstart, auth, error envelope, rate limits
- [**Recipes**](https://readyapis.com/recipes) - step-by-step how-tos for real product problems
- [**Free tools**](https://readyapis.com/free/address-validator) - try without signup
- [**MCP setup**](https://readyapis.com/mcp/connect) - connect Claude or Cursor in one click
- [**Pricing**](https://readyapis.com/pricing) - free tier, no card

## Contact

- **Email**: [support@readyapis.com](mailto:support@readyapis.com)
- **Bugs in these libraries**: file an issue on the relevant repo above
