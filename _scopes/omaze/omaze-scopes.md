---
authorization_urls: []
description: The OAuth 2.0 / OpenID Connect scopes advertised by the Shopify Customer Accounts authorization server behind the Omaze UK and German storefronts. Both markets advertise an identical set. These are the provider's own published values, read straight from the discovery document — none are inferred, and no scope descriptions beyond what the standard defines are asserted, because Omaze publishes no scope reference page of its own.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Omaze Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Omaze uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Omaze
provider_slug: omaze
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: omaze-scopes
source_filename: omaze-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: >-\n  scopes_supported from https://omaze.co.uk/.well-known/openid-configuration and\n  https://omaze.de/.well-known/openid-configuration, fetched 2026-08-02.\ndescription: >-\n  The OAuth 2.0 / OpenID Connect scopes advertised by the Shopify Customer\n  Accounts authorization server behind the Omaze UK and German storefronts. Both\n  markets advertise an identical set. These are the provider's own published\n  values, read straight from the discovery document — none are inferred, and no\n  scope descriptions beyond what the standard defines are asserted, because\n  Omaze publishes no scope reference page of its own.\nissuers:\n  - market: United Kingdom\n    issuer: https://shopify.com/authentication/27583905878\n    authorization_server: https://accounts.omaze.co.uk\n  - market: Germany\n    issuer: https://shopify.com/authentication/69889196213\n    authorization_server: https://accounts.omaze.de\nflows:\n  - type: authorization_code\n\
  \    pkce_required: true\n    code_challenge_methods:\n      - S256\nscopes:\n  - name: openid\n    description: >-\n      Standard OpenID Connect scope. Requests an ID token identifying the\n      authenticated Omaze customer.\n    standard: OpenID Connect Core 1.0\n  - name: email\n    description: >-\n      Standard OpenID Connect scope. Releases the `email` and `email_verified`\n      claims for the authenticated customer.\n    standard: OpenID Connect Core 1.0\n  - name: 'customer-account-api:full'\n    description: >-\n      Full access to the Shopify Customer Account API on behalf of the signed-in\n      customer — the account surface behind /account on the storefront (orders,\n      entries, subscriptions, profile).\n    standard: Shopify Customer Accounts\n  - name: 'customer-account-mcp-api:full'\n    description: >-\n      Full access to the authenticated Customer Account MCP surface. This is the\n      agent-facing counterpart to `customer-account-api:full`, and is distinct\n\
  \      from the anonymous UCP shopping MCP endpoint at /api/ucp/mcp.\n    standard: Shopify Customer Accounts\n    note: >-\n      Notable: Omaze's identity layer advertises an MCP-scoped grant. An agent\n      holding this scope acts as the customer against their own account, not as\n      an anonymous shopper.\nclaims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\ndocs: null\ndocs_note: >-\n  Omaze publishes no scope/permission reference page. The authoritative source\n  for these values is the live discovery document; Shopify documents the\n  underlying scopes at https://shopify.dev/docs/api/customer.\nauthentication: ../authentication/omaze-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omaze/refs/heads/main/scopes/omaze-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Charity
- Fundraising
- Nonprofit
- Prize Draws
- Sweepstakes
- Ecommerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- United Kingdom
- Germany
token_urls: []
---
