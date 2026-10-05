---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Agilitassports Scopes
name_suffix: OAuth Scopes
note: No client registration endpoint is published and no public client_id is documented, so these scopes are not requestable by a third-party integrator today. They are recorded as probed fact, not as an available developer surface.
overview: 'Agilitas Sports publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Agilitas Sports API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agilitas Sports
provider_slug: agilitassports
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Request an ID token identifying the signed-in shopper.
  flows: []
  scope: openid
- description: Release the shopper's email and email_verified claims.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in shopper (orders, addresses, profile). Semantics are Shopify's; Agilitas documents none of it.
  flows: []
  scope: customer-account-api:full
- description: Full access to the authenticated Shopify customer-account MCP API on behalf of the signed-in shopper. Not documented or advertised anywhere on an Agilitas host; listed here only because the discovery document served on agilitas.com names it.
  flows: []
  scope: customer-account-mcp-api:full
slug: agilitassports-scopes
source_filename: agilitassports-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://agilitas.com/.well-known/openid-configuration (HTTP 200, fetched 2026-09-12)\nname: Agilitas OAuth scopes\nslug: agilitassports\ndocs: null\ndocs_note: >-\n  Agilitas publishes no scope reference page of its own. The scope list below is read verbatim from\n  the scopes_supported array of the OIDC discovery document served at the Agilitas domain; the\n  descriptions are Shopify customer-account semantics, marked as such.\n\nauthorization_server: https://shopify.com/authentication/99796025642\noperator: Shopify (customer-account identity provider for shop 99796025642)\napplies_to: >-\n  Shopper sign-in to a customer account. NOT the anonymous UCP/MCP commerce surface, which requires\n  no token at all — see authentication/agilitassports-authentication.yml.\n\nscope_count: 4\nscopes:\n- name: openid\n  standard: OpenID Connect Core\n  description: Request an ID token identifying the signed-in shopper.\n  source: discovery\n\
  - name: email\n  standard: OpenID Connect Core\n  description: Release the shopper's email and email_verified claims.\n  source: discovery\n- name: customer-account-api:full\n  standard: Shopify\n  description: >-\n    Full access to the Shopify Customer Account API on behalf of the signed-in shopper (orders,\n    addresses, profile). Semantics are Shopify's; Agilitas documents none of it.\n  source: discovery\n- name: customer-account-mcp-api:full\n  standard: Shopify\n  description: >-\n    Full access to the authenticated Shopify customer-account MCP API on behalf of the signed-in\n    shopper. Not documented or advertised anywhere on an Agilitas host; listed here only because the\n    discovery document served on agilitas.com names it.\n  source: discovery\n\nclaims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\ncode_challenge_methods_supported: [S256]\nresponse_types_supported: [code]\n\nnote: >-\n  No client registration endpoint is published and no public\
  \ client_id is documented, so these\n  scopes are not requestable by a third-party integrator today. They are recorded as probed fact,\n  not as an available developer surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agilitassports/refs/heads/main/scopes/agilitassports-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Sportswear
- Footwear
- Athleisure
- Manufacturing
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- India
token_bound: false
token_urls: []
---
