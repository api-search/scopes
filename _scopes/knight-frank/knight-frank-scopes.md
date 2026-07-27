---
api_specs:
- filename: knight-frank-api-v3-openapi.json
  format: json
  label: KnightFrank Api v3
  slug: knight-frank-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/openapi/knight-frank-api-v3-openapi.json
authorization_urls: []
description: 'The only OAuth surface Knight Frank operates is the Azure AD B2C tenant behind the consumer "My Knight Frank" account. It is not a developer authorization server: there is no scope reference page, no consent screen for third-party applications, and no way for an outside client to be registered against it. The discovery documents advertise `openid` only; the single resource scope below is read from the first-party web client''s public configuration, not from any published documentation. The anonymous corporate search API (api-v3) has no OAuth and therefore no scopes at all.'
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Knight Frank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Knight Frank publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Knight Frank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Knight Frank
provider_slug: knight-frank
schemes:
- flows:
  - flow: authorizationCode
  name: azure-ad-b2c
  source: authentication/knight-frank-authentication.yml
  type: openIdConnect
scope_count: 2
scope_names:
- openid
- https://KnightFrankB2Cprod.onmicrosoft.com/6e6a9034-3e20-4ec6-993f-61c89c0a2e2a/MyKf.ReadWrite
scopes:
- description: Standard OpenID Connect scope. The only value listed in `scopes_supported` in both harvested B2C discovery documents.
  flows:
  - authorizationCode
  scope: openid
- description: Read/write access to the signed-in consumer's own "My Knight Frank" data — saved properties, saved searches and property alerts on the api-v2 /secure surface. Requested by the first-party Angular client through MSAL. It is a resource scope on a custom B2C application, not a delegated developer scope, and it is not obtainable by a third-party application.
  flows:
  - authorizationCode
  scope: https://KnightFrankB2Cprod.onmicrosoft.com/6e6a9034-3e20-4ec6-993f-61c89c0a2e2a/MyKf.ReadWrite
slug: knight-frank-scopes
source_filename: knight-frank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  authentication/knight-frank-b2c-mykfsignin-openid-configuration.json and\n  authentication/knight-frank-b2clogin-mykfsignin-openid-configuration.json\n  (both harvested HTTP 200), plus the public client-side `kfsearchconfig.Azureb2c`\n  object in the HTML of\n  https://www.knightfrank.co.uk/properties/residential/for-sale/london.\ndescription: >-\n  The only OAuth surface Knight Frank operates is the Azure AD B2C tenant behind\n  the consumer \"My Knight Frank\" account. It is not a developer authorization\n  server: there is no scope reference page, no consent screen for third-party\n  applications, and no way for an outside client to be registered against it.\n  The discovery documents advertise `openid` only; the single resource scope\n  below is read from the first-party web client's public configuration, not from\n  any published documentation. The anonymous corporate search API (api-v3) has\n  no OAuth and therefore\
  \ no scopes at all.\ndocs: null\ndocs_note: >-\n  No scopes / permissions reference page exists. Knight Frank publishes no\n  developer documentation.\nauthorization_servers:\n  - name: KnightFrankB2Cprod (B2C_1A_MYKFSIGNIN)\n    issuer_metadata: authentication/knight-frank-b2c-mykfsignin-openid-configuration.json\n    authorization_endpoint_host: login.prd-knightfrank.com\n    alternate_host: knightfrankb2cprod.b2clogin.com\n    policy: B2C_1A_MYKFSIGNIN\n    tenant_id: ea15e386-0dbc-4a5b-ac74-08f50f444486\n    flows:\n      - flow: authorizationCode\nschemes:\n  - name: azure-ad-b2c\n    source: authentication/knight-frank-authentication.yml\n    type: openIdConnect\n    flows:\n      - flow: authorizationCode\nscopes:\n  - scope: openid\n    description: >-\n      Standard OpenID Connect scope. The only value listed in\n      `scopes_supported` in both harvested B2C discovery documents.\n    flows: [authorizationCode]\n    sources:\n      - authentication/knight-frank-b2c-mykfsignin-openid-configuration.json\n\
  \      - authentication/knight-frank-b2clogin-mykfsignin-openid-configuration.json\n  - scope: https://KnightFrankB2Cprod.onmicrosoft.com/6e6a9034-3e20-4ec6-993f-61c89c0a2e2a/MyKf.ReadWrite\n    short_name: MyKf.ReadWrite\n    description: >-\n      Read/write access to the signed-in consumer's own \"My Knight Frank\" data —\n      saved properties, saved searches and property alerts on the api-v2 /secure\n      surface. Requested by the first-party Angular client through MSAL. It is a\n      resource scope on a custom B2C application, not a delegated developer scope,\n      and it is not obtainable by a third-party application.\n    flows: [authorizationCode]\n    protected_resource: https://api-v2.web.prd-knightfrank.com/secure\n    sources:\n      - https://www.knightfrank.co.uk/properties/residential/for-sale/london\n      - review.yml (frontEndConfiguration.appBundle.protectedResourceMap)\nthird_party_access: false\nthird_party_access_note: >-\n  No client registration, no partner\
  \ programme, no published redirect-URI policy\n  and no application review process. The scopes above describe a first-party\n  consumer login only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/scopes/knight-frank-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Real Estate
- United Kingdom
- Property Listings
- Commercial Real Estate
- Valuation
- Brokerage
- Property Management
- Rentals
- PropTech
- Research
token_urls: []
---
