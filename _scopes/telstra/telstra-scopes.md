---
api_specs:
- filename: telstra-messaging-api-openapi.yml
  format: yaml
  label: Telstra Messaging API
  slug: telstra-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/openapi/telstra-messaging-api-openapi.yml
- filename: telstra-mobile-number-verification-api-openapi.yml
  format: yaml
  label: Telstra Mobile Number Verification API
  slug: telstra-mobile-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/openapi/telstra-mobile-number-verification-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Telstra Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Telstra publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Telstra API on a user''s behalf.


  Tokens are issued from https://tapi.telstra.com/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Telstra
provider_slug: telstra
schemes:
- description: OAuth 2.0 client credentials grant against https://tapi.telstra.com/v2/oauth/token with the NSMS scope.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tapi.telstra.com/v2/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/telstra-messaging-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://tapi.telstra.com/v2/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/telstra-mobile-number-verification-api-openapi.yml
scope_count: 2
scope_names:
- MNV
- NSMS
scopes:
- description: Mobile Number Verification.
  flows:
  - clientCredentials
  scope: MNV
- description: Send and receive SMS/MMS through Telstra Messaging.
  flows:
  - clientCredentials
  scope: NSMS
slug: telstra-scopes
source_filename: telstra-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telstra-messaging-api-openapi.yml, openapi/telstra-mobile-number-verification-api-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/telstra-messaging-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tapi.telstra.com/v2/oauth/token\n  description: OAuth 2.0 client credentials grant against https://tapi.telstra.com/v2/oauth/token\n    with the NSMS scope.\n- name: OAuth2ClientCredentials\n  source: openapi/telstra-mobile-number-verification-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tapi.telstra.com/v2/oauth/token\nscopes:\n- scope: MNV\n  description: Mobile Number Verification.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/telstra-mobile-number-verification-api-openapi.yml\n- scope: NSMS\n  description: Send and receive SMS/MMS through Telstra Messaging.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/telstra-messaging-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/scopes/telstra-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Telecommunications
- Telco
- Mobile
- Messaging
- SMS
- MMS
- Networks
- Australia
- Verification
token_urls:
- https://tapi.telstra.com/v2/oauth/token
---
