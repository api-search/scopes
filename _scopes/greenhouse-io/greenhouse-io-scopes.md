---
authorization_urls:
- https://app.greenhouse.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Greenhouse Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Greenhouse publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Greenhouse API on a user''s behalf.


  Tokens are issued from https://app.greenhouse.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Greenhouse
provider_slug: greenhouse-io
schemes:
- flows:
  - authorizationUrl: https://app.greenhouse.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.greenhouse.io/oauth/token
  - flow: clientCredentials
    tokenUrl: https://app.greenhouse.io/oauth/token
  name: OAuth2
  source: openapi/greenhouse-candidate-ingestion-api-openapi.yml
scope_count: 1
scope_names:
- partner
scopes:
- description: Partner integration scope.
  flows:
  - authorizationCode
  - clientCredentials
  scope: partner
slug: greenhouse-io-scopes
source_filename: greenhouse-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/greenhouse-candidate-ingestion-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/greenhouse-candidate-ingestion-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.greenhouse.io/oauth/authorize\n    tokenUrl: https://app.greenhouse.io/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://app.greenhouse.io/oauth/token\nscopes:\n- scope: partner\n  description: Partner integration scope.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/greenhouse-candidate-ingestion-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenhouse-io/refs/heads/main/scopes/greenhouse-io-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- ATS
- Recruiting
- Hiring
- Talent Acquisition
- Enterprise SaaS
- Human Resources
- Onboarding
token_urls:
- https://app.greenhouse.io/oauth/token
---
