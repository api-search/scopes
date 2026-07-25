---
api_specs:
- filename: upwind-access-management-api-openapi.yml
  format: yaml
  label: Upwind access-management API
  slug: upwind-access-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-access-management-api-openapi.yml
- filename: upwind-api-security-api-openapi.yml
  format: yaml
  label: Upwind api-security API
  slug: upwind-api-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-api-security-api-openapi.yml
- filename: upwind-cloud-accounts-api-openapi.yml
  format: yaml
  label: Upwind cloud-accounts API
  slug: upwind-cloud-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-cloud-accounts-api-openapi.yml
- filename: upwind-configurations-api-openapi.yml
  format: yaml
  label: Upwind configurations API
  slug: upwind-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-configurations-api-openapi.yml
- filename: upwind-events-api-openapi.yml
  format: yaml
  label: Upwind events API
  slug: upwind-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-events-api-openapi.yml
- filename: upwind-integrations-api-openapi.yml
  format: yaml
  label: Upwind integrations API
  slug: upwind-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-integrations-api-openapi.yml
- filename: upwind-inventory-api-openapi.yml
  format: yaml
  label: Upwind Inventory API
  slug: upwind-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-inventory-api-openapi.yml
- filename: upwind-packages-api-openapi.yml
  format: yaml
  label: Upwind packages API
  slug: upwind-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-packages-api-openapi.yml
- filename: upwind-shiftleft-api-openapi.yml
  format: yaml
  label: Upwind shiftleft API
  slug: upwind-shiftleft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-shiftleft-api-openapi.yml
- filename: upwind-threats-api-openapi.yml
  format: yaml
  label: Upwind threats API
  slug: upwind-threats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-threats-api-openapi.yml
- filename: upwind-vulnerabilities-api-openapi.yml
  format: yaml
  label: Upwind vulnerabilities API
  slug: upwind-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-vulnerabilities-api-openapi.yml
- filename: upwind-workflows-api-openapi.yml
  format: yaml
  label: Upwind workflows API
  slug: upwind-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-workflows-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.upwind.io/settings/credentials
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Upwind Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Upwind uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.upwind.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Upwind
provider_slug: upwind
schemes:
- description: 'OAuth 2.0 client credentials grant. Obtain client credentials in the Upwind Management Console, then exchange them for a JWT access token at https://auth.upwind.io/oauth/token with an audience matching the regional API host (https://api.upwind.io, https://api.eu.upwind.io, or https://api.me.upwind.io). Send the token as Authorization: Bearer <token>.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.upwind.io/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/upwind-management-v1-openapi.yml
- description: 'OAuth 2.0 client credentials grant. Obtain client credentials in the Upwind Management Console, then exchange them for a JWT access token at https://auth.upwind.io/oauth/token with an audience matching the regional API host (https://api.upwind.io, https://api.eu.upwind.io, or https://api.me.upwind.io). Send the token as Authorization: Bearer <token>.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.upwind.io/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/upwind-management-v2-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: upwind-scopes
source_filename: upwind-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/upwind-management-v1-openapi.yml, openapi/upwind-management-v2-openapi.yml\ndocs: https://docs.upwind.io/settings/credentials\nnotes: >-\n  Upwind publishes no named OAuth scope strings. Authorization granularity is carried by the\n  audience parameter (one per regional API host) plus RBAC \"scope & roles\" attached to each API\n  credential in the console — any token generated from a credential inherits that credential's\n  permissions, bounded by the creating member's own access. Token lifetime is 24 hours.\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/upwind-management-v1-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.upwind.io/oauth/token\n  description: 'OAuth 2.0 client credentials grant. Obtain client credentials in the Upwind\n    Management Console, then exchange them for a JWT access token at https://auth.upwind.io/oauth/token\n    with an audience matching the\
  \ regional API host (https://api.upwind.io, https://api.eu.upwind.io,\n    or https://api.me.upwind.io). Send the token as Authorization: Bearer <token>.'\n- name: OAuth2ClientCredentials\n  source: openapi/upwind-management-v2-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.upwind.io/oauth/token\n  description: 'OAuth 2.0 client credentials grant. Obtain client credentials in the Upwind\n    Management Console, then exchange them for a JWT access token at https://auth.upwind.io/oauth/token\n    with an audience matching the regional API host (https://api.upwind.io, https://api.eu.upwind.io,\n    or https://api.me.upwind.io). Send the token as Authorization: Bearer <token>.'\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/scopes/upwind-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Security
- Cloud Security
- CNAPP
- Vulnerability Management
- Container Security
- Kubernetes
- API Security
- Threat Detection
- Data Security
token_urls:
- https://auth.upwind.io/oauth/token
---
