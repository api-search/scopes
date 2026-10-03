---
api_specs:
- filename: bodyspec-api-status-api-openapi.yml
  format: yaml
  label: BodySpec API Status API
  slug: bodyspec-api-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-api-status-api-openapi.yml
- filename: bodyspec-appointments-api-openapi.yml
  format: yaml
  label: BodySpec Appointments API
  slug: bodyspec-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-appointments-api-openapi.yml
- filename: bodyspec-availability-api-openapi.yml
  format: yaml
  label: BodySpec Availability API
  slug: bodyspec-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-availability-api-openapi.yml
- filename: bodyspec-bodyspec-api-api-openapi.yml
  format: yaml
  label: BodySpec BodySpec API
  slug: bodyspec-bodyspec-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-bodyspec-api-api-openapi.yml
- filename: bodyspec-locations-api-openapi.yml
  format: yaml
  label: BodySpec Locations API
  slug: bodyspec-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-locations-api-openapi.yml
- filename: bodyspec-partner-appointments-api-openapi.yml
  format: yaml
  label: BodySpec Partner Appointments API
  slug: bodyspec-partner-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-appointments-api-openapi.yml
- filename: bodyspec-partner-intake-api-openapi.yml
  format: yaml
  label: BodySpec Partner Intake API
  slug: bodyspec-partner-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-intake-api-openapi.yml
- filename: bodyspec-partner-orders-api-openapi.yml
  format: yaml
  label: BodySpec Partner Orders API
  slug: bodyspec-partner-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-orders-api-openapi.yml
- filename: bodyspec-partner-results-api-openapi.yml
  format: yaml
  label: BodySpec Partner Results API
  slug: bodyspec-partner-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-results-api-openapi.yml
- filename: bodyspec-partner-users-api-openapi.yml
  format: yaml
  label: BodySpec Partner Users API
  slug: bodyspec-partner-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-users-api-openapi.yml
- filename: bodyspec-partner-webhooks-api-openapi.yml
  format: yaml
  label: BodySpec Partner Webhooks API
  slug: bodyspec-partner-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-webhooks-api-openapi.yml
- filename: bodyspec-reservations-api-openapi.yml
  format: yaml
  label: BodySpec Reservations API
  slug: bodyspec-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-reservations-api-openapi.yml
- filename: bodyspec-results-api-openapi.yml
  format: yaml
  label: BodySpec Results API
  slug: bodyspec-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-results-api-openapi.yml
- filename: bodyspec-services-api-openapi.yml
  format: yaml
  label: BodySpec Services API
  slug: bodyspec-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-services-api-openapi.yml
- filename: bodyspec-users-api-openapi.yml
  format: yaml
  label: BodySpec Users API
  slug: bodyspec-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-users-api-openapi.yml
authorization_urls:
- https://auth.bodyspec.com/realms/bodyspec/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bodyspec Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BodySpec publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BodySpec API on a user''s behalf.


  Tokens are issued from https://auth.bodyspec.com/realms/bodyspec/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BodySpec
provider_slug: bodyspec
schemes:
- description: OAuth2 authentication via Keycloak with PKCE
  flows:
  - authorizationUrl: https://auth.bodyspec.com/realms/bodyspec/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://auth.bodyspec.com/realms/bodyspec/protocol/openid-connect/token
  name: OAuth2
  source: openapi/bodyspec-openapi.json
scope_count: 3
scope_names:
- email
- openid
- profile
scopes:
- description: Access to user email
  flows:
  - authorizationCode
  scope: email
- description: OpenID Connect scope
  flows:
  - authorizationCode
  scope: openid
- description: Access to user profile
  flows:
  - authorizationCode
  scope: profile
slug: bodyspec-scopes
source_filename: bodyspec-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: derived\nsource: openapi/bodyspec-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/bodyspec-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.bodyspec.com/realms/bodyspec/protocol/openid-connect/auth\n    tokenUrl: https://auth.bodyspec.com/realms/bodyspec/protocol/openid-connect/token\n  description: OAuth2 authentication via Keycloak with PKCE\nscopes:\n- scope: email\n  description: Access to user email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bodyspec-openapi.json\n- scope: openid\n  description: OpenID Connect scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bodyspec-openapi.json\n- scope: profile\n  description: Access to user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bodyspec-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/scopes/bodyspec-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Health
- Fitness
- API
- Data
token_urls:
- https://auth.bodyspec.com/realms/bodyspec/protocol/openid-connect/token
---
