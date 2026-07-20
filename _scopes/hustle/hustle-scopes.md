---
api_specs:
- filename: hustle-openapi-original.json
  format: json
  label: Hustle Public API
  slug: hustle-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-openapi-original.json
authorization_urls: []
description: ''
docs: https://api.hustle.com/v3/docs/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Hustle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hustle uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.hustle.com/v3/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hustle
provider_slug: hustle
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.hustle.com/v3/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/hustle-openapi-original.json
scope_count: 0
scope_names: []
scopes: []
slug: hustle-scopes
source_filename: hustle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hustle-openapi-original.json\ndocs: https://api.hustle.com/v3/docs/\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/hustle-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.hustle.com/v3/oauth/token\nscopes: []\nnotes: >-\n  The Hustle Public API uses the OAuth2 client-credentials flow and returns a\n  `scope` string on the token response, but the spec does not declare a\n  components.securitySchemes.flows.clientCredentials.scopes map and no\n  per-operation `security[]` scope requirements are present. No enumerable scope\n  values are published in the OpenAPI, so the derived scope list is empty by\n  design (absence is valid data, not a gap to fabricate). Access is governed by\n  the credentials issued to the client rather than a documented scope catalog.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/scopes/hustle-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Enterprise
- Messaging
- SMS
- Peer-to-Peer Texting
- Communications
- Marketing
- Civic Engagement
- Webhooks
- OAuth
token_urls:
- https://api.hustle.com/v3/oauth/token
---
