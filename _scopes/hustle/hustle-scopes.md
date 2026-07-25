---
api_specs:
- filename: hustle-access-token-api-openapi.yml
  format: yaml
  label: Hustle Access Token API
  slug: hustle-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-access-token-api-openapi.yml
- filename: hustle-agents-api-openapi.yml
  format: yaml
  label: Hustle Agents API
  slug: hustle-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-agents-api-openapi.yml
- filename: hustle-custom-fields-api-openapi.yml
  format: yaml
  label: Hustle Custom Fields API
  slug: hustle-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-custom-fields-api-openapi.yml
- filename: hustle-groups-api-openapi.yml
  format: yaml
  label: Hustle Groups API
  slug: hustle-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-groups-api-openapi.yml
- filename: hustle-integrations-api-openapi.yml
  format: yaml
  label: Hustle Integrations API
  slug: hustle-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-integrations-api-openapi.yml
- filename: hustle-leads-api-openapi.yml
  format: yaml
  label: Hustle Leads API
  slug: hustle-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-leads-api-openapi.yml
- filename: hustle-organizations-api-openapi.yml
  format: yaml
  label: Hustle Organizations API
  slug: hustle-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-organizations-api-openapi.yml
- filename: hustle-tags-api-openapi.yml
  format: yaml
  label: Hustle Tags API
  slug: hustle-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-tags-api-openapi.yml
- filename: hustle-webhooks-api-openapi.yml
  format: yaml
  label: Hustle Webhooks API
  slug: hustle-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hustle/refs/heads/main/openapi/hustle-webhooks-api-openapi.yml
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
