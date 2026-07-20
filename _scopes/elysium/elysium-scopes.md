---
authorization_urls:
- https://account.elysiumhealth.com/authentication/oauth/authorize
description: ''
docs: https://www.elysiumhealth.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Elysium Scopes
name_suffix: OAuth Scopes
note: Scopes are those advertised by the Shopify Customer Account authorization server for elysiumhealth.com. Elysium publishes no first-party developer OAuth program of its own.
overview: 'Elysium Health publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Elysium Health API on a user''s behalf.


  Tokens are issued from https://account.elysiumhealth.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elysium Health
provider_slug: elysium
schemes:
- flows:
  - authorizationUrl: https://account.elysiumhealth.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.elysiumhealth.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/26818117694
  name: ShopifyCustomerAccountOIDC
  source: well-known/elysium-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the authenticated customer.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer (orders, addresses, subscriptions, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API — the agent-facing customer surface, allowing an authorized agent to act on the customer's account.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: elysium-scopes
source_filename: elysium-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.elysiumhealth.com/.well-known/openid-configuration\ndocs: https://www.elysiumhealth.com/.well-known/openid-configuration\nnote: >-\n  Scopes are those advertised by the Shopify Customer Account authorization server for\n  elysiumhealth.com. Elysium publishes no first-party developer OAuth program of its own.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/elysium-openid-configuration.json\n  issuer: https://shopify.com/authentication/26818117694\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.elysiumhealth.com/authentication/oauth/authorize\n    tokenUrl: https://account.elysiumhealth.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token for the authenticated customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/elysium-openid-configuration.json\n- scope: email\n\
  \  description: Releases the customer's email address and email_verified claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/elysium-openid-configuration.json\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer\n    (orders, addresses, subscriptions, profile).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/elysium-openid-configuration.json\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API — the agent-facing customer\n    surface, allowing an authorized agent to act on the customer's account.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/elysium-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elysium/refs/heads/main/scopes/elysium-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Health
- Longevity
- Supplements
- Consumer Health
- Diagnostics
- Agentic Commerce
- Universal Commerce Protocol
- Shopify
- E-Commerce
- MCP
token_urls:
- https://account.elysiumhealth.com/authentication/oauth/token
---
