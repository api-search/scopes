---
api_specs:
- filename: total-expert-openapi.yml
  format: yaml
  label: Total Expert Public API
  slug: total-expert-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-openapi.yml
authorization_urls:
- https://public.totalexpert.net/v1/authorize
description: ''
docs: https://public.totalexpert.net/v1/docs/OAuth+Authorization+Guide.pdf
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Total Expert Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Total Expert publishes 5 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Total Expert API on a user''s behalf.


  Tokens are issued from https://public.totalexpert.net/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Total Expert
provider_slug: total-expert
schemes:
- description: OAuth 2.0. Obtain a token from POST /v1/token using HTTP Basic (client_id:client_secret base64-encoded) plus a grant_type body. Access tokens are bearer tokens, expires_in 3600.
  flows:
  - flow: clientCredentials
    tokenUrl: https://public.totalexpert.net/v1/token
  - authorizationUrl: https://public.totalexpert.net/v1/authorize
    flow: authorizationCode
    tokenUrl: https://public.totalexpert.net/v1/token
  name: oauth2
  source: openapi/total-expert-openapi.yml
scope_count: 5
scope_names:
- crm
- leadInteraction
- leadSurveyInteraction
- loanInteraction
- postLeads
scopes:
- description: Documented example scope (Vendor OAuth Integration Guide authorize example)
  flows:
  - authorizationCode
  - clientCredentials
  scope: crm
- description: Lead interaction access (documented in the collection token examples)
  flows:
  - authorizationCode
  - clientCredentials
  scope: leadInteraction
- description: Lead survey interaction access (documented example in the Vendor OAuth Integration Guide)
  flows:
  - authorizationCode
  - clientCredentials
  scope: leadSurveyInteraction
- description: Loan interaction access (documented in the collection token examples)
  flows:
  - authorizationCode
  - clientCredentials
  scope: loanInteraction
- description: Post leads access (documented example in the Vendor OAuth Integration Guide)
  flows:
  - authorizationCode
  - clientCredentials
  scope: postLeads
slug: total-expert-scopes
source_filename: total-expert-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/total-expert-openapi.yml\ndocs: https://public.totalexpert.net/v1/docs/OAuth+Authorization+Guide.pdf\nnotes: >-\n  Total Expert does not publish a full scope registry. The /v1/authorize\n  endpoint takes a required space-delimited `scope` parameter, and the token\n  response echoes the granted `scope` list. The scope strings below are the\n  ones the provider documents: crm, leadSurveyInteraction and postLeads appear\n  in the Vendor OAuth Integration Guide examples; leadInteraction and\n  loanInteraction appear in the Postman collection token examples. Integrations\n  are provisioned scopes per client by Total Expert.\nschemes:\n- name: oauth2\n  source: openapi/total-expert-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://public.totalexpert.net/v1/token\n  - flow: authorizationCode\n    authorizationUrl: https://public.totalexpert.net/v1/authorize\n    tokenUrl: https://public.totalexpert.net/v1/token\n\
  \  description: OAuth 2.0. Obtain a token from POST /v1/token using HTTP Basic (client_id:client_secret\n    base64-encoded) plus a grant_type body. Access tokens are bearer tokens, expires_in 3600.\nscopes:\n- scope: crm\n  description: Documented example scope (Vendor OAuth Integration Guide authorize example)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/total-expert-openapi.yml\n- scope: leadInteraction\n  description: Lead interaction access (documented in the collection token examples)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/total-expert-openapi.yml\n- scope: leadSurveyInteraction\n  description: Lead survey interaction access (documented example in the Vendor OAuth Integration\n    Guide)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/total-expert-openapi.yml\n- scope: loanInteraction\n  description: Loan interaction access (documented in the collection token examples)\n\
  \  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/total-expert-openapi.yml\n- scope: postLeads\n  description: Post leads access (documented example in the Vendor OAuth Integration Guide)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/total-expert-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/scopes/total-expert-scopes.yml
summary_line: 5 scopes · clientCredentials/authorizationCode
tags:
- Company
- Fintech
- CRM
- Marketing Automation
- Mortgage
- Banking
- Lending
- Customer Engagement
token_urls:
- https://public.totalexpert.net/v1/token
---
