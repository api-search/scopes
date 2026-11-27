---
api_specs:
- filename: synci-io-openapi-generated.yml
  format: yaml
  label: Synci API
  slug: synci-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synci-io/openapi/_ae-authored/synci-io-openapi-generated.yml
authorization_urls:
- https://api.synci.io/oauth/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Synci Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Synci publishes 16 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Synci API on a user''s behalf.


  Tokens are issued from https://api.synci.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Synci
provider_slug: synci-io
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.synci.io/oauth/token
  - authorizationUrl: https://api.synci.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.synci.io/oauth/token
  name: OAuth_2.0_authorization_code_grant_with_PKCE
  source: openapi/synci-io-openapi-generated.yml
scope_count: 16
scope_names:
- accounts:read
- accounts:write
- destinations:read
- destinations:write
- financial-connections:read
- financial-connections:write
- profile:read
- rules:read
- rules:write
- sensitive:read
- transactions:read
- transactions:write
- transfer-links:read
- transfer-links:write
- webhooks:read
- webhooks:write
scopes:
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts:write
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: destinations:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: destinations:write
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: financial-connections:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: financial-connections:write
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: profile:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: rules:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: rules:write
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: sensitive:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: transactions:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: transactions:write
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: transfer-links:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: transfer-links:write
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhooks:read
- description: ''
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhooks:write
slug: synci-io-scopes
source_filename: synci-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: derived\nsource: openapi/synci-io-openapi-generated.yml\nschemes:\n- name: OAuth_2.0_authorization_code_grant_with_PKCE\n  source: openapi/synci-io-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.synci.io/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.synci.io/oauth/authorize\n    tokenUrl: https://api.synci.io/oauth/token\nscopes:\n- scope: accounts:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: accounts:write\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: destinations:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: destinations:write\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n\
  - scope: financial-connections:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: financial-connections:write\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: profile:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: rules:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: rules:write\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: sensitive:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: transactions:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: transactions:write\n\
  \  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: transfer-links:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: transfer-links:write\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: webhooks:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n- scope: webhooks:write\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/synci-io-openapi-generated.yml\n"
source_yaml_url: https://artifacts.apis.io/synci-io/scopes/synci-io-scopes.yml
summary_line: 16 scopes · clientCredentials/authorizationCode
tags:
- Company
- Banking
- AI
- Finance
- Integration
token_bound: false
token_urls:
- https://api.synci.io/oauth/token
---
