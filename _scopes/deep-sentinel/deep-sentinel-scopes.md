---
authorization_urls:
- https://account.deepsentinel.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Deep Sentinel Scopes
name_suffix: OAuth Scopes
note: The complete `scopes_supported` set advertised by Deep Sentinel's own OIDC discovery document. There is no OpenAPI in this repo, so derive-oauth-scopes.py had nothing to read; these scopes come straight off the live discovery metadata. Deep Sentinel publishes no scope reference page of its own — the descriptions below are the standard meanings of these identifiers, not provider prose, and are marked as such.
overview: 'Deep Sentinel publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Deep Sentinel API on a user''s behalf.


  Tokens are issued from https://account.deepsentinel.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Deep Sentinel
provider_slug: deep-sentinel
schemes:
- flows:
  - authorizationUrl: https://account.deepsentinel.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.deepsentinel.com/authentication/oauth/token
  name: shopify-customer-account-oidc
  source: well-known/deep-sentinel-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Release the authenticated customer's email address and email_verified claim.
  flows: []
  scope: email
- description: Full access to the authenticated customer's account API (orders, addresses, payment methods, subscriptions).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the authenticated Customer Account MCP API, the agent-facing projection of the customer account.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: deep-sentinel-scopes
source_filename: deep-sentinel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://shop.deepsentinel.com/.well-known/openid-configuration\nnote: >-\n  The complete `scopes_supported` set advertised by Deep Sentinel's own OIDC discovery\n  document. There is no OpenAPI in this repo, so derive-oauth-scopes.py had nothing to\n  read; these scopes come straight off the live discovery metadata. Deep Sentinel\n  publishes no scope reference page of its own — the descriptions below are the standard\n  meanings of these identifiers, not provider prose, and are marked as such.\nschemes:\n- name: shopify-customer-account-oidc\n  source: well-known/deep-sentinel-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.deepsentinel.com/authentication/oauth/authorize\n    tokenUrl: https://account.deepsentinel.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token.\n  description_source:\
  \ standard\n  flows: [authorizationCode]\n- scope: email\n  description: Release the authenticated customer's email address and email_verified\n    claim.\n  description_source: standard\n- scope: customer-account-api:full\n  description: Full access to the authenticated customer's account API (orders, addresses,\n    payment methods, subscriptions).\n  description_source: standard\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the authenticated Customer Account MCP API, the agent-facing\n    projection of the customer account.\n  description_source: standard\n  flows: [authorizationCode]\n  note: >-\n    Notable: the identity layer advertises an MCP-specific scope, meaning agent access to\n    the customer account is a first-class, separately-scoped grant rather than an\n    afterthought on the REST scope.\ndocs: null\ndocs_note: Deep Sentinel publishes no scopes/permissions reference page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deep-sentinel/refs/heads/main/scopes/deep-sentinel-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Security
- Physical Security
- Video Surveillance
- Home Security
- Artificial Intelligence
- Computer Vision
- Monitoring
- Internet of Things
- Commerce
token_urls:
- https://account.deepsentinel.com/authentication/oauth/token
---
