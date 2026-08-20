---
api_specs:
- filename: corelogic-au-rp-inside-auth-example.postman_collection.json
  format: json
  label: CoreLogic Australia Access API
  slug: corelogic-au-access-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-rp-inside-auth-example.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Property Details API
  slug: corelogic-au-property-details-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Property Services API
  slug: corelogic-au-property-services-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Search API
  slug: corelogic-au-search-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia AVM API
  slug: corelogic-au-avm-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Auction API
  slug: corelogic-au-auction-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Statistics API
  slug: corelogic-au-statistics-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Charts API
  slug: corelogic-au-charts-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Property Timeline API
  slug: corelogic-au-property-timeline-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Content API
  slug: corelogic-au-content-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
authorization_urls:
- https://auth.corelogic.asia/as/authorization.oauth2
description: ''
docs: https://developer.corelogic.asia/guides/api-authentication
flows:
- authorizationCode
- clientCredentials
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Corelogic Au Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CoreLogic Australia publishes 5 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CoreLogic Australia API on a user''s behalf.


  Tokens are issued from https://auth.corelogic.asia/as/token.oauth2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CoreLogic Australia
provider_slug: corelogic-au
schemes:
- applies_to: developer portal human login
  flows:
  - authorizationUrl: https://auth.corelogic.asia/as/authorization.oauth2
    flow: authorizationCode
    tokenUrl: https://auth.corelogic.asia/as/token.oauth2
  - flow: clientCredentials
    tokenUrl: https://auth.corelogic.asia/as/token.oauth2
  - authorizationUrl: https://auth.corelogic.asia/as/authorization.oauth2
    flow: implicit
  issuer: https://auth.corelogic.asia
  name: CotalityDeveloperPortalOIDC
  source: well-known/corelogic-au-openid-configuration.json
scope_count: 5
scope_names:
- openid
- profile
- email
- phone
- address
scopes:
- description: OpenID Connect base scope. The only scope observed in Cotality's own published data-API token requests (client_credentials against access.api.cotality.com.au).
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: openid
- description: Standard OIDC profile claims for the portal user.
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Standard OIDC email claim for the portal user.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Standard OIDC phone claim for the portal user.
  flows:
  - authorizationCode
  - implicit
  scope: phone
- description: Standard OIDC address claim for the portal user.
  flows:
  - authorizationCode
  - implicit
  scope: address
slug: corelogic-au-scopes
source_filename: corelogic-au-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://auth.corelogic.asia/.well-known/openid-configuration\ndocs: https://developer.corelogic.asia/guides/api-authentication\nfinding: >-\n  CoreLogic Australia has NO data-product OAuth scope surface. The only scopes published anywhere\n  on the estate are the five PingFederate identity scopes advertised by the developer-portal\n  identity provider, which govern human login to the portal — not access to property, valuation,\n  auction or statistics data. The vendor's own published sample client_credentials token requests\n  carry scope \"openid\" and nothing else; entitlement to data products is carried in JWT claims\n  (roles, geo_codes, authorities) provisioned against a signed commercial licence, so a developer\n  cannot request finer-grained access by asking for a scope. This is the recorded model, not an\n  absence of research.\nauthorization_model: claims-based (roles / geo_codes / authorities in the JWT), not scope-based\n\
  schemes:\n- name: CotalityDeveloperPortalOIDC\n  source: well-known/corelogic-au-openid-configuration.json\n  issuer: https://auth.corelogic.asia\n  applies_to: developer portal human login\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.corelogic.asia/as/authorization.oauth2\n    tokenUrl: https://auth.corelogic.asia/as/token.oauth2\n  - flow: clientCredentials\n    tokenUrl: https://auth.corelogic.asia/as/token.oauth2\n  - flow: implicit\n    authorizationUrl: https://auth.corelogic.asia/as/authorization.oauth2\nscopes:\n- scope: openid\n  description: >-\n    OpenID Connect base scope. The only scope observed in Cotality's own published data-API token\n    requests (client_credentials against access.api.cotality.com.au).\n  flows: [authorizationCode, clientCredentials, implicit]\n  sources: [well-known/corelogic-au-openid-configuration.json]\n- scope: profile\n  description: Standard OIDC profile claims for the portal user.\n  flows: [authorizationCode, implicit]\n\
  \  sources: [well-known/corelogic-au-openid-configuration.json]\n- scope: email\n  description: Standard OIDC email claim for the portal user.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/corelogic-au-openid-configuration.json]\n- scope: phone\n  description: Standard OIDC phone claim for the portal user.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/corelogic-au-openid-configuration.json]\n- scope: address\n  description: Standard OIDC address claim for the portal user.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/corelogic-au-openid-configuration.json]\ngrant_types_supported:\n- implicit\n- authorization_code\n- refresh_token\n- password\n- client_credentials\n- urn:pingidentity.com:oauth2:grant_type:validate_bearer\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- urn:ietf:params:oauth:grant-type:saml2-bearer\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:openid:params:grant-type:ciba\n\
  data_api_grant_types_documented: [client_credentials, authorization_code, refresh_token]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/scopes/corelogic-au-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials/implicit
tags:
- Real-Estate
- Australia
- Property Data
- Valuation
- AVM
- PropTech
- Property Listings
- Rentals
- Auction Data
- Commercial Real Estate
- Mortgage
- Land Registry
- Cotality
- RP Data
token_urls:
- https://auth.corelogic.asia/as/token.oauth2
---
