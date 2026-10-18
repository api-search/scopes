---
api_specs:
- filename: brink-commerce-custom-api-openapi.yml
  format: yaml
  label: Brink Commerce Custom API
  slug: brink-commerce-custom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/brink-commerce-custom-api-openapi.yml
- filename: brink-commerce-deliveries-api-openapi.yml
  format: yaml
  label: Brink Commerce Deliveries API
  slug: brink-commerce-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/brink-commerce-deliveries-api-openapi.yml
- filename: brink-commerce-orders-api-openapi.yml
  format: yaml
  label: Brink Commerce Orders API
  slug: brink-commerce-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/brink-commerce-orders-api-openapi.yml
- filename: brink-commerce-products-api-openapi.yml
  format: yaml
  label: Brink Commerce Products API
  slug: brink-commerce-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/brink-commerce-products-api-openapi.yml
- filename: brink-commerce-technical-api-openapi.yml
  format: yaml
  label: Brink Commerce Technical API
  slug: brink-commerce-technical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/openapi/brink-commerce-technical-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Brink Commerce Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Brink Commerce publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Brink Commerce API on a user''s behalf.


  Tokens are issued from /oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Brink Commerce
provider_slug: brink-commerce
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: OAuth2
  source: openapi/brink-commerce-openapi-generated.yml
scope_count: 4
scope_names:
- product-management/addon:read
- product-management/addon:write
- product-management/product:read
- product-management/product:write
scopes:
- description: ''
  flows:
  - clientCredentials
  scope: product-management/addon:read
- description: ''
  flows:
  - clientCredentials
  scope: product-management/addon:write
- description: ''
  flows:
  - clientCredentials
  scope: product-management/product:read
- description: ''
  flows:
  - clientCredentials
  scope: product-management/product:write
slug: brink-commerce-scopes
source_filename: brink-commerce-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: derived\nsource: openapi/brink-commerce-openapi-generated.yml\nschemes:\n- name: OAuth2\n  source: openapi/brink-commerce-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\nscopes:\n- scope: product-management/addon:read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brink-commerce-openapi-generated.yml\n- scope: product-management/addon:write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brink-commerce-openapi-generated.yml\n- scope: product-management/product:read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brink-commerce-openapi-generated.yml\n- scope: product-management/product:write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/brink-commerce-openapi-generated.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brink-commerce/refs/heads/main/scopes/brink-commerce-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- E-Commerce
- Platform
- Enterprise
- Composable
token_bound: false
token_urls:
- /oauth2/token
---
