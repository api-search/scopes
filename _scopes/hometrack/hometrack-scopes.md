---
api_specs:
- filename: hometrack-broker-avm-api-openapi.yml
  format: yaml
  label: Hometrack Broker AVM API
  slug: hometrack-broker-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-broker-avm-api-openapi.yml
- filename: hometrack-climate-graphql-api-openapi.yml
  format: yaml
  label: Hometrack Climate GraphQL API
  slug: hometrack-climate-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-climate-graphql-api-openapi.yml
- filename: hometrack-api-public-openapi.yml
  format: yaml
  label: Hometrack API Public
  slug: hometrack-api-public-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-api-public-openapi.yml
- filename: hometrack-climate-api-v2-openapi.yml
  format: yaml
  label: Hometrack Climate API (v2)
  slug: hometrack-climate-api-v2-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-climate-api-v2-openapi.yml
- filename: hometrack-prh-core-external-client-api-v2-openapi.yml
  format: yaml
  label: Hometrack (PRH) - Core External Client API v2.0
  slug: hometrack-prh-core-external-client-api-v2-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-prh-core-external-client-api-v2-openapi.yml
- filename: hometrack-valuation-api-v1-openapi.yml
  format: yaml
  label: Hometrack Valuation API
  slug: hometrack-valuation-api-v1-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-valuation-api-v1-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.hometrack.com/api-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Hometrack Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hometrack publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hometrack API on a user''s behalf.


  Tokens are issued from https://hometrack-prod.eu.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hometrack
provider_slug: hometrack
schemes:
- flows:
  - audience: https://api.hometrack.com
    flow: clientCredentials
    tokenUrl: https://hometrack-prod.eu.auth0.com/oauth/token
  name: OAuth2ClientCredentials
  provider: Auth0
  source: https://developer.hometrack.com/api-authentication
scope_count: 2
scope_names:
- read:valuations
- write:valuations
scopes:
- description: Read access to valuations. Named verbatim in the token-response example on Hometrack's API authentication page; no separate scope reference documents what it covers.
  flows:
  - clientCredentials
  scope: read:valuations
- description: Write access to valuations (ordering / instructing a valuation). Named verbatim in the same token-response example.
  flows:
  - clientCredentials
  scope: write:valuations
slug: hometrack-scopes
source_filename: hometrack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\ndocs: https://developer.hometrack.com/api-authentication\nsource: >-\n  https://developer.hometrack.com/api-authentication (worked token-response\n  example) + well-known/hometrack-auth0-openid-configuration.json.\nsummary: >-\n  Hometrack documents OAuth 2.0 client credentials but publishes no scope\n  reference page. The only scopes visible anywhere on its public surface are the\n  two shown in the worked token-response example on the authentication page:\n  read:valuations and write:valuations. No harvested OpenAPI declares an oauth2\n  security scheme, so nothing further can be derived — the running derivation\n  (0-working/derive-oauth-scopes.py) correctly returns zero. Any additional\n  scopes (climate, PRH case management, reporting) exist only inside the\n  commercial agreement and are not published.\nschemes:\n- name: OAuth2ClientCredentials\n  source: https://developer.hometrack.com/api-authentication\n  provider: Auth0\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://hometrack-prod.eu.auth0.com/oauth/token\n    audience: https://api.hometrack.com\nscopes:\n- scope: read:valuations\n  description: >-\n    Read access to valuations. Named verbatim in the token-response example on\n    Hometrack's API authentication page; no separate scope reference documents\n    what it covers.\n  flows: [clientCredentials]\n  sources: [https://developer.hometrack.com/api-authentication]\n- scope: write:valuations\n  description: >-\n    Write access to valuations (ordering / instructing a valuation). Named\n    verbatim in the same token-response example.\n  flows: [clientCredentials]\n  sources: [https://developer.hometrack.com/api-authentication]\nscope_reference_page: null\nidp_scopes_supported:\n  source: well-known/hometrack-auth0-openid-configuration.json\n  note: >-\n    The Auth0 tenant's scopes_supported list (openid, profile, offline_access,\n    name, given_name, family_name, nickname, email,\
  \ email_verified, picture,\n    created_at, identities, phone, address) is the standard OIDC user-profile\n    set advertised by every Auth0 tenant. It is NOT Hometrack's API permission\n    model and is recorded here only so it is not mistaken for one.\ngaps:\n- No published scope-to-operation mapping.\n- No scopes documented for the Climate, PRH Core External Client, Broker AVM or Public APIs.\n- OpenAPI documents declare only APIM subscription-key schemes, so scopes cannot be derived from the specs.\ncross_links:\n  authentication: authentication/hometrack-authentication.yml\n  well_known: well-known/hometrack-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/scopes/hometrack-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Real-Estate
- United Kingdom
- PropTech
- Valuation
- AVM
- Mortgage
- Property Data
- Climate Risk
- Lending
- Surveying
token_urls:
- https://hometrack-prod.eu.auth0.com/oauth/token
---
