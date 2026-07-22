---
api_specs:
- filename: orum-openapi-original.yml
  format: yaml
  label: Orum API
  slug: orum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-openapi-original.yml
authorization_urls: []
description: ''
docs: https://docs.orum.io/guides/api-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Orum Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Orum publishes 29 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Orum API on a user''s behalf.


  Tokens are issued from https://api-sandbox.orum.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Orum
provider_slug: orum
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api-sandbox.orum.io/oauth/token
  name: oauth2
  source: openapi/orum-openapi-original.yml
scope_count: 29
scope_names:
- invoke:webhook
- read:balances
- read:booktransfers
- read:businesses
- read:cards
- read:external-accounts
- read:persons
- read:reports
- read:routing-number-eligibility
- read:schedules
- read:subledgers
- read:transfer-groups
- read:transfers
- read:verify-accounts
- read:webhook-configurations
- read:webhook-secret
- write:booktransfers
- write:businesses
- write:cards
- write:external-accounts
- write:persons
- write:reports
- write:schedules
- write:subledgers
- write:transfer-groups
- write:transfers
- write:verify-accounts
- write:webhook-configurations
- write:webhook-secret
scopes:
- description: Invoke webhook
  flows:
  - clientCredentials
  scope: invoke:webhook
- description: Read balances
  flows:
  - clientCredentials
  scope: read:balances
- description: Read book transfers
  flows:
  - clientCredentials
  scope: read:booktransfers
- description: Read businesses
  flows:
  - clientCredentials
  scope: read:businesses
- description: Read cards
  flows:
  - clientCredentials
  scope: read:cards
- description: Read external accounts
  flows:
  - clientCredentials
  scope: read:external-accounts
- description: Read persons
  flows:
  - clientCredentials
  scope: read:persons
- description: Read reports
  flows:
  - clientCredentials
  scope: read:reports
- description: Read routing number eligibility
  flows:
  - clientCredentials
  scope: read:routing-number-eligibility
- description: Read schedules
  flows:
  - clientCredentials
  scope: read:schedules
- description: Read subledgers
  flows:
  - clientCredentials
  scope: read:subledgers
- description: Read transfer groups
  flows:
  - clientCredentials
  scope: read:transfer-groups
- description: Read transfers
  flows:
  - clientCredentials
  scope: read:transfers
- description: Read verify accounts
  flows:
  - clientCredentials
  scope: read:verify-accounts
- description: Read webhook configurations
  flows:
  - clientCredentials
  scope: read:webhook-configurations
- description: Read webhook secret
  flows:
  - clientCredentials
  scope: read:webhook-secret
- description: Write book transfers
  flows:
  - clientCredentials
  scope: write:booktransfers
- description: Write businesses
  flows:
  - clientCredentials
  scope: write:businesses
- description: Write cards
  flows:
  - clientCredentials
  scope: write:cards
- description: Write external accounts
  flows:
  - clientCredentials
  scope: write:external-accounts
- description: Write persons
  flows:
  - clientCredentials
  scope: write:persons
- description: Write reports
  flows:
  - clientCredentials
  scope: write:reports
- description: Write schedules
  flows:
  - clientCredentials
  scope: write:schedules
- description: Write subledgers
  flows:
  - clientCredentials
  scope: write:subledgers
- description: Write transfer groups
  flows:
  - clientCredentials
  scope: write:transfer-groups
- description: Write transfers
  flows:
  - clientCredentials
  scope: write:transfers
- description: Write verify accounts
  flows:
  - clientCredentials
  scope: write:verify-accounts
- description: Write webhook configurations
  flows:
  - clientCredentials
  scope: write:webhook-configurations
- description: Write webhook secret
  flows:
  - clientCredentials
  scope: write:webhook-secret
slug: orum-scopes
source_filename: orum-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/orum-openapi-original.yml\ndocs: https://docs.orum.io/guides/api-authentication\nschemes:\n- name: oauth2\n  source: openapi/orum-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-sandbox.orum.io/oauth/token\nscopes:\n- scope: invoke:webhook\n  description: Invoke webhook\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:balances\n  description: Read balances\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:booktransfers\n  description: Read book transfers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:businesses\n  description: Read businesses\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:cards\n  description: Read cards\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n\
  - scope: read:external-accounts\n  description: Read external accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:persons\n  description: Read persons\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:reports\n  description: Read reports\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:routing-number-eligibility\n  description: Read routing number eligibility\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:schedules\n  description: Read schedules\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:subledgers\n  description: Read subledgers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:transfer-groups\n  description: Read transfer groups\n  flows:\n  - clientCredentials\n  sources:\n  -\
  \ openapi/orum-openapi-original.yml\n- scope: read:transfers\n  description: Read transfers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:verify-accounts\n  description: Read verify accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:webhook-configurations\n  description: Read webhook configurations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: read:webhook-secret\n  description: Read webhook secret\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:booktransfers\n  description: Write book transfers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:businesses\n  description: Write businesses\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:cards\n  description: Write cards\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:external-accounts\n  description: Write external accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:persons\n  description: Write persons\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:reports\n  description: Write reports\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:schedules\n  description: Write schedules\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:subledgers\n  description: Write subledgers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:transfer-groups\n  description: Write transfer groups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:transfers\n  description: Write transfers\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:verify-accounts\n  description: Write verify accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:webhook-configurations\n  description: Write webhook configurations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n- scope: write:webhook-secret\n  description: Write webhook secret\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orum-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/scopes/orum-scopes.yml
summary_line: 29 scopes · clientCredentials
tags:
- Company
- Payments
- Fintech
- Banking
- Instant Payments
- ACH
- Money Movement
- Bank Account Verification
token_urls:
- https://api-sandbox.orum.io/oauth/token
---
