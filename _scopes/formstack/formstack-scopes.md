---
api_specs:
- filename: formstack-asyncapi.yml
  format: yaml
  label: Formstack Webhooks API
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/openapi/formstack-asyncapi.yml
authorization_urls:
- https://www.formstack.com/api/v2/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Formstack Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Formstack publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Formstack API on a user''s behalf.


  Tokens are issued from https://www.formstack.com/api/v2/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Formstack
provider_slug: formstack
schemes:
- description: OAuth 2.0 authorization code flow.
  flows:
  - authorizationUrl: https://www.formstack.com/api/v2/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.formstack.com/api/v2/oauth2/token
  name: oauth2
  source: openapi/formstack-openapi.yml
scope_count: 4
scope_names:
- forms_read
- forms_write
- submissions_read
- submissions_write
scopes:
- description: Read forms
  flows:
  - authorizationCode
  scope: forms_read
- description: Manage forms
  flows:
  - authorizationCode
  scope: forms_write
- description: Read submissions
  flows:
  - authorizationCode
  scope: submissions_read
- description: Manage submissions
  flows:
  - authorizationCode
  scope: submissions_write
slug: formstack-scopes
source_filename: formstack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/formstack-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/formstack-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.formstack.com/api/v2/oauth2/authorize\n    tokenUrl: https://www.formstack.com/api/v2/oauth2/token\n  description: OAuth 2.0 authorization code flow.\nscopes:\n- scope: forms_read\n  description: Read forms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formstack-openapi.yml\n- scope: forms_write\n  description: Manage forms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formstack-openapi.yml\n- scope: submissions_read\n  description: Read submissions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formstack-openapi.yml\n- scope: submissions_write\n  description: Manage submissions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/formstack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/scopes/formstack-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Forms
- Documents
- eSignature
- Workflow Automation
- No-Code
- OAuth2
token_urls:
- https://www.formstack.com/api/v2/oauth2/token
---
