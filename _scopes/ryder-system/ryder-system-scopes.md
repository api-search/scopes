---
authorization_urls: []
description: ''
docs: https://developer.ryder.com/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Ryder System Scopes
name_suffix: OAuth Scopes
note: Ryder uses a fixed-scope OAuth model — the authentication docs document only the single scope APIM, with no granular per-permission scopes published (https://developer.ryder.com/docs/authentication).
overview: 'Ryder System publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ryder System API on a user''s behalf.


  Tokens are issued from https://login.okta.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ryder System
provider_slug: ryder-system
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.okta.com/oauth2/v1/token
  name: oauth2
  source: openapi/ryder-tm-shipment-api-openapi.yml
scope_count: 1
scope_names:
- APIM
scopes:
- description: The single fixed scope Ryder documents for OAuth 2.0 token requests (both Client Credentials and Authorization Code flows) against its Okta-backed Azure API Management gateway; requests must set scope to APIM, with per-API access governed by the Ocp-Apim-Subscription-Key subscription key rather than granular scopes.
  flows: []
  scope: APIM
slug: ryder-system-scopes
source_filename: ryder-system-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/ryder-tm-shipment-api-openapi.yml\ndocs: https://developer.ryder.com/docs/authentication\nschemes:\n- name: oauth2\n  source: openapi/ryder-tm-shipment-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.okta.com/oauth2/v1/token\nscopes:\n- scope: APIM\n  description: The single fixed scope Ryder documents for OAuth 2.0 token requests\n    (both Client Credentials and Authorization Code flows) against its Okta-backed\n    Azure API Management gateway; requests must set scope to APIM, with per-API access\n    governed by the Ocp-Apim-Subscription-Key subscription key rather than granular\n    scopes.\n  sources:\n  - https://developer.ryder.com/docs/authentication\nnote: Ryder uses a fixed-scope OAuth model — the authentication docs document only\n  the single scope APIM, with no granular per-permission scopes published (https://developer.ryder.com/docs/authentication).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/scopes/ryder-system-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Fleet Management
- Logistics
- Supply Chain
- Transportation
- Trucking
- Fortune 500
token_urls:
- https://login.okta.com/oauth2/v1/token
---
