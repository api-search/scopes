---
api_specs:
- filename: accredify0604-nexus-auth-openapi.yaml
  format: yaml
  label: Accredify Nexus API
  slug: accredify0604-nexus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/openapi/accredify0604-nexus-auth-openapi.yaml
- filename: accredify0604-dashboard-v1-openapi.yaml
  format: yaml
  label: Accredify Dashboard API
  slug: accredify0604-dashboard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/openapi/accredify0604-dashboard-v1-openapi.yaml
authorization_urls: []
description: ''
docs: https://docs.nexus.accredify.io/auth.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Accredify0604 Scopes
name_suffix: OAuth Scopes
note: 'The 20 scopes below are published verbatim by Accredify in two places that agree: the components.securitySchemes.OAuth2 clientCredentials block of the Nexus specs, and a scope/permission table rendered in the description of POST /oauth/token. Accredify has no separate scopes reference page; the specification IS the reference. The Accredify Dashboard API declares no scopes at all — it uses an unscoped bearer JWT — so this file covers the Nexus family only. The provider instructs: "Request only the scopes required by your integration, separated by spaces."'
overview: 'Accredify publishes 20 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Accredify API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Accredify
provider_slug: accredify0604
schemes:
- description: OAuth2 client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/accredify0604-nexus-auth-openapi.yaml
- description: OAuth2 client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/accredify0604-nexus-verification-openapi.yaml
- description: OAuth2 client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/accredify0604-nexus-workflow-openapi.yaml
scope_count: 20
scope_names:
- courses:read
- courses:write
- custom-views:read
- design-templates:read
- document-templates:read
- documents:read
- documents:write
- groups:read
- groups:write
- roles:read
- run-workflow
- user-tokens:read
- user-tokens:write
- users:read
- users:write
- verification-suite
- webcomponent-verification
- workflow-runs:read
- workflows:read
- workflows:write
scopes:
- description: Ability to read courses
  flows:
  - clientCredentials
  scope: courses:read
- description: Ability to write courses
  flows:
  - clientCredentials
  scope: courses:write
- description: Ability to read custom views
  flows:
  - clientCredentials
  scope: custom-views:read
- description: Ability to read design templates
  flows:
  - clientCredentials
  scope: design-templates:read
- description: Ability to read document templates
  flows:
  - clientCredentials
  scope: document-templates:read
- description: Ability to read documents
  flows:
  - clientCredentials
  scope: documents:read
- description: Ability to write documents
  flows:
  - clientCredentials
  scope: documents:write
- description: Ability to read groups
  flows:
  - clientCredentials
  scope: groups:read
- description: Ability to write groups
  flows:
  - clientCredentials
  scope: groups:write
- description: Ability to read roles
  flows:
  - clientCredentials
  scope: roles:read
- description: Ability to run a specific workflow
  flows:
  - clientCredentials
  scope: run-workflow
- description: Ability to read user tokens
  flows:
  - clientCredentials
  scope: user-tokens:read
- description: Ability to write user tokens
  flows:
  - clientCredentials
  scope: user-tokens:write
- description: Ability to read users
  flows:
  - clientCredentials
  scope: users:read
- description: Ability to write users
  flows:
  - clientCredentials
  scope: users:write
- description: Ability to access the verification suite APIs
  flows:
  - clientCredentials
  scope: verification-suite
- description: Ability to get the verification access from webcomponent
  flows:
  - clientCredentials
  scope: webcomponent-verification
- description: Ability to read workflow runs
  flows:
  - clientCredentials
  scope: workflow-runs:read
- description: Ability to read workflows
  flows:
  - clientCredentials
  scope: workflows:read
- description: Ability to write workflows
  flows:
  - clientCredentials
  scope: workflows:write
slug: accredify0604-scopes
source_filename: accredify0604-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://docs.nexus.accredify.io/auth.yaml, https://docs.nexus.accredify.io/workflow.yaml, https://docs.nexus.accredify.io/verification.yaml\n  (fetched 2026-09-06); mirrored to openapi/accredify0604-nexus-auth-openapi.yaml, openapi/accredify0604-nexus-workflow-openapi.yaml,\n  openapi/accredify0604-nexus-verification-openapi.yaml\ndocs: https://docs.nexus.accredify.io/auth.html\nnote: 'The 20 scopes below are published verbatim by Accredify in two places that agree: the components.securitySchemes.OAuth2\n  clientCredentials block of the Nexus specs, and a scope/permission table rendered in the description\n  of POST /oauth/token. Accredify has no separate scopes reference page; the specification IS the reference.\n  The Accredify Dashboard API declares no scopes at all — it uses an unscoped bearer JWT — so this file\n  covers the Nexus family only. The provider instructs: \"Request only the scopes required by your integration,\n\
  \  separated by spaces.\"'\napplies_to:\n- Accredify Nexus API\nnot_applicable:\n- api: Accredify Dashboard API\n  reason: bearer JWT with no declared scopes (components.securitySchemes.bearerAuth)\nscope_count: 20\nschemes:\n- name: OAuth2\n  source: openapi/accredify0604-nexus-auth-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  description: OAuth2 client credentials flow\n- name: OAuth2\n  source: openapi/accredify0604-nexus-verification-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  description: OAuth2 client credentials flow\n- name: OAuth2\n  source: openapi/accredify0604-nexus-workflow-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  description: OAuth2 client credentials flow\nscopes:\n- scope: courses:read\n  description: Ability to read courses\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n\
  - scope: courses:write\n  description: Ability to write courses\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: custom-views:read\n  description: Ability to read custom views\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: design-templates:read\n  description: Ability to read design templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: document-templates:read\n  description: Ability to read document templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: documents:read\n  description: Ability to read documents\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: documents:write\n  description: Ability to write documents\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: groups:read\n  description: Ability to read groups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: groups:write\n  description: Ability to write groups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n- scope: roles:read\n  description: Ability to read roles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n- scope: run-workflow\n  description: Ability to run a specific workflow\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n\
  \  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: user-tokens:read\n  description: Ability to read user tokens\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n- scope: user-tokens:write\n  description: Ability to write user tokens\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n- scope: users:read\n  description: Ability to read users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: users:write\n  description: Ability to write users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n- scope: verification-suite\n  description: Ability to access the verification suite APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-verification-openapi.yaml\n\
  \  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: webcomponent-verification\n  description: Ability to get the verification access from webcomponent\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: workflow-runs:read\n  description: Ability to read workflow runs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: workflows:read\n  description: Ability to read workflows\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n- scope: workflows:write\n  description: Ability to write workflows\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/accredify0604-nexus-auth-openapi.yaml\n  - openapi/accredify0604-nexus-workflow-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/scopes/accredify0604-scopes.yml
summary_line: 20 scopes · clientCredentials
tags:
- Company
- Verifiable Credentials
- Digital Credentials
- Identity
- Document Verification
- Credentialing
- Education
- Healthcare
- Trust
- OpenBadges
- OID4VCI
- Singapore
token_urls:
- /oauth/token
---
