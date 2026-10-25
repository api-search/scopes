---
api_specs:
- filename: digi-key-barcoding-api-openapi.yml
  format: yaml
  label: Digi-Key Barcoding API
  slug: digi-key-barcoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-barcoding-api-openapi.yml
- filename: digi-key-bondedinventory-api-openapi.yml
  format: yaml
  label: Digi-Key Bonded Inventory API
  slug: digi-key-bondedinventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-bondedinventory-api-openapi.yml
- filename: digi-key-customerresource-api-openapi.yml
  format: yaml
  label: Digi-Key Customer Resource API
  slug: digi-key-customerresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-customerresource-api-openapi.yml
- filename: digi-key-lists-api-openapi.yml
  format: yaml
  label: Digi-Key Lists API
  slug: digi-key-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-lists-api-openapi.yml
- filename: digi-key-orderhistory-api-openapi.yml
  format: yaml
  label: Digi-Key Order History API
  slug: digi-key-orderhistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-orderhistory-api-openapi.yml
- filename: digi-key-ordermanagement-api-openapi.yml
  format: yaml
  label: Digi-Key Order Management API
  slug: digi-key-ordermanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-ordermanagement-api-openapi.yml
- filename: digi-key-orders-api-openapi.yml
  format: yaml
  label: Digi-Key Orders API
  slug: digi-key-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-orders-api-openapi.yml
- filename: digi-key-packlist-api-openapi.yml
  format: yaml
  label: Digi-Key Pack List API
  slug: digi-key-packlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-packlist-api-openapi.yml
- filename: digi-key-parts-api-openapi.yml
  format: yaml
  label: Digi-Key Parts API
  slug: digi-key-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-parts-api-openapi.yml
- filename: digi-key-pcn-api-openapi.yml
  format: yaml
  label: Digi-Key Pcn API
  slug: digi-key-pcn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-pcn-api-openapi.yml
- filename: digi-key-quotes-api-openapi.yml
  format: yaml
  label: Digi-Key Quotes API
  slug: digi-key-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-quotes-api-openapi.yml
- filename: digi-key-product-search-api-openapi.yml
  format: yaml
  label: Digi-Key Product Search API
  slug: digi-key-product-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-product-search-api-openapi.yml
authorization_urls:
- https://api.digikey.com/v1/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Digi Key Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Digi-Key publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Digi-Key API on a user''s behalf.


  Tokens are issued from https://api.digikey.com/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Digi-Key
provider_slug: digi-key
schemes:
- flows:
  - authorizationUrl: https://api.digikey.com/v1/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2AccessCodeSecurity
  source: openapi/digi-key-b2bapi-order-management-api-ordermanagement-v1-openapi.yml
- flows:
  - authorizationUrl: https://api.digikey.com/v1/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2AccessCodeSecurity
  source: openapi/digi-key-barcoding-barcoding-v3-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2ApplicationSecurity
  source: openapi/digi-key-customerresource-customerresource-v1-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2ApplicationSecurity
  source: openapi/digi-key-mylists-api-mylists-v1-openapi.yml
- flows:
  - authorizationUrl: https://api.digikey.com/v1/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2AccessCodeSecurity
  source: openapi/digi-key-ordering-api-v3-ordering-v3-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2ApplicationSecurity
  source: openapi/digi-key-orderstatus-orderstatus-v4-openapi.yml
- flows:
  - authorizationUrl: https://api.digikey.com/v1/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2AccessCodeSecurity
  source: openapi/digi-key-packinglist-api-packinglist-openapi.yml
- flows:
  - authorizationUrl: https://api.digikey.com/v1/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2AccessCodeSecurity
  source: openapi/digi-key-product-change-notifications-api-changenotifications-v3-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2ApplicationSecurity
  source: openapi/digi-key-productsearch-api-products-v4-openapi.yml
- flows:
  - authorizationUrl: https://api.digikey.com/v1/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2SecurityScheme
  source: openapi/digi-key-quote-api-quoting-v4-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.digikey.com/v1/oauth2/token
  name: oauth2ApplicationSecurity
  source: openapi/digi-key-supply-chain-api-supplychain-v1-openapi.yml
scope_count: 1
scope_names:
- Audience
scopes:
- description: developer.digikey.com HTTP Api
  flows:
  - authorizationCode
  scope: Audience
slug: digi-key-scopes
source_filename: digi-key-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/digi-key-b2bapi-order-management-api-ordermanagement-v1-openapi.yml, openapi/digi-key-barcoding-barcoding-v3-openapi.yml,\n  openapi/digi-key-customerresource-customerresource-v1-openapi.yml, openapi/digi-key-mylists-api-mylists-v1-openapi.yml,\n  openapi/digi-key-ordering-api-v3-ordering-v3-openapi.yml, openapi/digi-key-orderstatus-orderstatus-v4-openapi.yml,\n  openapi/digi-key-packinglist-api-packinglist-openapi.yml, openapi/digi-key-product-change-notifications-api-changenotifications-v3-openapi.yml,\n  openapi/digi-key-productsearch-api-products-v4-openapi.yml, openapi/digi-key-quote-api-quoting-v4-openapi.yml,\n  openapi/digi-key-supply-chain-api-supplychain-v1-openapi.yml\nschemes:\n- name: oauth2AccessCodeSecurity\n  source: openapi/digi-key-b2bapi-order-management-api-ordermanagement-v1-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.digikey.com/v1/oauth2/authorize\n   \
  \ tokenUrl: https://api.digikey.com/v1/oauth2/token\n- name: oauth2AccessCodeSecurity\n  source: openapi/digi-key-barcoding-barcoding-v3-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.digikey.com/v1/oauth2/authorize\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\n- name: oauth2ApplicationSecurity\n  source: openapi/digi-key-customerresource-customerresource-v1-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\n- name: oauth2ApplicationSecurity\n  source: openapi/digi-key-mylists-api-mylists-v1-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\n- name: oauth2AccessCodeSecurity\n  source: openapi/digi-key-ordering-api-v3-ordering-v3-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.digikey.com/v1/oauth2/authorize\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\n- name: oauth2ApplicationSecurity\n\
  \  source: openapi/digi-key-orderstatus-orderstatus-v4-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\n- name: oauth2AccessCodeSecurity\n  source: openapi/digi-key-packinglist-api-packinglist-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.digikey.com/v1/oauth2/authorize\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\n- name: oauth2AccessCodeSecurity\n  source: openapi/digi-key-product-change-notifications-api-changenotifications-v3-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.digikey.com/v1/oauth2/authorize\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\n- name: oauth2ApplicationSecurity\n  source: openapi/digi-key-productsearch-api-products-v4-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\n- name: oauth2SecurityScheme\n  source: openapi/digi-key-quote-api-quoting-v4-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.digikey.com/v1/oauth2/authorize\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\n- name: oauth2ApplicationSecurity\n  source: openapi/digi-key-supply-chain-api-supplychain-v1-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.digikey.com/v1/oauth2/token\nscopes:\n- scope: Audience\n  description: developer.digikey.com HTTP Api\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/digi-key-quote-api-quoting-v4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/scopes/digi-key-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Shopping
- Public APIs
- Electronic Components
- Distribution
- Ordering
- Product Search
- Pricing
- Inventory
- Supply Chain
token_bound: false
token_urls:
- https://api.digikey.com/v1/oauth2/token
---
