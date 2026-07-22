---
authorization_urls: []
description: ''
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Nara Organics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nara Organics publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nara Organics API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nara Organics
provider_slug: nara-organics
schemes:
- authorizationUrl: https://account.nara.com/authentication/oauth/authorize
  name: ShopifyCustomerAccountOIDC
  source: well-known/nara-organics-openid-configuration.json
  tokenUrl: https://account.nara.com/authentication/oauth/token
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OIDC authentication of the customer account.
  flows: []
  scope: openid
- description: Access to the customer's email address.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API surface for agent-driven access.
  flows: []
  scope: customer-account-mcp-api:full
slug: nara-organics-scopes
source_filename: nara-organics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://nara.com/.well-known/oauth-authorization-server (scopes_supported) + https://nara.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  authorizationUrl: https://account.nara.com/authentication/oauth/authorize\n  tokenUrl: https://account.nara.com/authentication/oauth/token\n  source: well-known/nara-organics-openid-configuration.json\nscopes:\n- scope: openid\n  description: OIDC authentication of the customer account.\n- scope: email\n  description: Access to the customer's email address.\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer.\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API surface for agent-driven access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nara-organics/refs/heads/main/scopes/nara-organics-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Consumer
- Commerce
- Retail
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Infant Formula
token_urls: []
---
