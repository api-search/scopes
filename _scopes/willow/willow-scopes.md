---
authorization_urls: []
description: ''
docs: https://onewillow.com/.well-known/oauth-authorization-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Willow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Willow uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Willow
provider_slug: willow
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: willow-scopes
source_filename: willow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://onewillow.com/.well-known/openid-configuration\ndocs: https://onewillow.com/.well-known/oauth-authorization-server\nsummary: >-\n  The only OAuth surface Willow serves is Shopify Customer Accounts on its own account.onewillow.com\n  host. Its RFC 8414 / OIDC metadata declares four scopes. Willow publishes no scope reference page\n  of its own; the descriptions below are read from the scope names and the discovery document, and\n  are marked as such.\nissuer: https://shopify.com/authentication/15958015\nauthorization_server: https://account.onewillow.com\nscope_count: 4\nscopes:\n  - name: openid\n    description: OpenID Connect — request an ID token for the signed-in Willow customer.\n    standard: true\n    description_method: derived\n  - name: email\n    description: Release the customer's email address and email_verified claim.\n    standard: true\n    description_method: derived\n  - name: customer-account-api:full\n\
  \    description: >-\n      Full access to the Willow customer account API for the signed-in buyer — orders, addresses,\n      payment methods and profile on onewillow.com.\n    standard: false\n    description_method: derived\n  - name: customer-account-mcp-api:full\n    description: >-\n      Full access to the MCP-addressable projection of the same customer account surface. This is the\n      scope an agent acting for a signed-in Willow buyer would hold.\n    standard: false\n    description_method: derived\nclaims_supported:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - nonce\n  - sid\n  - email\n  - email_verified\nnotes:\n  - >-\n    The anonymous UCP commerce MCP endpoint (https://onewillow.com/api/ucp/mcp) is NOT scope-gated —\n    it gates on a UCP agent profile URI and, for order reads, an agent JWT. See\n    authentication/willow-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/willow/refs/heads/main/scopes/willow-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Consumer Health
- Breast Pumps
- Maternal Health
- Medical Devices
- Ecommerce
- Agentic Commerce
- MCP
- UCP
- agent-native
- Shopify
token_urls: []
---
