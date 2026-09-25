---
api_specs:
- filename: open-food-facts-api-v2-openapi.yml
  format: yaml
  label: Open Food Facts API v2
  slug: open-food-facts-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-api-v2-openapi.yml
- filename: open-food-facts-api-v3-openapi.yml
  format: yaml
  label: Open Food Facts API v3
  slug: open-food-facts-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-api-v3-openapi.yml
- filename: open-food-facts-open-prices-openapi.yml
  format: yaml
  label: Open Prices API
  slug: open-food-facts-open-prices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-open-prices-openapi.yml
- filename: open-food-facts-search-a-licious-openapi.json
  format: json
  label: Search-a-licious API
  slug: open-food-facts-search-a-licious
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-search-a-licious-openapi.json
- filename: open-food-facts-folksonomy-openapi.json
  format: json
  label: Folksonomy Engine API
  slug: open-food-facts-folksonomy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-folksonomy-openapi.json
- filename: open-food-facts-facets-knowledge-panels-openapi.json
  format: json
  label: Facets Knowledge Panels API
  slug: open-food-facts-facets-knowledge-panels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-facets-knowledge-panels-openapi.json
- filename: open-food-facts-nutripatrol-openapi.json
  format: json
  label: NutriPatrol API
  slug: open-food-facts-nutripatrol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-nutripatrol-openapi.json
- filename: open-food-facts-cgi-api-openapi.yml
  format: yaml
  label: Open Food Facts Cgi API
  slug: open-food-facts-cgi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-cgi-api-openapi.yml
- filename: open-food-facts-product-api-openapi.yml
  format: yaml
  label: Open Food Facts Product API
  slug: open-food-facts-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-product-api-openapi.yml
- filename: open-food-facts-search-api-openapi.yml
  format: yaml
  label: Open Food Facts Search API
  slug: open-food-facts-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-search-api-openapi.yml
- filename: open-food-facts-taxonomy-api-openapi.yml
  format: yaml
  label: Open Food Facts Taxonomy API
  slug: open-food-facts-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-taxonomy-api-openapi.yml
- filename: open-food-facts-taxonomy-suggestions-api-openapi.yml
  format: yaml
  label: Open Food Facts Taxonomy Suggestions API
  slug: open-food-facts-taxonomy-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-taxonomy-suggestions-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Open Food Facts Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Open Food Facts uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from auth.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Open Food Facts
provider_slug: open-food-facts
schemes:
- flows:
  - flow: password
    tokenUrl: auth
  name: OAuth2PasswordBearer
  source: openapi/open-food-facts-folksonomy-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: open-food-facts-scopes
source_filename: open-food-facts-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: derived\nsource: openapi/open-food-facts-folksonomy-openapi.json\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/open-food-facts-folksonomy-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: auth\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/scopes/open-food-facts-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Food
- Nutrition
- Open Data
- Product Data
- Barcodes
- Taxonomy
- Prices
- Search
- Food and Beverage
token_urls:
- auth
---
