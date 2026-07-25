---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Our Place Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Our Place publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Our Place API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Our Place
provider_slug: our-place
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; enables issuance of an ID token.
  flows: []
  scope: openid
- description: Grants access to the customer's email address and email_verified claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API surface for agent-driven commerce.
  flows: []
  scope: customer-account-mcp-api:full
slug: our-place-scopes
source_filename: our-place-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://fromourplace.com/.well-known/openid-configuration (scopes_supported)\nissuer: https://shopify.com/authentication/2441379915\nauthorization_endpoint: https://account.fromourplace.com/authentication/oauth/authorize\nscope_count: 4\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; enables issuance of an ID token.\n- scope: email\n  description: Grants access to the customer's email address and email_verified claim.\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API surface for agent-driven commerce.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/our-place/refs/heads/main/scopes/our-place-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Ecommerce
- Retail
- Cookware
- Consumer
- Agentic Commerce
- Shopify
token_urls: []
---
