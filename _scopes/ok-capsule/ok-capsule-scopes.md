---
api_specs:
- filename: ok-capsule-core-api-v2-openapi.yaml
  format: yaml
  label: OK Capsule Core API V2
  slug: ok-capsule-core-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ok-capsule/refs/heads/main/openapi/ok-capsule-core-api-v2-openapi.yaml
authorization_urls: []
description: ''
docs: https://okcapsule.com/mcp/developers
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ok Capsule Scopes
name_suffix: OAuth Scopes
note: These scopes govern the MCP server (https://storefront.okcapsule.app/mcp), not the REST Core API V2. The REST API declares a single bearerAuth (http/JWT) securityScheme with no oauth2 flows and therefore has no scope surface; its permissions are role-based and managed in the client portal. The scope list here is read verbatim from the RFC 8414 discovery document (scopes_supported) and cross-checked against the provider's own scope table at https://okcapsule.com/mcp/developers. The provider states the discovery document is authoritative and that "scopes may be added or split", so clients should read it at runtime.
overview: 'OK Capsule uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OK Capsule
provider_slug: ok-capsule
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ok-capsule-scopes
source_filename: ok-capsule-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://storefront.okcapsule.app/.well-known/oauth-authorization-server\ndocs: https://okcapsule.com/mcp/developers\nnote: >-\n  These scopes govern the MCP server (https://storefront.okcapsule.app/mcp), not the REST Core API V2.\n  The REST API declares a single bearerAuth (http/JWT) securityScheme with no oauth2 flows and\n  therefore has no scope surface; its permissions are role-based and managed in the client portal.\n  The scope list here is read verbatim from the RFC 8414 discovery document (scopes_supported) and\n  cross-checked against the provider's own scope table at https://okcapsule.com/mcp/developers. The\n  provider states the discovery document is authoritative and that \"scopes may be added or split\", so\n  clients should read it at runtime.\nauthorization_server: https://storefront.okcapsule.app\nflows:\n- type: authorization_code\n  authorization_endpoint: https://storefront.okcapsule.app/oauth/authorize\n\
  \  token_endpoint: https://storefront.okcapsule.app/oauth/token\n  registration_endpoint: https://storefront.okcapsule.app/oauth/register\n  revocation_endpoint: https://storefront.okcapsule.app/oauth/revoke\n  pkce: required (S256)\n  token_endpoint_auth_methods_supported: [none]\n- type: refresh_token\nscope_count: 16\nscopes:\n- name: catalog:read\n  description: Brands, products, catalog, product intelligence, pack builder\n  default_grant: true\n- name: recommendations:read\n  description: Recommendation validation\n  default_grant: true\n- name: orders:read\n  description: List/get orders, transaction logs, order status\n  default_grant: true\n- name: orders:write\n  description: Create/update orders\n  default_grant: false\n  consent: opt-in\n- name: orders:cancel\n  description: Cancel orders\n  default_grant: false\n  consent: opt-in\n  destructive: true\n- name: consumers:read\n  description: Get/list consumers\n  default_grant: true\n- name: consumers:write\n  description: Create/update\
  \ consumers\n  default_grant: true\n- name: consumers:delete\n  description: Delete consumers\n  default_grant: false\n  consent: opt-in\n  destructive: true\n- name: fulfillments:read\n  description: Fulfillments, shipping labels\n  default_grant: true\n- name: meta:read\n  description: Status lists\n  default_grant: true\n- name: documents:write\n  description: Supplement-facts PDF generation\n  default_grant: true\n- name: orders:read:own\n  description: >-\n    Present in scopes_supported in the discovery document. The \":own\" family is not documented in the\n    provider's published scope table; the developer page states there is no consumer-facing sign-in\n    yet, so these read as reserved for a future consumer persona.\n  default_grant: unknown\n- name: orders:write:own\n  description: Reserved consumer-persona scope present in scopes_supported but not in the published scope table.\n  default_grant: unknown\n- name: orders:cancel:own\n  description: Reserved consumer-persona scope\
  \ present in scopes_supported but not in the published scope table.\n  default_grant: unknown\n- name: profile:read:own\n  description: Reserved consumer-persona scope present in scopes_supported but not in the published scope table.\n  default_grant: unknown\n- name: profile:write:own\n  description: Reserved consumer-persona scope present in scopes_supported but not in the published scope table.\n  default_grant: unknown\nconsent_model: >-\n  Read access is the default grant; anything destructive is opt-in at the consent screen. The user\n  approves exactly what the client asked for, and one token is bound to exactly one workspace.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ok-capsule/refs/heads/main/scopes/ok-capsule-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Supplements
- Nutrition
- Health
- Manufacturing
- Fulfillment
- Ecommerce
- Personalization
- Orders
- Shipping
- Agents
- MCP
- Telehealth
token_urls: []
---
