---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Uniqode QR Code API
  slug: uniqode-qr-code-api
  spec_type: Postman
  url: https://apidocs.uniqode.com/
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Beaconstac Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Beaconstac publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Beaconstac API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beaconstac
provider_slug: beaconstac
schemes: []
scope_count: 6
scope_names:
- openid
- profile
- email
- offline_access
- read:analytics
- read:organizations
scopes:
- description: OIDC authentication; issues an ID token.
  flows: []
  scope: openid
- description: Standard OIDC profile claims (name, nickname, picture).
  flows: []
  scope: profile
- description: Standard OIDC email + email_verified claims.
  flows: []
  scope: email
- description: Issues a refresh token so the agent can act between interactive sessions.
  flows: []
  scope: offline_access
- description: Read access to scan/engagement analytics. Provider-specific; interpretation from the scope name — Uniqode publishes no scope reference page defining it.
  flows: []
  scope: read:analytics
- description: Read access to organization records and organization-wide reporting. Provider-specific; interpretation from the scope name — no published definition.
  flows: []
  scope: read:organizations
slug: beaconstac-scopes
source_filename: beaconstac-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.uniqode.com/.well-known/oauth-protected-resource\ndocs: null\n# No OpenAPI is published, so derive-oauth-scopes.py has nothing to read. The scopes below are\n# NOT derived and NOT guessed — they were read verbatim from the two anonymous discovery\n# documents Uniqode serves. Uniqode publishes no human-readable scope reference page; the\n# `description` on each row is our plain-language reading of the scope name, marked as such.\n# The REST API (api.uniqode.com) has no scope surface at all — it uses a static account token.\nauthorization_servers:\n- issuer: https://auth.uniqode.com/\n  metadata: well-known/beaconstac-oauth-authorization-server.json\n  authorization_endpoint: https://auth.uniqode.com/authorize\n  token_endpoint: https://auth.uniqode.com/oauth/token\n  registration_endpoint: https://auth.uniqode.com/oidc/register\n  revocation_endpoint: https://auth.uniqode.com/oauth/revoke\n  jwks_uri: https://auth.uniqode.com/.well-known/jwks.json\n\
  \  device_authorization_endpoint: https://auth.uniqode.com/oauth/device/code\n  code_challenge_methods_supported: [S256, plain]\n  dynamic_client_registration: true\n  platform: Auth0 on the uniqode.com custom identity domain\nprotected_resources:\n- resource: https://mcp.uniqode.com/\n  metadata: well-known/beaconstac-oauth-protected-resource.json\n  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  bearer_methods_supported: [header]\n# Scopes the MCP protected resource declares (scopes_supported)\nscopes:\n- scope: openid\n  description: OIDC authentication; issues an ID token.\n  standard: true\n  sources: [https://mcp.uniqode.com/.well-known/oauth-protected-resource]\n- scope: profile\n  description: Standard OIDC profile claims (name, nickname, picture).\n  standard: true\n  sources: [https://mcp.uniqode.com/.well-known/oauth-protected-resource]\n- scope: email\n  description: Standard OIDC email + email_verified claims.\n  standard: true\n  sources: [https://mcp.uniqode.com/.well-known/oauth-protected-resource]\n\
  - scope: offline_access\n  description: Issues a refresh token so the agent can act between interactive sessions.\n  standard: true\n  sources: [https://mcp.uniqode.com/.well-known/oauth-protected-resource]\n- scope: read:analytics\n  description: >-\n    Read access to scan/engagement analytics. Provider-specific; interpretation from the scope\n    name — Uniqode publishes no scope reference page defining it.\n  standard: false\n  interpretation: unverified-by-docs\n  sources: [https://mcp.uniqode.com/.well-known/oauth-protected-resource]\n- scope: read:organizations\n  description: >-\n    Read access to organization records and organization-wide reporting. Provider-specific;\n    interpretation from the scope name — no published definition.\n  standard: false\n  interpretation: unverified-by-docs\n  sources: [https://mcp.uniqode.com/.well-known/oauth-protected-resource]\nobservations:\n- >-\n  The published MCP scope set is READ-ONLY. There is no write/create scope, so the press-release\n\
  \  claim that the connector can \"create QR Codes individually or in bulk\" is not reachable through\n  any scope Uniqode advertises anonymously.\n- >-\n  The authorization server advertises 13 grant types including password, implicit and\n  client_credentials (an Auth0 tenant default set), which is broader than an MCP client needs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beaconstac/refs/heads/main/scopes/beaconstac-scopes.yml
summary_line: 6 scopes
tags:
- Company
- Big Data
- QR Codes
- Digital Business Cards
- Marketing
- Analytics
- SaaS
- Proximity
- Webhooks
- MCP
token_urls: []
---
