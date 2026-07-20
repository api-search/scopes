---
api_specs:
- filename: fingoal-insights-openapi-original.json
  format: json
  label: FinGoal Insights API
  slug: fingoal-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/openapi/fingoal-insights-openapi-original.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Fingoal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FinGoal publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the FinGoal API on a user''s behalf.


  Tokens are issued from https://findmoney.fingoal.com/v3/authentication.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FinGoal
provider_slug: fingoal
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://findmoney.fingoal.com/v3/authentication
  name: Authentication
  source: openapi/fingoal-insights-openapi-original.json
scope_count: 3
scope_names:
- calls_to_action
- enrichment
- read
scopes:
- description: Required (with `enrichment`) by GET /users/{userId}/sync to trigger a user tag update / calls-to-action refresh. No standalone description is published in the spec; derived from operation security requirements.
  flows: []
  scope: calls_to_action
- description: Grants access to the transaction enrichment APIs.
  flows:
  - clientCredentials
  scope: enrichment
- description: Read access to user data. Required by GET /users/{userId} and GET /users/tags/{guid}. No standalone description is published in the spec; derived from operation security requirements.
  flows: []
  scope: read
slug: fingoal-scopes
source_filename: fingoal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/fingoal-insights-openapi-original.json\nschemes:\n- name: Authentication\n  source: openapi/fingoal-insights-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://findmoney.fingoal.com/v3/authentication\nscopes:\n- scope: calls_to_action\n  description: >-\n    Required (with `enrichment`) by GET /users/{userId}/sync to trigger a user\n    tag update / calls-to-action refresh. No standalone description is published\n    in the spec; derived from operation security requirements.\n  used_by:\n  - getOneUserSync\n  sources:\n  - openapi/fingoal-insights-openapi-original.json\n- scope: enrichment\n  description: Grants access to the transaction enrichment APIs.\n  flows:\n  - clientCredentials\n  used_by:\n  - syncCleanupTransactions\n  - asyncCleanupTransactions\n  - streamingCleanupTransactions\n  - baseCleanupTransactions\n  - getEnrichment\n  - getOneUserSync\n  - listWebhookConfigurations\n\
  \  - upsertWebhookConfiguration\n  - deleteWebhookConfiguration\n  - testWebhook\n  sources:\n  - openapi/fingoal-insights-openapi-original.json\n- scope: read\n  description: >-\n    Read access to user data. Required by GET /users/{userId} and\n    GET /users/tags/{guid}. No standalone description is published in the spec;\n    derived from operation security requirements.\n  used_by:\n  - getOneUser\n  - getUserTagUpdates\n  sources:\n  - openapi/fingoal-insights-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/scopes/fingoal-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Financial Services
- Fintech
- Transaction Enrichment
- Data Enrichment
- Personal Financial Management
- Banking
- Categorization
- Webhooks
token_urls:
- https://findmoney.fingoal.com/v3/authentication
---
