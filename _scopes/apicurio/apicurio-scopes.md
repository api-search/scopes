---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Apicurio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Apicurio publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Apicurio API on a user''s behalf.


  Tokens are issued from https://example.com/realms/apicurio/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apicurio
provider_slug: apicurio
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/realms/apicurio/protocol/openid-connect/token
  name: OAuth2
  source: openapi/apicurio-openapi.yml
scope_count: 3
scope_names:
- admin
- read
- write
scopes:
- description: Admin access
  flows:
  - clientCredentials
  scope: admin
- description: Read access
  flows:
  - clientCredentials
  scope: read
- description: Write access
  flows:
  - clientCredentials
  scope: write
slug: apicurio-scopes
source_filename: apicurio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apicurio-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/apicurio-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/realms/apicurio/protocol/openid-connect/token\nscopes:\n- scope: admin\n  description: Admin access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/apicurio-openapi.yml\n- scope: read\n  description: Read access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/apicurio-openapi.yml\n- scope: write\n  description: Write access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/apicurio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/scopes/apicurio-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Apache License
- API Design
- API Registry
- Avro
- AsyncAPI
- Java
- Open Source
- OpenAPI
- Red Hat
- Schema Registry
token_urls:
- https://example.com/realms/apicurio/protocol/openid-connect/token
---
