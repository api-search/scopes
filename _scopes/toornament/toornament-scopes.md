---
api_specs:
- filename: toornament-disciplines-api-openapi.yml
  format: yaml
  label: Toornament Disciplines API
  slug: toornament-disciplines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-disciplines-api-openapi.yml
- filename: toornament-matches-api-openapi.yml
  format: yaml
  label: Toornament Matches API
  slug: toornament-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-matches-api-openapi.yml
- filename: toornament-participants-api-openapi.yml
  format: yaml
  label: Toornament Participants API
  slug: toornament-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-participants-api-openapi.yml
- filename: toornament-rankings-api-openapi.yml
  format: yaml
  label: Toornament Rankings API
  slug: toornament-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-rankings-api-openapi.yml
- filename: toornament-registrations-api-openapi.yml
  format: yaml
  label: Toornament Registrations API
  slug: toornament-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-registrations-api-openapi.yml
- filename: toornament-stages-api-openapi.yml
  format: yaml
  label: Toornament Stages API
  slug: toornament-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-stages-api-openapi.yml
- filename: toornament-tournaments-api-openapi.yml
  format: yaml
  label: Toornament Tournaments API
  slug: toornament-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-tournaments-api-openapi.yml
- filename: toornament-webhooks-api-openapi.yml
  format: yaml
  label: Toornament Webhooks API
  slug: toornament-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-webhooks-api-openapi.yml
authorization_urls:
- https://app.toornament.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Toornament Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Toornament publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Toornament API on a user''s behalf.


  Tokens are issued from https://api.toornament.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Toornament
provider_slug: toornament
schemes:
- description: OAuth2 access token with scoped permissions (organizer:view, organizer:admin).
  flows:
  - authorizationUrl: https://app.toornament.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.toornament.com/oauth/v2/token
  name: oauth2
  source: openapi/toornament-openapi.yml
scope_count: 3
scope_names:
- organizer:admin
- organizer:view
- participant:manage
scopes:
- description: Full administrative access to tournament management.
  flows:
  - authorizationCode
  scope: organizer:admin
- description: Read access to organizer tournament data.
  flows:
  - authorizationCode
  scope: organizer:view
- description: Manage participant registrations.
  flows:
  - authorizationCode
  scope: participant:manage
slug: toornament-scopes
source_filename: toornament-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/toornament-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/toornament-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.toornament.com/oauth/authorize\n    tokenUrl: https://api.toornament.com/oauth/v2/token\n  description: OAuth2 access token with scoped permissions (organizer:view, organizer:admin).\nscopes:\n- scope: organizer:admin\n  description: Full administrative access to tournament management.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/toornament-openapi.yml\n- scope: organizer:view\n  description: Read access to organizer tournament data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/toornament-openapi.yml\n- scope: participant:manage\n  description: Manage participant registrations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/toornament-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/scopes/toornament-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Esports
- Gaming
- Tournaments
- Brackets
- Competition
token_urls:
- https://api.toornament.com/oauth/v2/token
---
