---
api_specs:
- filename: hometrack-authentication-api-openapi.yml
  format: yaml
  label: Hometrack Authentication API
  slug: hometrack-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-authentication-api-openapi.yml
- filename: hometrack-brands-api-openapi.yml
  format: yaml
  label: Hometrack Brands API
  slug: hometrack-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-brands-api-openapi.yml
- filename: hometrack-broker-api-openapi.yml
  format: yaml
  label: Hometrack Broker API
  slug: hometrack-broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-broker-api-openapi.yml
- filename: hometrack-epc-hometrack-api-openapi.yml
  format: yaml
  label: Hometrack Epc Hometrack API
  slug: hometrack-epc-hometrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-epc-hometrack-api-openapi.yml
- filename: hometrack-flood-twinn-api-openapi.yml
  format: yaml
  label: Hometrack Flood Twinn API
  slug: hometrack-flood-twinn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-flood-twinn-api-openapi.yml
- filename: hometrack-ground-coastalerosion-twinn-api-openapi.yml
  format: yaml
  label: Hometrack Ground Coastalerosion Twinn API
  slug: hometrack-ground-coastalerosion-twinn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-ground-coastalerosion-twinn-api-openapi.yml
- filename: hometrack-ground-subsidence-twinn-api-openapi.yml
  format: yaml
  label: Hometrack Ground Subsidence Twinn API
  slug: hometrack-ground-subsidence-twinn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-ground-subsidence-twinn-api-openapi.yml
- filename: hometrack-ground-terrafirma-api-openapi.yml
  format: yaml
  label: Hometrack Ground Terrafirma API
  slug: hometrack-ground-terrafirma-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-ground-terrafirma-api-openapi.yml
- filename: hometrack-internal-api-openapi.yml
  format: yaml
  label: Hometrack Internal API
  slug: hometrack-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-internal-api-openapi.yml
- filename: hometrack-licences-api-openapi.yml
  format: yaml
  label: Hometrack Licences API
  slug: hometrack-licences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-licences-api-openapi.yml
- filename: hometrack-organisation-api-openapi.yml
  format: yaml
  label: Hometrack Organisation API
  slug: hometrack-organisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-organisation-api-openapi.yml
- filename: hometrack-partners-api-openapi.yml
  format: yaml
  label: Hometrack Partners API
  slug: hometrack-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-partners-api-openapi.yml
- filename: hometrack-pvrplugin-api-openapi.yml
  format: yaml
  label: Hometrack Pvrplugin API
  slug: hometrack-pvrplugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-pvrplugin-api-openapi.yml
- filename: hometrack-reporting-api-openapi.yml
  format: yaml
  label: Hometrack Reporting API
  slug: hometrack-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-reporting-api-openapi.yml
- filename: hometrack-status-api-openapi.yml
  format: yaml
  label: Hometrack Status API
  slug: hometrack-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-status-api-openapi.yml
- filename: hometrack-trial-api-openapi.yml
  format: yaml
  label: Hometrack Trial API
  slug: hometrack-trial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-trial-api-openapi.yml
- filename: hometrack-valuation-api-openapi.yml
  format: yaml
  label: Hometrack Valuation API
  slug: hometrack-valuation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-valuation-api-openapi.yml
- filename: hometrack-zoopla-api-openapi.yml
  format: yaml
  label: Hometrack Zoopla API
  slug: hometrack-zoopla-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-zoopla-api-openapi.yml
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
