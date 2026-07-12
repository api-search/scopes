---
authorization_urls:
- /OAuth/Authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Practicepanther Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PracticePanther publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PracticePanther API on a user''s behalf.


  Tokens are issued from /OAuth/Token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PracticePanther
provider_slug: practicepanther
schemes:
- description: OAuth 2.0 - Authorization Code Grant
  flows:
  - authorizationUrl: /OAuth/Authorize
    flow: authorizationCode
    tokenUrl: /OAuth/Token
  name: oauth2
  source: openapi/practicepanther-practicepanther-api-openapi.yml
scope_count: 1
scope_names:
- full
scopes:
- description: Read/Write access to all resources
  flows:
  - authorizationCode
  scope: full
slug: practicepanther-scopes
source_filename: practicepanther-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/practicepanther-practicepanther-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/practicepanther-practicepanther-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /OAuth/Authorize\n    tokenUrl: /OAuth/Token\n  description: OAuth 2.0 - Authorization Code Grant\nscopes:\n- scope: full\n  description: Read/Write access to all resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/practicepanther-practicepanther-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/practicepanther/refs/heads/main/scopes/practicepanther-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Legal
- Law Practice Management
- Case Management
- Billing
- Trust Accounting
- Time Tracking
- Legal Tech
token_urls:
- /OAuth/Token
---
