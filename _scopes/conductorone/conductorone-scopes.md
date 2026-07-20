---
api_specs:
- filename: conductorone-openapi-original.yml
  format: yaml
  label: ConductorOne API
  slug: conductorone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conductorone/refs/heads/main/openapi/conductorone-openapi-original.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Conductorone Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ConductorOne uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /auth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ConductorOne
provider_slug: conductorone
schemes:
- description: 'This API uses OAuth2 with the Client Credential flow.

    Client Credentials must be sent in the BODY, not the headers.

    For an example of how to implement this, refer to the [c1TokenSource.Token()](https://github.com/ConductorOne/conductorone-sdk-go/blob/3375fe7c0126d17e7ec4e711693dee7b791023aa/token_source.go#L101-L187) function.'
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/v1/token
  name: oauth
  source: openapi/conductorone-openapi-original.yml
scope_count: 0
scope_names: []
scopes: []
slug: conductorone-scopes
source_filename: conductorone-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/conductorone-openapi-original.yml\nschemes:\n- name: oauth\n  source: openapi/conductorone-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/v1/token\n  description: |-\n    This API uses OAuth2 with the Client Credential flow.\n    Client Credentials must be sent in the BODY, not the headers.\n    For an example of how to implement this, refer to the [c1TokenSource.Token()](https://github.com/ConductorOne/conductorone-sdk-go/blob/3375fe7c0126d17e7ec4e711693dee7b791023aa/token_source.go#L101-L187) function.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conductorone/refs/heads/main/scopes/conductorone-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Cloud Saas
- Identity Security
- Access Governance
- Identity and Access Management
- Access Reviews
- Provisioning
- Least Privilege
- MCP Governance
- Security
token_urls:
- /auth/v1/token
---
