---
authorization_urls:
- https://console.cycloid.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Cycloid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cycloid publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cycloid API on a user''s behalf.


  Tokens are issued from https://http-api.cycloid.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cycloid
provider_slug: cycloid
schemes:
- flows:
  - authorizationUrl: https://console.cycloid.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://http-api.cycloid.io/oauth/token
  name: OAuth2
  source: openapi/cycloid-api-openapi.yml
scope_count: 2
scope_names:
- organization:read
- organization:write
scopes:
- description: Read organization data
  flows:
  - authorizationCode
  scope: organization:read
- description: Modify organization data
  flows:
  - authorizationCode
  scope: organization:write
slug: cycloid-scopes
source_filename: cycloid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cycloid-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/cycloid-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://console.cycloid.io/oauth/authorize\n    tokenUrl: https://http-api.cycloid.io/oauth/token\nscopes:\n- scope: organization:read\n  description: Read organization data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cycloid-api-openapi.yml\n- scope: organization:write\n  description: Modify organization data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cycloid-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cycloid/refs/heads/main/scopes/cycloid-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Asset Inventory
- CI/CD
- Cloud Cost Management
- Cloud Management
- Developer Experience
- DevOps
- FinOps
- GitOps
- GreenOps
- Infrastructure as Code
- Internal Developer Platform
- Internal Developer Portal
- Multi-Cloud
- Platform Engineering
- RBAC
- Self-Service
- Service Catalog
- StackForms
- Terraform
token_urls:
- https://http-api.cycloid.io/oauth/token
---
