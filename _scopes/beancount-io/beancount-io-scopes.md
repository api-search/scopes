---
api_specs:
- filename: beancount-io-ledger-api-openapi.yml
  format: yaml
  label: Beancount.io Ledger API
  slug: beancount-io-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beancount-io/openapi/beancount-io-ledger-api-openapi.yml
- filename: beancount-io-mcp-api-openapi.yml
  format: yaml
  label: Beancount.io MCP API
  slug: beancount-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beancount-io/openapi/beancount-io-mcp-api-openapi.yml
- filename: beancount-io-graph-ql-api-openapi.yml
  format: yaml
  label: Beancount.io Graph QL API
  slug: beancount-io-graph-ql-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beancount-io/openapi/beancount-io-graph-ql-api-openapi.yml
authorization_urls:
- https://beancount.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Beancount Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Beancount.io publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Beancount.io API on a user''s behalf.


  Tokens are issued from https://beancount.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beancount.io
provider_slug: beancount-io
schemes:
- description: OAuth 2.1 with PKCE for MCP and GraphQL. Scopes enforce least privilege.
  flows:
  - authorizationUrl: https://beancount.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://beancount.io/oauth/token
  - flow: clientCredentials
    tokenUrl: https://beancount.io/oauth/token
  name: OAuth2
  source: openapi/beancount-io-openapi.json
scope_count: 3
scope_names:
- admin
- read
- write
scopes:
- description: Full administrative access
  flows:
  - authorizationCode
  scope: admin
- description: Read ledgers, queries, and content
  flows:
  - authorizationCode
  - clientCredentials
  scope: read
- description: Edit ledgers and commit changes
  flows:
  - authorizationCode
  - clientCredentials
  scope: write
slug: beancount-io-scopes
source_filename: beancount-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/beancount-io-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/beancount-io-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://beancount.io/oauth/authorize\n    tokenUrl: https://beancount.io/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://beancount.io/oauth/token\n  description: OAuth 2.1 with PKCE for MCP and GraphQL. Scopes enforce least privilege.\nscopes:\n- scope: admin\n  description: Full administrative access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/beancount-io-openapi.json\n- scope: read\n  description: Read ledgers, queries, and content\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/beancount-io-openapi.json\n- scope: write\n  description: Edit ledgers and commit changes\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/beancount-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/beancount-io/scopes/beancount-io-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Accounting
- Finance
- Software-as-a-Service
- Open Source
- Collaboration
token_bound: false
token_urls:
- https://beancount.io/oauth/token
---
