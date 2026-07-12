---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Vanta Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vanta publishes 8 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vanta API on a user''s behalf.


  Tokens are issued from https://api.vanta.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vanta
provider_slug: vanta
schemes:
- description: Get an oauth token from the token url and use it as a bearer token to access the Vanta API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.vanta.com/oauth/token
  name: oauth
  source: openapi/vanta-auditor-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.vanta.com/oauth/token
  name: OAuth2
  source: openapi/vanta-openapi.yml
scope_count: 8
scope_names:
- auditor-api.audit:read
- auditor-api.audit:write
- auditor-api.auditor:read
- auditor-api.auditor:write
- connectors.self:read-resource
- connectors.self:write-resource
- vanta.read
- vanta.write
scopes:
- description: Grant read-only access to your audits
  flows:
  - clientCredentials
  scope: auditor-api.audit:read
- description: Grant read-write access to your audits
  flows:
  - clientCredentials
  scope: auditor-api.audit:write
- description: Grant read-only access to your auditors
  flows:
  - clientCredentials
  scope: auditor-api.auditor:read
- description: Grant read-write access to your auditors
  flows:
  - clientCredentials
  scope: auditor-api.auditor:write
- description: Read connector resources
  flows:
  - clientCredentials
  scope: connectors.self:read-resource
- description: Write connector resources
  flows:
  - clientCredentials
  scope: connectors.self:write-resource
- description: Read access to Vanta data
  flows:
  - clientCredentials
  scope: vanta.read
- description: Write access to Vanta data
  flows:
  - clientCredentials
  scope: vanta.write
slug: vanta-scopes
source_filename: vanta-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vanta-auditor-openapi.yml, openapi/vanta-openapi.yml\nschemes:\n- name: oauth\n  source: openapi/vanta-auditor-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.vanta.com/oauth/token\n  description: Get an oauth token from the token url and use it as a bearer token to access\n    the Vanta API.\n- name: OAuth2\n  source: openapi/vanta-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.vanta.com/oauth/token\nscopes:\n- scope: auditor-api.audit:read\n  description: Grant read-only access to your audits\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/vanta-auditor-openapi.yml\n  - openapi/vanta-openapi.yml\n- scope: auditor-api.audit:write\n  description: Grant read-write access to your audits\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/vanta-auditor-openapi.yml\n- scope: auditor-api.auditor:read\n  description: Grant read-only access to your\
  \ auditors\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/vanta-auditor-openapi.yml\n  - openapi/vanta-openapi.yml\n- scope: auditor-api.auditor:write\n  description: Grant read-write access to your auditors\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/vanta-auditor-openapi.yml\n- scope: connectors.self:read-resource\n  description: Read connector resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/vanta-openapi.yml\n- scope: connectors.self:write-resource\n  description: Write connector resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/vanta-openapi.yml\n- scope: vanta.read\n  description: Read access to Vanta data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/vanta-openapi.yml\n- scope: vanta.write\n  description: Write access to Vanta data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/vanta-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/scopes/vanta-scopes.yml
summary_line: 8 scopes · clientCredentials
tags:
- Cybersecurity
- Compliance
- Security
- Governance
- Risk Management
token_urls:
- https://api.vanta.com/oauth/token
---
