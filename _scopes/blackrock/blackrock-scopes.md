---
api_specs:
- filename: blackrock-authorizationurl-generate-api-openapi.yml
  format: yaml
  label: BlackRock Authorization Url:generate API
  slug: blackrock-authorizationurl-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-authorizationurl-generate-api-openapi.yml
- filename: blackrock-studionotifications-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications API
  slug: blackrock-studionotifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-api-openapi.yml
- filename: blackrock-studionotifications-batchcreate-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications:batch Create API
  slug: blackrock-studionotifications-batchcreate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-batchcreate-api-openapi.yml
- filename: blackrock-studionotifications-filter-api-openapi.yml
  format: yaml
  label: BlackRock Studio Notifications:filter API
  slug: blackrock-studionotifications-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studionotifications-filter-api-openapi.yml
- filename: blackrock-studiosubscriptions-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions API
  slug: blackrock-studiosubscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-api-openapi.yml
- filename: blackrock-studiosubscriptions-batchcreate-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions:batch Create API
  slug: blackrock-studiosubscriptions-batchcreate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-batchcreate-api-openapi.yml
- filename: blackrock-studiosubscriptions-filter-api-openapi.yml
  format: yaml
  label: BlackRock Studio Subscriptions:filter API
  slug: blackrock-studiosubscriptions-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-studiosubscriptions-filter-api-openapi.yml
- filename: blackrock-token-checktokenexists-api-openapi.yml
  format: yaml
  label: BlackRock Token:check Token Exists API
  slug: blackrock-token-checktokenexists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-token-checktokenexists-api-openapi.yml
- filename: blackrock-token-generate-api-openapi.yml
  format: yaml
  label: BlackRock Token:generate API
  slug: blackrock-token-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/openapi/blackrock-token-generate-api-openapi.yml
authorization_urls:
- https://client.blackrock.com/api/oauth2/default/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Blackrock Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BlackRock publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the BlackRock API on a user''s behalf.


  Tokens are issued from https://client.blackrock.com/api/oauth2/default/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BlackRock
provider_slug: blackrock
schemes:
- description: This API uses OAuth 2.0 with the access code flow.
  flows:
  - authorizationUrl: https://client.blackrock.com/api/oauth2/default/v1/authorize
    flow: authorizationCode
    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token
  name: OAuth2AccessCode
  source: openapi/blackrock-studio-notification-openapi.yml
- description: This API uses OAuth 2.0 with the client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token
  name: OAuth2ClientCredentials
  source: openapi/blackrock-studio-notification-openapi.yml
- description: This API uses OAuth 2.0 with the access code flow.
  flows:
  - authorizationUrl: https://client.blackrock.com/api/oauth2/default/v1/authorize
    flow: authorizationCode
    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token
  name: OAuth2AccessCode
  source: openapi/blackrock-studio-subscription-openapi.yml
- description: This API uses OAuth 2.0 with the client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token
  name: OAuth2ClientCredentials
  source: openapi/blackrock-studio-subscription-openapi.yml
- description: This API uses OAuth 2.0 with the access code flow.
  flows:
  - authorizationUrl: https://client.blackrock.com/api/oauth2/default/v1/authorize
    flow: authorizationCode
    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token
  name: OAuth2AccessCode
  source: openapi/blackrock-token-openapi.yml
- description: This API uses OAuth 2.0 with the client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token
  name: OAuth2ClientCredentials
  source: openapi/blackrock-token-openapi.yml
scope_count: 4
scope_names:
- offline_access
- platform.infrastructure.token.v1.Token:read
- platform.studio.studio_notification.v1.StudioNotification
- platform.studio.studio_notification.v1.StudioSubscription
scopes:
- description: This keeps you signed in to the app, even when you are not using it.
  flows:
  - authorizationCode
  - clientCredentials
  scope: offline_access
- description: non-sensitive read
  flows:
  - authorizationCode
  - clientCredentials
  scope: platform.infrastructure.token.v1.Token:read
- description: This grants access to all endpoints in the platform.studio.studio_notification.v1.StudioNotification API
  flows:
  - authorizationCode
  - clientCredentials
  scope: platform.studio.studio_notification.v1.StudioNotification
- description: This grants access to all endpoints in the platform.studio.studio_notification.v1.StudioSubscription API
  flows:
  - authorizationCode
  - clientCredentials
  scope: platform.studio.studio_notification.v1.StudioSubscription
slug: blackrock-scopes
source_filename: blackrock-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/blackrock-studio-notification-openapi.yml, openapi/blackrock-studio-subscription-openapi.yml,\n  openapi/blackrock-token-openapi.yml\nschemes:\n- name: OAuth2AccessCode\n  source: openapi/blackrock-studio-notification-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://client.blackrock.com/api/oauth2/default/v1/authorize\n    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token\n  description: This API uses OAuth 2.0 with the access code flow.\n- name: OAuth2ClientCredentials\n  source: openapi/blackrock-studio-notification-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token\n  description: This API uses OAuth 2.0 with the client credentials flow.\n- name: OAuth2AccessCode\n  source: openapi/blackrock-studio-subscription-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://client.blackrock.com/api/oauth2/default/v1/authorize\n\
  \    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token\n  description: This API uses OAuth 2.0 with the access code flow.\n- name: OAuth2ClientCredentials\n  source: openapi/blackrock-studio-subscription-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token\n  description: This API uses OAuth 2.0 with the client credentials flow.\n- name: OAuth2AccessCode\n  source: openapi/blackrock-token-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://client.blackrock.com/api/oauth2/default/v1/authorize\n    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token\n  description: This API uses OAuth 2.0 with the access code flow.\n- name: OAuth2ClientCredentials\n  source: openapi/blackrock-token-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://client.blackrock.com/api/oauth2/default/v1/token\n  description: This API uses OAuth 2.0 with the client\
  \ credentials flow.\nscopes:\n- scope: offline_access\n  description: This keeps you signed in to the app, even when you are not using it.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/blackrock-studio-notification-openapi.yml\n  - openapi/blackrock-studio-subscription-openapi.yml\n  - openapi/blackrock-token-openapi.yml\n- scope: platform.infrastructure.token.v1.Token:read\n  description: non-sensitive read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/blackrock-token-openapi.yml\n- scope: platform.studio.studio_notification.v1.StudioNotification\n  description: This grants access to all endpoints in the platform.studio.studio_notification.v1.StudioNotification\n    API\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/blackrock-studio-notification-openapi.yml\n- scope: platform.studio.studio_notification.v1.StudioSubscription\n  description: This grants access to all endpoints in the\
  \ platform.studio.studio_notification.v1.StudioSubscription\n    API\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/blackrock-studio-subscription-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/scopes/blackrock-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Asset Management
- Finance
- Fintech
- Investment Management
- Portfolio Management
- Risk Analytics
- Fortune 500
token_bound: false
token_urls:
- https://client.blackrock.com/api/oauth2/default/v1/token
---
