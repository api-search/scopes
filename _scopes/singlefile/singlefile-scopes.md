---
api_specs:
- filename: singlefile-openapi.yml
  format: yaml
  label: SingleFile External API
  slug: singlefile-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singlefile/refs/heads/main/openapi/singlefile-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Singlefile Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SingleFile publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SingleFile API on a user''s behalf.


  Tokens are issued from https://api.demo.singlefile.ai/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SingleFile
provider_slug: singlefile
schemes:
- description: 'OAuth 2.0 Client Credentials flow. Exchange client_id/client_secret at the token endpoint for a 1-hour bearer token; send it as Authorization: Bearer <token>.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.demo.singlefile.ai/o/token/
  name: OAuth2ClientCredentials
  source: openapi/singlefile-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to entities, organizations, orders, documents, jurisdictions and tasks
  flows:
  - clientCredentials
  scope: read
- description: Create and update entities, organizations, orders, documents and jurisdictions
  flows:
  - clientCredentials
  scope: write
slug: singlefile-scopes
source_filename: singlefile-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/singlefile-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/singlefile-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.demo.singlefile.ai/o/token/\n  description: 'OAuth 2.0 Client Credentials flow. Exchange client_id/client_secret at the token\n    endpoint for a 1-hour bearer token; send it as Authorization: Bearer <token>.'\nscopes:\n- scope: read\n  description: Read access to entities, organizations, orders, documents, jurisdictions and\n    tasks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/singlefile-openapi.yml\n- scope: write\n  description: Create and update entities, organizations, orders, documents and jurisdictions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/singlefile-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singlefile/refs/heads/main/scopes/singlefile-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Compliance
- Legal
- Entity Management
- Corporate Compliance
- Registered Agent
- Business Filings
- Regulatory
- API
- Webhooks
- OAuth
token_urls:
- https://api.demo.singlefile.ai/o/token/
---
