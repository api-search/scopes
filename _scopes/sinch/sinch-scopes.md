---
authorization_urls: []
description: ''
docs: https://developers.sinch.com/docs/numbers/api-reference/authentication/oauth
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sinch Scopes
name_suffix: OAuth Scopes
note: Sinch OAuth 2.0 uses the client_credentials flow with project access keys (key ID and secret) and does not publish or use OAuth scopes (https://developers.sinch.com/docs/numbers/api-reference/authentication/oauth).
overview: 'Sinch uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.sinch.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sinch
provider_slug: sinch
schemes:
- description: OAuth 2.0 client credentials flow using project key ID and secret.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sinch.com/oauth2/token
  name: oAuth2
  source: openapi/sinch-conversation-openapi.yml
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sinch.com/oauth2/token
  name: oAuth2
  source: openapi/sinch-elastic-sip-trunking-openapi.yml
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sinch.com/oauth2/token
  name: oAuth2
  source: openapi/sinch-fax-openapi.yml
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sinch.com/oauth2/token
  name: oAuth2
  source: openapi/sinch-numbers-openapi.yml
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sinch.com/oauth2/token
  name: oAuth2
  source: openapi/sinch-provisioning-openapi.yml
- description: OAuth 2.0 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sinch.com/oauth2/token
  name: oAuth2
  source: openapi/sinch-registration-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: sinch-scopes
source_filename: sinch-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\ndocs: https://developers.sinch.com/docs/numbers/api-reference/authentication/oauth\nnote: Sinch OAuth 2.0 uses the client_credentials flow with project access keys (key\n  ID and secret) and does not publish or use OAuth scopes (https://developers.sinch.com/docs/numbers/api-reference/authentication/oauth).\nsource: openapi/sinch-conversation-openapi.yml, openapi/sinch-elastic-sip-trunking-openapi.yml,\n  openapi/sinch-fax-openapi.yml, openapi/sinch-numbers-openapi.yml, openapi/sinch-provisioning-openapi.yml,\n  openapi/sinch-registration-openapi.yml\nschemes:\n- name: oAuth2\n  source: openapi/sinch-conversation-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sinch.com/oauth2/token\n  description: OAuth 2.0 client credentials flow using project key ID and secret.\n- name: oAuth2\n  source: openapi/sinch-elastic-sip-trunking-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sinch.com/oauth2/token\n\
  \  description: OAuth 2.0 client credentials flow.\n- name: oAuth2\n  source: openapi/sinch-fax-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sinch.com/oauth2/token\n  description: OAuth 2.0 client credentials flow.\n- name: oAuth2\n  source: openapi/sinch-numbers-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sinch.com/oauth2/token\n  description: OAuth 2.0 client credentials flow.\n- name: oAuth2\n  source: openapi/sinch-provisioning-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sinch.com/oauth2/token\n  description: OAuth 2.0 client credentials flow.\n- name: oAuth2\n  source: openapi/sinch-registration-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sinch.com/oauth2/token\n  description: OAuth 2.0 client credentials flow.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/scopes/sinch-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Communications
- Messaging
- SMS
- Voice
- Verification
- CPaaS
token_urls:
- https://auth.sinch.com/oauth2/token
---
