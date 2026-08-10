---
authorization_urls:
- https://account.ekohealth.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Eko Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Eko Health publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Eko Health API on a user''s behalf.


  Tokens are issued from https://account.ekohealth.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Eko Health
provider_slug: eko-health
schemes:
- flows:
  - authorizationUrl: https://account.ekohealth.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.ekohealth.com/authentication/oauth/token
  name: shopify-customer-account-oidc
  source: well-known/eko-health-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Release the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the customer account API for the signed-in Eko Health customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API — the authenticated counterpart of the anonymous storefront MCP server at https://www.ekohealth.com/api/mcp.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: eko-health-scopes
source_filename: eko-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://www.ekohealth.com/.well-known/openid-configuration\nnotes: >-\n  Scopes taken verbatim from the scopes_supported array of the OAuth/OIDC discovery\n  document Eko Health serves at www.ekohealth.com. These govern the storefront customer\n  account and the customer-account MCP API. The Eko Connect API (api.ekodevices.com)\n  publishes no scope surface — no OAuth metadata is served on that host — so it is not\n  represented here. Descriptions below are the plain meaning of each scope name; Eko\n  publishes no scope reference page.\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/eko-health-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.ekohealth.com/authentication/oauth/authorize\n    tokenUrl: https://account.ekohealth.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope requesting\
  \ an ID token for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/eko-health-openid-configuration.json]\n- scope: email\n  description: Release the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/eko-health-openid-configuration.json]\n- scope: 'customer-account-api:full'\n  description: Full access to the customer account API for the signed-in Eko Health customer.\n  flows: [authorizationCode]\n  sources: [well-known/eko-health-openid-configuration.json]\n- scope: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the customer-account MCP API — the authenticated counterpart of the\n    anonymous storefront MCP server at https://www.ekohealth.com/api/mcp.\n  flows: [authorizationCode]\n  sources: [well-known/eko-health-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eko-health/refs/heads/main/scopes/eko-health-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Health
- Healthcare
- Medical Devices
- Digital Health
- Telehealth
- Artificial Intelligence
- Cardiology
- Remote Patient Monitoring
- Commerce
token_urls:
- https://account.ekohealth.com/authentication/oauth/token
---
