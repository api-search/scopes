---
authorization_urls: []
description: ''
docs: https://ihealthlabs.com/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Andon Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Andon Health uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Andon Health
provider_slug: andon-health
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: andon-health-scopes
source_filename: andon-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: >-\n  ihealthlabs.com /.well-known/openid-configuration (scopes_supported). These\n  scopes govern the Shopify Customer Account API on the storefront. The iHealth\n  Open API V2 (api.ihealthlabs.com) also uses OAuth 2.0, but its device-data\n  scope list is not published on any public endpoint.\ndocs: https://ihealthlabs.com/.well-known/openid-configuration\nprovider: shopify-customer-account\nscopes:\n  - name: openid\n    description: OpenID Connect authentication; issue an ID token for the signed-in shopper.\n  - name: email\n    description: Access the shopper's email claim.\n  - name: customer-account-api:full\n    description: Full access to the Shopify Customer Account API for the authorized shopper.\n  - name: customer-account-mcp-api:full\n    description: >-\n      Full access to the Customer Account MCP API, enabling agent-driven access\n      to the shopper's account over the Model Context Protocol.\nnotes: >-\n\
  \  The iHealth Open API V2 device-data OAuth flow\n  (developer.ihealthlabs.com/api/public/oauth2/*) is confirmed live but its\n  scope names are gated behind developer registration and are not enumerated\n  publicly; only search evidence, no fabrication, is recorded here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andon-health/refs/heads/main/scopes/andon-health-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Medical Devices
- Digital Health
- Remote Patient Monitoring
- Connected Health
- IoT
- Wearables
token_urls: []
---
