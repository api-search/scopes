---
api_specs:
- filename: lawmatics-openapi.yml
  format: yaml
  label: Lawmatics OAuth API
  slug: lawmatics-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lawmatics/refs/heads/main/openapi/lawmatics-openapi.yml
authorization_urls:
- https://app.lawmatics.com/oauth/authorize
description: ''
docs: https://docs.lawmatics.com/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Lawmatics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lawmatics uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.lawmatics.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lawmatics
provider_slug: lawmatics
schemes:
- description: OAuth 2.0 authorization code grant. Register a developer app at https://app.lawmatics.com/settings/developers (developer settings must be enabled by Lawmatics support). Access tokens are non-expiring; no refresh tokens are issued and scopes are not supported.
  flows:
  - authorizationUrl: https://app.lawmatics.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.lawmatics.com/oauth/token
  name: oauth2
  source: openapi/lawmatics-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: lawmatics-scopes
source_filename: lawmatics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.lawmatics.com/\ndocs: https://docs.lawmatics.com/\nderived_from: openapi/lawmatics-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/lawmatics-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.lawmatics.com/oauth/authorize\n    tokenUrl: https://api.lawmatics.com/oauth/token\n  description: OAuth 2.0 authorization code grant. Register a developer app at https://app.lawmatics.com/settings/developers\n    (developer settings must be enabled by Lawmatics support). Access tokens are non-expiring; no refresh\n    tokens are issued and scopes are not supported.\nscopes: []\nscope_count: 0\nsupported: false\nfinding: 'Lawmatics runs OAuth 2.0 but implements NO scopes, and says so in its own documentation: \"We\n  currently do not support scopes. Once a user authenticates your app, they are giving you full CRUD access\n  to their account.\" The empty scopes list below is therefore\
  \ a measured fact, not a harvesting failure.\n  Combined with non-expiring tokens and no deauthorization endpoint, an authorized integration holds permanent\n  unrestricted access to a law firm''s client data - there is no least-privilege posture available to\n  an integrator, and no way to issue a read-only credential to an agent.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lawmatics/refs/heads/main/scopes/lawmatics-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Legal
- CRM
- Law Firms
- Client Intake
- Marketing Automation
- Matter Management
- E-Signature
- Workflow-Automation
- Legal Tech
- Time and Billing
- Webhook
- Authentication
token_urls:
- https://api.lawmatics.com/oauth/token
---
