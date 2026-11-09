---
api_specs:
- filename: compsniper-com-account-api-openapi.yml
  format: yaml
  label: compsniper-com Account API
  slug: compsniper-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-account-api-openapi.yml
- filename: compsniper-com-best-offer-prices-api-openapi.yml
  format: yaml
  label: compsniper-com Best Offer Prices API
  slug: compsniper-com-best-offer-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-best-offer-prices-api-openapi.yml
- filename: compsniper-com-bulk-search-api-openapi.yml
  format: yaml
  label: compsniper-com Bulk Search API
  slug: compsniper-com-bulk-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-bulk-search-api-openapi.yml
- filename: compsniper-com-cards-api-openapi.yml
  format: yaml
  label: compsniper-com Cards API
  slug: compsniper-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-cards-api-openapi.yml
- filename: compsniper-com-depop-api-openapi.yml
  format: yaml
  label: compsniper-com Depop API
  slug: compsniper-com-depop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-depop-api-openapi.yml
- filename: compsniper-com-grailed-api-openapi.yml
  format: yaml
  label: compsniper-com Grailed API
  slug: compsniper-com-grailed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-grailed-api-openapi.yml
- filename: compsniper-com-mercari-api-openapi.yml
  format: yaml
  label: compsniper-com Mercari API
  slug: compsniper-com-mercari-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-mercari-api-openapi.yml
- filename: compsniper-com-poshmark-api-openapi.yml
  format: yaml
  label: compsniper-com Poshmark API
  slug: compsniper-com-poshmark-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-poshmark-api-openapi.yml
- filename: compsniper-com-psa-api-openapi.yml
  format: yaml
  label: compsniper-com PSA API
  slug: compsniper-com-psa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-psa-api-openapi.yml
- filename: compsniper-com-scrape-api-openapi.yml
  format: yaml
  label: compsniper-com Scrape API
  slug: compsniper-com-scrape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-scrape-api-openapi.yml
- filename: compsniper-com-shipping-rates-api-openapi.yml
  format: yaml
  label: compsniper-com Shipping Rates API
  slug: compsniper-com-shipping-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-shipping-rates-api-openapi.yml
- filename: compsniper-com-sold-history-api-openapi.yml
  format: yaml
  label: compsniper-com Sold history API
  slug: compsniper-com-sold-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-sold-history-api-openapi.yml
- filename: compsniper-com-summary-api-openapi.yml
  format: yaml
  label: compsniper-com Summary API
  slug: compsniper-com-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-summary-api-openapi.yml
- filename: compsniper-com-tcgplayer-api-openapi.yml
  format: yaml
  label: compsniper-com TC Gplayer API
  slug: compsniper-com-tcgplayer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compsniper-com/openapi/compsniper-com-tcgplayer-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Compsniper Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'compsniper-com publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the compsniper-com API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: compsniper-com
provider_slug: compsniper-com
schemes: []
scope_count: 4
scope_names:
- comps:read
- account:read
- jobs:write
- offline_access
scopes:
- description: Search and compare sold listings
  flows: []
  scope: comps:read
- description: Read plan and remaining quota
  flows: []
  scope: account:read
- description: Start and cancel Max Mode jobs when requested
  flows: []
  scope: jobs:write
- description: Refresh the approved connection
  flows: []
  scope: offline_access
slug: compsniper-com-scopes
source_filename: compsniper-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://compsniper.com/docs/authentication.md\nscopes:\n  - name: comps:read\n    description: Search and compare sold listings\n  - name: account:read\n    description: Read plan and remaining quota\n  - name: jobs:write\n    description: Start and cancel Max Mode jobs when requested\n  - name: offline_access\n    description: Refresh the approved connection"
source_yaml_url: https://artifacts.apis.io/compsniper-com/scopes/compsniper-com-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Marketplace
- E-Commerce
- Data
- Collectibles
token_bound: false
token_urls: []
---
