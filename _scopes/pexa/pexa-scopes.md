---
api_specs:
- filename: pexa-exchange-api-swagger.json
  format: json
  label: PEXA Exchange API
  slug: pexa-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-exchange-api-swagger.json
- filename: pexa-standalone-discharge-experience-api-openapi.yaml
  format: yaml
  label: PEXA Standalone Discharge Experience API
  slug: pexa-standalone-discharge-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-standalone-discharge-experience-api-openapi.yaml
- filename: pexa-plus-marketplace-b2b-api-openapi.yaml
  format: yaml
  label: PEXA Plus Marketplace B2B API
  slug: pexa-plus-marketplace-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-plus-marketplace-b2b-api-openapi.yaml
- filename: pexa-notification-service-openapi.yaml
  format: yaml
  label: PEXA Notification Service [$]
  slug: pexa-notification-service-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-notification-service-openapi.yaml
- filename: pexa-projects-api-v4-openapi.yaml
  format: yaml
  label: PEXA Projects API
  slug: pexa-projects-api-v4-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/openapi/pexa-projects-api-v4-openapi.yaml
authorization_urls:
- https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/auth
- https://'{{auth2_env}}'/authorize
description: ''
docs: https://developer.pexa.com.au/Exchange/docs/documentation/
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Pexa Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PEXA publishes 11 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the PEXA API on a user''s behalf.


  Tokens are issued from https://auth.pexa.com.au/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PEXA
provider_slug: pexa
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.pexa.com.au/oauth/token
  name: oauth2
  source: openapi/pexa-notification-service-openapi.yaml
- flows:
  - authorizationUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/token
  name: oauth2
  source: openapi/pexa-projects-api-v4-openapi.yaml
- flows:
  - authorizationUrl: https://'{{auth2_env}}'/authorize
    flow: authorizationCode
    tokenUrl: https://'{{auth2_env}}'/oauth/token
  - flow: clientCredentials
    tokenUrl: https://'{{auth2_env}}'/oauth/token
  name: oauth2
  source: openapi/pexa-standalone-discharge-experience-api-openapi.yaml
scope_count: 11
scope_names:
- au:projects:notification:read
- au:projects:project:write
- au:projects:status:read
- au:projects:workspaces:read
- au:projects:workspaces:write
- create:notification_registrations
- create:notification_registrations_secret_rotation
- delete:notification_registrations
- edit:notification_registrations
- view:notification_registrations
- '{{api_scope}}'
scopes:
- description: ''
  flows: []
  scope: au:projects:notification:read
- description: Grant project write access
  flows:
  - authorizationCode
  - clientCredentials
  scope: au:projects:project:write
- description: Grant project status read access
  flows:
  - authorizationCode
  - clientCredentials
  scope: au:projects:status:read
- description: Grant project workspaces read access
  flows:
  - authorizationCode
  - clientCredentials
  scope: au:projects:workspaces:read
- description: ''
  flows: []
  scope: au:projects:workspaces:write
- description: Create registrations
  flows:
  - clientCredentials
  scope: create:notification_registrations
- description: Rotate shared secret
  flows:
  - clientCredentials
  scope: create:notification_registrations_secret_rotation
- description: Delete registrations
  flows:
  - clientCredentials
  scope: delete:notification_registrations
- description: Edit registrations
  flows:
  - clientCredentials
  scope: edit:notification_registrations
- description: View registrations
  flows:
  - clientCredentials
  scope: view:notification_registrations
- description: API scope
  flows:
  - authorizationCode
  - clientCredentials
  scope: '{{api_scope}}'
slug: pexa-scopes
source_filename: pexa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/pexa-notification-service-openapi.yaml, openapi/pexa-projects-api-v4-openapi.yaml, openapi/pexa-standalone-discharge-experience-api-openapi.yaml\nschemes:\n- name: oauth2\n  source: openapi/pexa-notification-service-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.pexa.com.au/oauth/token\n- name: oauth2\n  source: openapi/pexa-projects-api-v4-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/auth\n    tokenUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/token\n- name: oauth2\n  source: openapi/pexa-standalone-discharge-experience-api-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://'{{auth2_env}}'/authorize\n\
  \    tokenUrl: https://'{{auth2_env}}'/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://'{{auth2_env}}'/oauth/token\nscopes:\n- scope: au:projects:notification:read\n  sources:\n  - openapi/pexa-projects-api-v4-openapi.yaml\n- scope: au:projects:project:write\n  description: Grant project write access\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/pexa-projects-api-v4-openapi.yaml\n- scope: au:projects:status:read\n  description: Grant project status read access\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/pexa-projects-api-v4-openapi.yaml\n- scope: au:projects:workspaces:read\n  description: Grant project workspaces read access\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/pexa-projects-api-v4-openapi.yaml\n- scope: au:projects:workspaces:write\n  sources:\n  - openapi/pexa-projects-api-v4-openapi.yaml\n- scope: create:notification_registrations\n  description: Create\
  \ registrations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pexa-notification-service-openapi.yaml\n- scope: create:notification_registrations_secret_rotation\n  description: Rotate shared secret\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pexa-notification-service-openapi.yaml\n- scope: delete:notification_registrations\n  description: Delete registrations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pexa-notification-service-openapi.yaml\n- scope: edit:notification_registrations\n  description: Edit registrations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pexa-notification-service-openapi.yaml\n- scope: view:notification_registrations\n  description: View registrations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pexa-notification-service-openapi.yaml\n- scope: '{{api_scope}}'\n  description: API scope\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/pexa-standalone-discharge-experience-api-openapi.yaml\n\
  docs: https://developer.pexa.com.au/Exchange/docs/documentation/\ndocs_note: PEXA does not publish a single consolidated scopes reference page. Scopes are declared per endpoint in\n  the developer portal API reference (login-gated) and, for the Notification Service, restated in the PEXA Webhooks\n  Guide. The Exchange Swagger 2.0 contracts declare no securityDefinitions at all, so Exchange scope names do not\n  appear in any machine-readable artifact - the only Exchange scope PEXA publishes in the open is the worked example\n  au_pub_tst_pexa_conversation_api_v2_read.\nnaming_conventions:\n- family: notification-service\n  pattern: <verb>:notification_registrations[_<qualifier>]\n  source: openapi/pexa-notification-service-openapi.yaml + https://developer.pexa.com.au/Webhooks/docs/definitions/webhooks/\n  environments: the same five scope names apply in both non-prod and prod\n- family: projects\n  pattern: au:projects:<resource>:<read|write>\n  source: openapi/pexa-projects-api-v4-openapi.yaml\n\
  - family: exchange\n  pattern: au_<visibility>_<env>_pexa_<api>_<version>_<read|write>\n  example: au_pub_tst_pexa_conversation_api_v2_read\n  source: https://developer.pexa.com.au/Exchange/docs/documentation/\n  note: Environment appears to be encoded in the scope name itself (tst), so scope strings differ between test and\n    production.\ntoken_request: Scope is passed on the OAuth 2.0 token request (client_credentials) or on the authorize request (authorization_code);\n  each endpoint requires specific scopes.\nunresolved:\n- scope: '{{api_scope}}'\n  source: openapi/pexa-standalone-discharge-experience-api-openapi.yaml\n  note: Unresolved template shipped in the contract, not a real scope name. Recorded verbatim rather than guessed.\nscope_count: 11\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pexa/refs/heads/main/scopes/pexa-scopes.yml
summary_line: 11 scopes · clientCredentials/authorizationCode
tags:
- Real-Estate
- Australia
- Conveyancing
- Property Settlement
- Land Registry
- Title
- PropTech
- Mortgage
- Digital Signing
- Webhook
token_urls:
- https://auth.pexa.com.au/oauth/token
- https://host.kubernetes.internal/auth/realms/pexa/protocol/openid-connect/token
- https://'{{auth2_env}}'/oauth/token
---
