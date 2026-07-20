---
api_specs:
- filename: calm-partner-api-openapi.yml
  format: yaml
  label: Calm Partner API
  slug: calm-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calm/refs/heads/main/openapi/calm-partner-api-openapi.yml
authorization_urls: []
description: ''
docs: https://partner.calm.com/docs/api
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Calm Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Calm publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Calm API on a user''s behalf.


  Tokens are issued from https://auth.calm.com/v0/authorize.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Calm
provider_slug: calm
schemes:
- description: OAuth 2.0 client-credentials grant against the Calm auth service.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.calm.com/v0/authorize
  name: CalmOAuth2
  source: openapi/calm-partner-api-openapi.yml
scope_count: 2
scope_names:
- b2b.subscription.cancel
- b2b.users.integrate
scopes:
- description: Cancel partner-user Calm subscriptions.
  flows:
  - clientCredentials
  scope: b2b.subscription.cancel
- description: Provision and link partner users to Calm subscriptions.
  flows:
  - clientCredentials
  scope: b2b.users.integrate
slug: calm-scopes
source_filename: calm-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/calm-partner-api-openapi.yml\ndocs: https://partner.calm.com/docs/api\nnotes: >-\n  The Partner API documents a single comma-delimited scope string\n  \"b2b.users.integrate,b2b.subscription.cancel\" requested at the /v0/authorize\n  client-credentials endpoint.\nschemes:\n- name: CalmOAuth2\n  source: openapi/calm-partner-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.calm.com/v0/authorize\n  description: OAuth 2.0 client-credentials grant against the Calm auth service.\nscopes:\n- scope: b2b.subscription.cancel\n  description: Cancel partner-user Calm subscriptions.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/calm-partner-api-openapi.yml\n- scope: b2b.users.integrate\n  description: Provision and link partner users to Calm subscriptions.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/calm-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calm/refs/heads/main/scopes/calm-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Mental Health
- Wellness
- Meditation
- Mindfulness
- Sleep
- Employee Benefits
- Health
- B2B
- Subscriptions
token_urls:
- https://auth.calm.com/v0/authorize
---
