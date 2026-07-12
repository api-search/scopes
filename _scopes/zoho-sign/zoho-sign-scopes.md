---
authorization_urls:
- https://accounts.zoho.com/oauth/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zoho Sign Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zoho Sign publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoho Sign API on a user''s behalf.


  Tokens are issued from https://accounts.zoho.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoho Sign
provider_slug: zoho-sign
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: oauth2
  source: openapi/openapi.json
scope_count: 3
scope_names:
- ZohoSign.account.ALL
- ZohoSign.documents.ALL
- ZohoSign.templates.ALL
scopes:
- description: Account operations
  flows:
  - authorizationCode
  scope: ZohoSign.account.ALL
- description: All document operations
  flows:
  - authorizationCode
  scope: ZohoSign.documents.ALL
- description: All template operations
  flows:
  - authorizationCode
  scope: ZohoSign.templates.ALL
slug: zoho-sign-scopes
source_filename: zoho-sign-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nschemes:\n- name: oauth2\n  source: openapi/openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\nscopes:\n- scope: ZohoSign.account.ALL\n  description: Account operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoSign.documents.ALL\n  description: All document operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoSign.templates.ALL\n  description: All template operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-sign/refs/heads/main/scopes/zoho-sign-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Electronic Signatures
- eSignature
- Document Management
- Digital Signatures
- Signature Workflows
- Templates
- Compliance
token_urls:
- https://accounts.zoho.com/oauth/v2/token
---
