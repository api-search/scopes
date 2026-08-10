---
authorization_urls:
- https://api.meshpayments.com/as/authorize
description: ''
docs: https://developers.meshpayments.com
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Mesh Payments Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mesh Payments publishes 1 OAuth 2.0 scope via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mesh Payments API on a user''s behalf.


  Tokens are issued from https://api.meshpayments.com/as/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mesh Payments
provider_slug: mesh-payments
schemes:
- flows:
  - authorizationUrl: https://api.meshpayments.com/as/authorize
    flow: authorizationCode
    tokenUrl: https://api.meshpayments.com/as/token
  - flow: clientCredentials
    tokenUrl: https://api.meshpayments.com/as/token
  - deviceAuthorizationUrl: https://api.meshpayments.com/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://api.meshpayments.com/as/token
  issuer: https://api.meshpayments.com
  name: Mesh Payments authorization server
  source: https://api.meshpayments.com/.well-known/openid-configuration
scope_count: 1
scope_names:
- openid
scopes:
- description: OpenID Connect authentication scope; requests an ID token from the Mesh authorization server.
  flows:
  - authorizationCode
  scope: openid
slug: mesh-payments-scopes
source_filename: mesh-payments-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://api.meshpayments.com/.well-known/openid-configuration\ndocs: https://developers.meshpayments.com\ndocs_note: the developers portal that would carry the scope/permission reference returns\n  401 (HTTP Basic) to the public, so only the scopes the authorization server advertises\n  anonymously are recorded.\nschemes:\n- name: Mesh Payments authorization server\n  issuer: https://api.meshpayments.com\n  source: https://api.meshpayments.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.meshpayments.com/as/authorize\n    tokenUrl: https://api.meshpayments.com/as/token\n  - flow: clientCredentials\n    tokenUrl: https://api.meshpayments.com/as/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://api.meshpayments.com/oauth2/device_authorization\n    tokenUrl: https://api.meshpayments.com/as/token\nscopes:\n- scope: openid\n  description: OpenID Connect\
  \ authentication scope; requests an ID token from the Mesh\n    authorization server.\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.meshpayments.com/.well-known/openid-configuration\ngaps:\n- scopes_supported on the discovery document lists only \"openid\". Any API or MCP resource\n  scopes Mesh issues are not advertised anonymously, and the RFC 9728 protected-resource\n  metadata for https://api.meshpayments.com/mcp omits the optional scopes_supported\n  member. Publishing scopes_supported on the protected-resource metadata would let an\n  agent discover the permission surface without credentials.\nx-evidence:\n- fetched: '2026-08-04'\n  url: https://api.meshpayments.com/.well-known/openid-configuration\n  http_status: 200\n- fetched: '2026-08-04'\n  url: https://api.meshpayments.com/.well-known/oauth-protected-resource/mcp\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mesh-payments/refs/heads/main/scopes/mesh-payments-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Payments
- Spend Management
- Expense Management
- Corporate Cards
- Travel
- Accounts Payable
- Fintech
- Card Issuing
- Accounting Automation
token_urls:
- https://api.meshpayments.com/as/token
---
