---
authorization_urls:
- https://shopify.com/authentication/7887683702/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Modifyhealth Scopes
name_suffix: OAuth Scopes
note: Read verbatim from scopes_supported in the OIDC discovery document served on ModifyHealth's own host. The authorization server is Shopify's customer-account issuer for shop 7887683702; ModifyHealth publishes no scope reference page of its own, so there is no richer docs source to upgrade this from.
overview: 'ModifyHealth publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ModifyHealth API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/7887683702/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ModifyHealth
provider_slug: modifyhealth
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/7887683702/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/7887683702/oauth/token
  name: shopify-customer-account-oauth2
  source: well-known/modifyhealth-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issues an id_token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for this shop - the authenticated buyer's orders, addresses, subscriptions and profile.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the buyer-scoped Customer Account MCP API. This is the authenticated counterpart to the anonymous UCP commerce MCP endpoint, and is what an agent would need to act on a signed-in customer's own account rather than on a fresh cart.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: modifyhealth-scopes
source_filename: modifyhealth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://modifyhealth.com/.well-known/openid-configuration\nnote: >-\n  Read verbatim from scopes_supported in the OIDC discovery document served on\n  ModifyHealth's own host. The authorization server is Shopify's customer-account issuer\n  for shop 7887683702; ModifyHealth publishes no scope reference page of its own, so\n  there is no richer docs source to upgrade this from.\nschemes:\n- name: shopify-customer-account-oauth2\n  source: well-known/modifyhealth-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/7887683702/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/7887683702/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an id_token identifying the customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/modifyhealth-openid-configuration.json\n- scope: email\n  description:\
  \ Access to the customer's email address and email_verified claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/modifyhealth-openid-configuration.json\n- scope: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API for this shop - the authenticated\n    buyer's orders, addresses, subscriptions and profile.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/modifyhealth-openid-configuration.json\n- scope: customer-account-mcp-api:full\n  description: >-\n    Full access to the buyer-scoped Customer Account MCP API. This is the authenticated\n    counterpart to the anonymous UCP commerce MCP endpoint, and is what an agent would\n    need to act on a signed-in customer's own account rather than on a fresh cart.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/modifyhealth-openid-configuration.json\nscope_count: 4\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modifyhealth/refs/heads/main/scopes/modifyhealth-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Health
- Food and Beverage
- Nutrition
- Meal Delivery
- Food as Medicine
- eCommerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Direct to Consumer
token_urls:
- https://shopify.com/authentication/7887683702/oauth/token
---
