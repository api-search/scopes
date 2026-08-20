---
api_specs:
- filename: opal-v2-openapi.yml
  format: yaml
  label: Opal API v2
  slug: opal-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/openapi/opal-v2-openapi.yml
- filename: opal-v3-openapi.yml
  format: yaml
  label: Opal API v3
  slug: opal-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/openapi/opal-v3-openapi.yml
- filename: opal-asgard-bff-openapi.yml
  format: yaml
  label: Opal Asgard BFF API
  slug: opal-asgard-bff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/openapi/opal-asgard-bff-openapi.yml
authorization_urls:
- /oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Opal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Opal publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Opal API on a user''s behalf.


  Tokens are issued from /oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Opal
provider_slug: opal
schemes:
- description: This API uses OAuth 2.0 with the authorization code grant flow. You can find more detailed authentication instructions in the [Authentication Strategies](/api/documentation#section/Authentication-Strategies/OAuth-2.0) section.
  flows:
  - authorizationUrl: /oauth2/auth
    flow: authorizationCode
    tokenUrl: /oauth2/token
  name: oauth2
  source: openapi/opal-v2-openapi.yml
- description: 'This API uses OAuth 2.0 with the authorization code grant flow. You can

    find more detailed authentication instructions in the [Authentication

    Strategies](/api/documentation#section/Authentication-Strategies/OAuth-2.0)

    section.'
  flows:
  - authorizationUrl: /oauth2/auth
    flow: authorizationCode
    tokenUrl: /oauth2/token
  name: oauth2
  source: openapi/opal-v3-openapi.yml
- description: 'The OAuth 2.0 client credentials flow is used for secure server-server

    requests when Opal does not need to associate a request with a particular

    Opal user. These anonymous requests are instead authorized based on the

    OAuth scope.'
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: anonymous_oauth
  source: openapi/opal-v3-openapi.yml
scope_count: 2
scope_names:
- offline_access
- write:onboarding
scopes:
- description: Include this scope if you wish to receive a refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: Include this scope if you wish to make API requests to onboard new Opals.
  flows:
  - clientCredentials
  scope: write:onboarding
slug: opal-scopes
source_filename: opal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/opal-v2-openapi.yml, openapi/opal-v3-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/opal-v2-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/auth\n    tokenUrl: /oauth2/token\n  description: This API uses OAuth 2.0 with the authorization code grant flow. You can find\n    more detailed authentication instructions in the [Authentication Strategies](/api/documentation#section/Authentication-Strategies/OAuth-2.0)\n    section.\n- name: oauth2\n  source: openapi/opal-v3-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/auth\n    tokenUrl: /oauth2/token\n  description: |-\n    This API uses OAuth 2.0 with the authorization code grant flow. You can\n    find more detailed authentication instructions in the [Authentication\n    Strategies](/api/documentation#section/Authentication-Strategies/OAuth-2.0)\n    section.\n- name: anonymous_oauth\n  source:\
  \ openapi/opal-v3-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  description: |-\n    The OAuth 2.0 client credentials flow is used for secure server-server\n    requests when Opal does not need to associate a request with a particular\n    Opal user. These anonymous requests are instead authorized based on the\n    OAuth scope.\nscopes:\n- scope: offline_access\n  description: Include this scope if you wish to receive a refresh token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/opal-v2-openapi.yml\n  - openapi/opal-v3-openapi.yml\n- scope: write:onboarding\n  description: Include this scope if you wish to make API requests to onboard new Opals.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/opal-v3-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/scopes/opal-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Company
- Consumer
- Marketing
- Content Planning
- Marketing Calendar
- Campaign Management
- Collaboration
- Software-as-a-Service
- Content Marketing
- Editorial Calendar
- Workflows
- Approvals
- Digital Asset Management
- JSON:API
- Authentication
- OpenAPI
token_urls:
- /oauth2/token
- /oauth/token
---
