---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Linusbio Scopes
name_suffix: OAuth Scopes
note: Derived directly from the scopes_supported array of the RFC 8414 authorization server metadata served on traced.life. LinusBio publishes no scope reference page; these are the Shopify Customer Accounts scopes for the Traced storefront. No OpenAPI declaring oauth2 securitySchemes exists for this provider, so derive-oauth-scopes.py had no input.
overview: 'LinusBio uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LinusBio
provider_slug: linusbio
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: linusbio-scopes
source_filename: linusbio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://traced.life/.well-known/oauth-authorization-server\nnote: >-\n  Derived directly from the scopes_supported array of the RFC 8414 authorization server\n  metadata served on traced.life. LinusBio publishes no scope reference page; these are the\n  Shopify Customer Accounts scopes for the Traced storefront. No OpenAPI declaring oauth2\n  securitySchemes exists for this provider, so derive-oauth-scopes.py had no input.\nauthorization_server: https://shopify.com/authentication/70566805578\nprotected_resource: https://traced.life\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OIDC scope requesting an ID token for the authenticated customer.\n- name: email\n  description: Releases the email and email_verified claims for the authenticated customer.\n- name: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API for the authenticated customer of the\n    traced.life\
  \ store (orders, addresses, profile).\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the authenticated Customer Account MCP surface. This is a distinct,\n    credentialed MCP surface from the anonymous UCP commerce endpoint at\n    https://traced.life/api/ucp/mcp; its tool list was not probed because it requires\n    customer credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linusbio/refs/heads/main/scopes/linusbio-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Health
- Diagnostics
- Precision Medicine
- Biotechnology
- Exposomics
- Life Sciences
- Autism
- Commerce
- Agents
token_urls: []
---
