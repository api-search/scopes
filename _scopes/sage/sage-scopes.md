---
api_specs:
- filename: sage-accounting-openapi.yml
  format: yaml
  label: Sage Accounting API
  slug: accounting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/openapi/sage-accounting-openapi.yml
authorization_urls:
- https://www.sageone.com/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Sage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sage publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sage API on a user''s behalf.


  Tokens are issued from https://oauth.accounting.sage.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sage
provider_slug: sage
schemes:
- flows:
  - authorizationUrl: https://www.sageone.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth.accounting.sage.com/token
  name: OAuth2
  source: openapi/sage-accounting-openapi.yml
scope_count: 2
scope_names:
- full_access
- readonly
scopes:
- description: Full read/write access to all accounting data
  flows:
  - authorizationCode
  scope: full_access
- description: Read-only access to accounting data
  flows:
  - authorizationCode
  scope: readonly
slug: sage-scopes
source_filename: sage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sage-accounting-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/sage-accounting-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.sageone.com/oauth2/auth\n    tokenUrl: https://oauth.accounting.sage.com/token\nscopes:\n- scope: full_access\n  description: Full read/write access to all accounting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sage-accounting-openapi.yml\n- scope: readonly\n  description: Read-only access to accounting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sage-accounting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/scopes/sage-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Accounting
- Business Management
- Cloud Software
- ERP
- Payroll
- HR
token_urls:
- https://oauth.accounting.sage.com/token
---
