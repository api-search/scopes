---
api_specs:
- filename: apis.md
  format: yaml
  label: Zocdoc API
  slug: zocdoc-api
  spec_type: OpenAPI
  url: https://api-docs.zocdoc.com/apis.md
authorization_urls:
- https://auth.zocdoc.com/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zocdoc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zocdoc publishes 6 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zocdoc API on a user''s behalf.


  Tokens are issued from https://auth.zocdoc.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zocdoc
provider_slug: zocdoc
schemes:
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-zocdoc-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-zocdoc-api-openapi.yml
scope_count: 6
scope_names:
- external.anonymous_token.write
- external.appointment.read
- external.appointment.write
- external.credential.rotate
- external.provider_insurance.write
- external.schedulable_entity.read
scopes:
- description: Create anonymous tokens used for discovery endpoints.
  flows:
  - clientCredentials
  scope: external.anonymous_token.write
- description: Read basic details of your appointments.
  flows:
  - authorizationCode
  - clientCredentials
  scope: external.appointment.read
- description: Book and modify appointments.
  flows:
  - authorizationCode
  - clientCredentials
  scope: external.appointment.write
- description: Rotate the authenticated client secret.
  flows:
  - clientCredentials
  scope: external.credential.rotate
- description: Update the insurance accepted by a provider.
  flows:
  - clientCredentials
  scope: external.provider_insurance.write
- description: Read schedulable entities.
  flows:
  - authorizationCode
  - clientCredentials
  scope: external.schedulable_entity.read
slug: zocdoc-scopes
source_filename: zocdoc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zocdoc-zocdoc-api-openapi.yml\nschemes:\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-zocdoc-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-zocdoc-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\nscopes:\n- scope: external.anonymous_token.write\n  description: Create\
  \ anonymous tokens used for discovery endpoints.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-zocdoc-api-openapi.yml\n- scope: external.appointment.read\n  description: Read basic details of your appointments.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-zocdoc-api-openapi.yml\n- scope: external.appointment.write\n  description: Book and modify appointments.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-zocdoc-api-openapi.yml\n- scope: external.credential.rotate\n  description: Rotate the authenticated client secret.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-zocdoc-api-openapi.yml\n- scope: external.provider_insurance.write\n  description: Update the insurance accepted by a provider.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-zocdoc-api-openapi.yml\n- scope: external.schedulable_entity.read\n  description: Read schedulable entities.\n  flows:\n\
  \  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-zocdoc-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/scopes/zocdoc-scopes.yml
summary_line: 6 scopes · clientCredentials/authorizationCode
tags:
- Healthcare
- Appointments
- Booking
- Providers
- Insurance
- Telehealth
- Scheduling
token_urls:
- https://auth.zocdoc.com/oauth/token
---
