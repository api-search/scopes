---
api_specs:
- filename: total-expert-account-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Account Endpoints API
  slug: total-expert-account-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-account-endpoints-api-openapi.yml
- filename: total-expert-activity-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Activity Endpoints API
  slug: total-expert-activity-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-activity-endpoints-api-openapi.yml
- filename: total-expert-alm-leads-formerly-lead-opportunities-api-openapi.yml
  format: yaml
  label: Total Expert ALM Leads (formerly Lead Opportunities) API
  slug: total-expert-alm-leads-formerly-lead-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-alm-leads-formerly-lead-opportunities-api-openapi.yml
- filename: total-expert-authentication-api-openapi.yml
  format: yaml
  label: Total Expert Authentication API
  slug: total-expert-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-authentication-api-openapi.yml
- filename: total-expert-contact-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Contact Endpoints API
  slug: total-expert-contact-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-contact-endpoints-api-openapi.yml
- filename: total-expert-email-apis-api-openapi.yml
  format: yaml
  label: Total Expert Email APIs API
  slug: total-expert-email-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-email-apis-api-openapi.yml
- filename: total-expert-email-unsubscribes-api-openapi.yml
  format: yaml
  label: Total Expert Email Unsubscribes API
  slug: total-expert-email-unsubscribes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-email-unsubscribes-api-openapi.yml
- filename: total-expert-entities-api-openapi.yml
  format: yaml
  label: Total Expert Entities API
  slug: total-expert-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-entities-api-openapi.yml
- filename: total-expert-heartbeat-api-openapi.yml
  format: yaml
  label: Total Expert Heartbeat API
  slug: total-expert-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-heartbeat-api-openapi.yml
- filename: total-expert-insight-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Insight Endpoints API
  slug: total-expert-insight-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-insight-endpoints-api-openapi.yml
- filename: total-expert-lead-opportunities-new-api-openapi.yml
  format: yaml
  label: Total Expert Lead Opportunities (New) API
  slug: total-expert-lead-opportunities-new-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-lead-opportunities-new-api-openapi.yml
- filename: total-expert-loan-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Loan Endpoints API
  slug: total-expert-loan-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-loan-endpoints-api-openapi.yml
- filename: total-expert-scenarios-api-openapi.yml
  format: yaml
  label: Total Expert Scenarios API
  slug: total-expert-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-scenarios-api-openapi.yml
- filename: total-expert-schema-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert Schema Endpoints API
  slug: total-expert-schema-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-schema-endpoints-api-openapi.yml
- filename: total-expert-sms-opting-api-openapi.yml
  format: yaml
  label: Total Expert SMS Opting API
  slug: total-expert-sms-opting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-sms-opting-api-openapi.yml
- filename: total-expert-user-endpoints-api-openapi.yml
  format: yaml
  label: Total Expert User Endpoints API
  slug: total-expert-user-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-user-endpoints-api-openapi.yml
- filename: total-expert-webhooks-api-openapi.yml
  format: yaml
  label: Total Expert Webhooks API
  slug: total-expert-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-expert/refs/heads/main/openapi/total-expert-webhooks-api-openapi.yml
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
