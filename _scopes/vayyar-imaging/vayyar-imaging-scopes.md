---
authorization_urls:
- https://account.walabot.com/authentication/oauth/authorize
description: OAuth scopes published in the Walabot DIY storefront's OIDC discovery document (Shopify customer accounts on account.walabot.com), captured verbatim from scopes_supported. Vayyar publishes no OpenAPI and no first-party scope reference of its own; these are the only documented scopes on any Vayyar-operated host. Descriptions are from the Shopify customer-account platform semantics the discovery document points at.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Vayyar Imaging Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vayyar Imaging publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vayyar Imaging API on a user''s behalf.


  Tokens are issued from https://account.walabot.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vayyar Imaging
provider_slug: vayyar-imaging
schemes:
- flows:
  - authorizationUrl: https://account.walabot.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.walabot.com/authentication/oauth/token
  name: walabot-customer-account-oidc
  source: well-known/vayyar-imaging-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication (ID token issuance)
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address claim
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the walabot.com store
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API surface for the walabot.com store
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: vayyar-imaging-scopes
source_filename: vayyar-imaging-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://walabot.com/.well-known/openid-configuration\ndescription: >-\n  OAuth scopes published in the Walabot DIY storefront's OIDC discovery\n  document (Shopify customer accounts on account.walabot.com), captured\n  verbatim from scopes_supported. Vayyar publishes no OpenAPI and no\n  first-party scope reference of its own; these are the only documented\n  scopes on any Vayyar-operated host. Descriptions are from the Shopify\n  customer-account platform semantics the discovery document points at.\nschemes:\n  - name: walabot-customer-account-oidc\n    source: well-known/vayyar-imaging-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://account.walabot.com/authentication/oauth/authorize\n        tokenUrl: https://account.walabot.com/authentication/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication (ID token issuance)\n    flows: [authorizationCode]\n\
  \    sources: [well-known/vayyar-imaging-openid-configuration.json]\n  - scope: email\n    description: Access to the customer's email address claim\n    flows: [authorizationCode]\n    sources: [well-known/vayyar-imaging-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API for the walabot.com store\n    flows: [authorizationCode]\n    sources: [well-known/vayyar-imaging-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the customer-account MCP API surface for the walabot.com store\n    flows: [authorizationCode]\n    sources: [well-known/vayyar-imaging-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vayyar-imaging/refs/heads/main/scopes/vayyar-imaging-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Sensors
- Radar
- Imaging
- IoT
- Healthcare
- Elderly Care
- Automotive
- Smart Home
token_urls:
- https://account.walabot.com/authentication/oauth/token
---
