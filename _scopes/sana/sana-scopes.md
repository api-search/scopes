---
api_specs:
- filename: sana-openapi.yml
  format: yaml
  label: Sana API
  slug: sana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.sana.ai/api-docs/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Sana Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sana publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sana API on a user''s behalf.


  Tokens are issued from https://{domain}.sana.ai/api/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sana
provider_slug: sana
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{domain}.sana.ai/api/token
  name: oauth2ClientCredentials
  source: https://docs.sana.ai/api-docs/
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access. Required for all GET requests.
  flows:
  - clientCredentials
  scope: read
- description: Write access. Required for all POST, PATCH, and DELETE requests.
  flows:
  - clientCredentials
  scope: write
slug: sana-scopes
source_filename: sana-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.sana.ai/api-docs/\ndocs: https://docs.sana.ai/api-docs/\nschemes:\n  - name: oauth2ClientCredentials\n    source: https://docs.sana.ai/api-docs/\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://{domain}.sana.ai/api/token\nscope_format: comma-separated\nscopes:\n  - scope: read\n    description: Read access. Required for all GET requests.\n    flows: [clientCredentials]\n    sources: [https://docs.sana.ai/api-docs/]\n  - scope: write\n    description: Write access. Required for all POST, PATCH, and DELETE requests.\n    flows: [clientCredentials]\n    sources: [https://docs.sana.ai/api-docs/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/scopes/sana-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Enterprise AI
- Artificial Intelligence
- Learning Management
- LMS
- Knowledge Management
- Agents
- SCIM
- xAPI
- REST API
token_urls:
- https://{domain}.sana.ai/api/token
---
