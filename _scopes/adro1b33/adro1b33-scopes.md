---
api_specs:
- filename: adro1b33-aox-openapi.yaml
  format: yaml
  label: AOX Platform API
  slug: aox-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adro1b33/refs/heads/main/openapi/adro1b33-aox-openapi.yaml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Adro1B33 Scopes
name_suffix: OAuth Scopes
note: The AOX Platform API at api.aoxlabs.com declares no oauth2 securityScheme and publishes no scope reference, so it contributes no scopes to this file. These four are the storefront identity scopes ADRO's own domain advertises; the authorization server is Shopify's, scoped to ADRO's shop id.
overview: 'ADRO uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ADRO
provider_slug: adro1b33
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: adro1b33-scopes
source_filename: adro1b33-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://adro.com/.well-known/openid-configuration\napplies_to: ADRO US Store Agent Commerce (UCP / MCP)\nauthorization_server: https://shopify.com/authentication/67310649500\nauthorization_endpoint: https://shopify.com/authentication/67310649500/oauth/authorize\ntoken_endpoint: https://shopify.com/authentication/67310649500/oauth/token\njwks_uri: https://shopify.com/authentication/67310649500/.well-known/jwks.json\ngrant_types:\n- authorization_code\n- refresh_token\n- urn:ietf:params:oauth:grant-type:jwt-bearer\npkce:\n- S256\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an id_token identifying the customer.\n- name: email\n  description: Releases the customer's email address and email_verified claim.\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for this shop on the customer's behalf.\n- name: customer-account-mcp-api:full\n\
  \  description: >-\n    Full access to the Customer Account MCP API — the authenticated agent surface that sits alongside\n    the anonymous UCP commerce MCP endpoint at /api/ucp/mcp.\nnote: >-\n  The AOX Platform API at api.aoxlabs.com declares no oauth2 securityScheme and publishes no scope\n  reference, so it contributes no scopes to this file. These four are the storefront identity scopes\n  ADRO's own domain advertises; the authorization server is Shopify's, scoped to ADRO's shop id.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adro1b33/refs/heads/main/scopes/adro1b33-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Aerodynamics
- Computational Fluid Dynamics
- Simulation
- Automotive
- Engineering
- Optimization
- Manufacturing
- Artificial Intelligence
- High Performance Computing
- Ecommerce
- MCP
- South Korea
token_urls: []
---
