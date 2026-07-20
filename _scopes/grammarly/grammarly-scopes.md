---
authorization_urls: []
description: ''
docs: https://developer.grammarly.com/oauth-credentials.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Grammarly Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Grammarly publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Grammarly API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Grammarly
provider_slug: grammarly
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  token_url: https://auth.grammarly.com/v4/api/oauth2/token
scope_count: 5
scope_names:
- scores-api:read
- scores-api:write
- analytics-api:read
- users-api:read
- users-api:write
scopes:
- description: Read-only access to the Writing Score API.
  flows: []
  scope: scores-api:read
- description: Write access to the Writing Score API.
  flows: []
  scope: scores-api:write
- description: Read-only access to the Analytics API (usage and communication statistics).
  flows: []
  scope: analytics-api:read
- description: Read-only access to the License Management API.
  flows: []
  scope: users-api:read
- description: Write access to the License Management API (license allocation/reallocation).
  flows: []
  scope: users-api:write
slug: grammarly-scopes
source_filename: grammarly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.grammarly.com/oauth-credentials.html\ndocs: https://developer.grammarly.com/oauth-credentials.html\nschemes:\n- name: OAuth2ClientCredentials\n  flow: clientCredentials\n  token_url: https://auth.grammarly.com/v4/api/oauth2/token\nscopes:\n- scope: scores-api:read\n  description: Read-only access to the Writing Score API.\n  api: Writing Score API\n- scope: scores-api:write\n  description: Write access to the Writing Score API.\n  api: Writing Score API\n- scope: analytics-api:read\n  description: Read-only access to the Analytics API (usage and communication statistics).\n  api: Analytics API\n- scope: users-api:read\n  description: Read-only access to the License Management API.\n  api: License Management API\n- scope: users-api:write\n  description: Write access to the License Management API (license allocation/reallocation).\n  api: License Management API\nnotes: >-\n  Scopes are assigned to each OAuth\
  \ 2.0 credential in the Grammarly Admin panel\n  and requested via the `scope` parameter of the client-credentials token\n  request. The Beta AI Detection and Plagiarism Detection APIs did not publish\n  dedicated scope names on the credentials page at capture time.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grammarly/refs/heads/main/scopes/grammarly-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Ai
- Writing Assistance
- Productivity
- Natural Language Processing
- Analytics
- Content
- OAuth
- Enterprise
token_urls: []
---
