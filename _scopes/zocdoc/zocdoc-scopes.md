---
api_specs:
- filename: zocdoc-appointments-api-openapi.yml
  format: yaml
  label: Zocdoc appointments API
  slug: zocdoc-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-appointments-api-openapi.yml
- filename: zocdoc-calendar-integration-timeslots-api-openapi.yml
  format: yaml
  label: Zocdoc calendar-integration-timeslots API
  slug: zocdoc-calendar-integration-timeslots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml
- filename: zocdoc-credentials-api-openapi.yml
  format: yaml
  label: Zocdoc credentials API
  slug: zocdoc-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-credentials-api-openapi.yml
- filename: zocdoc-facilities-api-openapi.yml
  format: yaml
  label: Zocdoc facilities API
  slug: zocdoc-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-facilities-api-openapi.yml
- filename: zocdoc-insurance-reference-api-openapi.yml
  format: yaml
  label: Zocdoc insurance-reference API
  slug: zocdoc-insurance-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-insurance-reference-api-openapi.yml
- filename: zocdoc-provider-locations-api-openapi.yml
  format: yaml
  label: Zocdoc provider-locations API
  slug: zocdoc-provider-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-provider-locations-api-openapi.yml
- filename: zocdoc-providers-api-openapi.yml
  format: yaml
  label: Zocdoc providers API
  slug: zocdoc-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-providers-api-openapi.yml
- filename: zocdoc-reference-api-openapi.yml
  format: yaml
  label: Zocdoc reference API
  slug: zocdoc-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-reference-api-openapi.yml
- filename: zocdoc-schedulable-entities-api-openapi.yml
  format: yaml
  label: Zocdoc schedulable-entities API
  slug: zocdoc-schedulable-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-schedulable-entities-api-openapi.yml
- filename: zocdoc-webhook-api-openapi.yml
  format: yaml
  label: Zocdoc webhook API
  slug: zocdoc-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-webhook-api-openapi.yml
- filename: zocdoc-reviews-api-openapi.yml
  format: yaml
  label: Zocdoc reviews API
  slug: zocdoc-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-reviews-api-openapi.yml
- filename: zocdoc-specialties-api-openapi.yml
  format: yaml
  label: Zocdoc specialties API
  slug: zocdoc-specialties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-specialties-api-openapi.yml
- filename: zocdoc-visit-reasons-api-openapi.yml
  format: yaml
  label: Zocdoc visit-reasons API
  slug: zocdoc-visit-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/openapi/zocdoc-visit-reasons-api-openapi.yml
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
overview: 'Zocdoc publishes 10 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zocdoc API on a user''s behalf.


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
  source: openapi/zocdoc-appointments-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-appointments-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-credentials-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-credentials-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-facilities-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-facilities-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-insurance-reference-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-insurance-reference-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-provider-locations-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-provider-locations-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-providers-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-providers-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-reference-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-reference-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-reviews-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-reviews-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-schedulable-entities-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-schedulable-entities-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-specialties-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-specialties-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-visit-reasons-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-visit-reasons-api-openapi.yml
- description: 'Machine to machine authentication (for use from client server to Zocdoc).

    Production: `https://auth.zocdoc.com/oauth/token`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: ClientCredentialsFlow
  source: openapi/zocdoc-webhook-api-openapi.yml
- description: 'Log in as a user. Client Secret is not necessary for this login flow.

    Production: `https://auth.zocdoc.com`

    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`'
  flows:
  - authorizationUrl: https://auth.zocdoc.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.zocdoc.com/oauth/token
  name: AuthorizationCodeFlow
  source: openapi/zocdoc-webhook-api-openapi.yml
scope_count: 10
scope_names:
- external.anonymous_token.write
- external.appointment.read
- external.appointment.write
- external.booking_intent.read
- external.booking_intent.write
- external.consent.read
- external.credential.rotate
- external.partner_consent.write
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
- description: Read booking intents.
  flows:
  - clientCredentials
  scope: external.booking_intent.read
- description: Create and modify booking intents.
  flows:
  - clientCredentials
  scope: external.booking_intent.write
- description: Read your partner-connect consent grants.
  flows:
  - clientCredentials
  scope: external.consent.read
- description: Rotate the authenticated client secret.
  flows:
  - clientCredentials
  scope: external.credential.rotate
- description: Revoke your partner-connect consent grants.
  flows:
  - clientCredentials
  scope: external.partner_consent.write
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
source_yaml: "generated: '2026-08-15'\nmethod: derived\nsource: openapi/zocdoc-appointments-api-openapi.yml, openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml,\n  openapi/zocdoc-credentials-api-openapi.yml, openapi/zocdoc-facilities-api-openapi.yml, openapi/zocdoc-insurance-reference-api-openapi.yml,\n  openapi/zocdoc-provider-locations-api-openapi.yml, openapi/zocdoc-providers-api-openapi.yml,\n  openapi/zocdoc-reference-api-openapi.yml, openapi/zocdoc-reviews-api-openapi.yml, openapi/zocdoc-schedulable-entities-api-openapi.yml,\n  openapi/zocdoc-specialties-api-openapi.yml, openapi/zocdoc-visit-reasons-api-openapi.yml,\n  openapi/zocdoc-webhook-api-openapi.yml\nschemes:\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-appointments-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n\
  \    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-appointments-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-credentials-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-credentials-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n\
  \    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-facilities-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-facilities-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n\
  - name: ClientCredentialsFlow\n  source: openapi/zocdoc-insurance-reference-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-insurance-reference-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-provider-locations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n\
  \  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-provider-locations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-providers-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox:\
  \ `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-providers-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-reference-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-reference-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-reviews-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-reviews-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary\
  \ for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-schedulable-entities-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-schedulable-entities-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n- name: ClientCredentialsFlow\n\
  \  source: openapi/zocdoc-specialties-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-specialties-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-visit-reasons-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n\
  \    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n- name: AuthorizationCodeFlow\n  source: openapi/zocdoc-visit-reasons-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\n- name: ClientCredentialsFlow\n  source: openapi/zocdoc-webhook-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Machine to machine authentication (for use from client server to Zocdoc).\n    Production: `https://auth.zocdoc.com/oauth/token`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com/oauth/token`\n\
  - name: AuthorizationCodeFlow\n  source: openapi/zocdoc-webhook-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.zocdoc.com/authorize\n    tokenUrl: https://auth.zocdoc.com/oauth/token\n  description: |-\n    Log in as a user. Client Secret is not necessary for this login flow.\n    Production: `https://auth.zocdoc.com`\n    Sandbox: `https://auth-api-developer-sandbox.zocdoc.com`\nscopes:\n- scope: external.anonymous_token.write\n  description: Create anonymous tokens used for discovery endpoints.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-appointments-api-openapi.yml\n  - openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml\n  - openapi/zocdoc-credentials-api-openapi.yml\n  - openapi/zocdoc-facilities-api-openapi.yml\n  - openapi/zocdoc-insurance-reference-api-openapi.yml\n  - openapi/zocdoc-provider-locations-api-openapi.yml\n  - openapi/zocdoc-providers-api-openapi.yml\n  - openapi/zocdoc-reference-api-openapi.yml\n\
  \  - openapi/zocdoc-reviews-api-openapi.yml\n  - openapi/zocdoc-schedulable-entities-api-openapi.yml\n  - openapi/zocdoc-specialties-api-openapi.yml\n  - openapi/zocdoc-visit-reasons-api-openapi.yml\n  - openapi/zocdoc-webhook-api-openapi.yml\n- scope: external.appointment.read\n  description: Read basic details of your appointments.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-appointments-api-openapi.yml\n  - openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml\n  - openapi/zocdoc-credentials-api-openapi.yml\n  - openapi/zocdoc-facilities-api-openapi.yml\n  - openapi/zocdoc-insurance-reference-api-openapi.yml\n  - openapi/zocdoc-provider-locations-api-openapi.yml\n  - openapi/zocdoc-providers-api-openapi.yml\n  - openapi/zocdoc-reference-api-openapi.yml\n  - openapi/zocdoc-reviews-api-openapi.yml\n  - openapi/zocdoc-schedulable-entities-api-openapi.yml\n  - openapi/zocdoc-specialties-api-openapi.yml\n  - openapi/zocdoc-visit-reasons-api-openapi.yml\n\
  \  - openapi/zocdoc-webhook-api-openapi.yml\n- scope: external.appointment.write\n  description: Book and modify appointments.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-appointments-api-openapi.yml\n  - openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml\n  - openapi/zocdoc-credentials-api-openapi.yml\n  - openapi/zocdoc-facilities-api-openapi.yml\n  - openapi/zocdoc-insurance-reference-api-openapi.yml\n  - openapi/zocdoc-provider-locations-api-openapi.yml\n  - openapi/zocdoc-providers-api-openapi.yml\n  - openapi/zocdoc-reference-api-openapi.yml\n  - openapi/zocdoc-reviews-api-openapi.yml\n  - openapi/zocdoc-schedulable-entities-api-openapi.yml\n  - openapi/zocdoc-specialties-api-openapi.yml\n  - openapi/zocdoc-visit-reasons-api-openapi.yml\n  - openapi/zocdoc-webhook-api-openapi.yml\n- scope: external.booking_intent.read\n  description: Read booking intents.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-appointments-api-openapi.yml\n\
  \  - openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml\n  - openapi/zocdoc-facilities-api-openapi.yml\n  - openapi/zocdoc-insurance-reference-api-openapi.yml\n  - openapi/zocdoc-provider-locations-api-openapi.yml\n  - openapi/zocdoc-providers-api-openapi.yml\n  - openapi/zocdoc-reference-api-openapi.yml\n  - openapi/zocdoc-reviews-api-openapi.yml\n  - openapi/zocdoc-schedulable-entities-api-openapi.yml\n  - openapi/zocdoc-specialties-api-openapi.yml\n  - openapi/zocdoc-visit-reasons-api-openapi.yml\n  - openapi/zocdoc-webhook-api-openapi.yml\n- scope: external.booking_intent.write\n  description: Create and modify booking intents.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-appointments-api-openapi.yml\n  - openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml\n  - openapi/zocdoc-facilities-api-openapi.yml\n  - openapi/zocdoc-insurance-reference-api-openapi.yml\n  - openapi/zocdoc-provider-locations-api-openapi.yml\n  - openapi/zocdoc-providers-api-openapi.yml\n\
  \  - openapi/zocdoc-reference-api-openapi.yml\n  - openapi/zocdoc-reviews-api-openapi.yml\n  - openapi/zocdoc-schedulable-entities-api-openapi.yml\n  - openapi/zocdoc-specialties-api-openapi.yml\n  - openapi/zocdoc-visit-reasons-api-openapi.yml\n  - openapi/zocdoc-webhook-api-openapi.yml\n- scope: external.consent.read\n  description: Read your partner-connect consent grants.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-appointments-api-openapi.yml\n  - openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml\n  - openapi/zocdoc-facilities-api-openapi.yml\n  - openapi/zocdoc-insurance-reference-api-openapi.yml\n  - openapi/zocdoc-provider-locations-api-openapi.yml\n  - openapi/zocdoc-providers-api-openapi.yml\n  - openapi/zocdoc-reference-api-openapi.yml\n  - openapi/zocdoc-reviews-api-openapi.yml\n  - openapi/zocdoc-schedulable-entities-api-openapi.yml\n  - openapi/zocdoc-specialties-api-openapi.yml\n  - openapi/zocdoc-visit-reasons-api-openapi.yml\n  - openapi/zocdoc-webhook-api-openapi.yml\n\
  - scope: external.credential.rotate\n  description: Rotate the authenticated client secret.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-credentials-api-openapi.yml\n- scope: external.partner_consent.write\n  description: Revoke your partner-connect consent grants.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-appointments-api-openapi.yml\n  - openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml\n  - openapi/zocdoc-facilities-api-openapi.yml\n  - openapi/zocdoc-insurance-reference-api-openapi.yml\n  - openapi/zocdoc-provider-locations-api-openapi.yml\n  - openapi/zocdoc-providers-api-openapi.yml\n  - openapi/zocdoc-reference-api-openapi.yml\n  - openapi/zocdoc-reviews-api-openapi.yml\n  - openapi/zocdoc-schedulable-entities-api-openapi.yml\n  - openapi/zocdoc-specialties-api-openapi.yml\n  - openapi/zocdoc-visit-reasons-api-openapi.yml\n  - openapi/zocdoc-webhook-api-openapi.yml\n- scope: external.provider_insurance.write\n  description:\
  \ Update the insurance accepted by a provider.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-appointments-api-openapi.yml\n  - openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml\n  - openapi/zocdoc-credentials-api-openapi.yml\n  - openapi/zocdoc-facilities-api-openapi.yml\n  - openapi/zocdoc-insurance-reference-api-openapi.yml\n  - openapi/zocdoc-provider-locations-api-openapi.yml\n  - openapi/zocdoc-providers-api-openapi.yml\n  - openapi/zocdoc-reference-api-openapi.yml\n  - openapi/zocdoc-reviews-api-openapi.yml\n  - openapi/zocdoc-schedulable-entities-api-openapi.yml\n  - openapi/zocdoc-specialties-api-openapi.yml\n  - openapi/zocdoc-visit-reasons-api-openapi.yml\n  - openapi/zocdoc-webhook-api-openapi.yml\n- scope: external.schedulable_entity.read\n  description: Read schedulable entities.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/zocdoc-appointments-api-openapi.yml\n  - openapi/zocdoc-calendar-integration-timeslots-api-openapi.yml\n\
  \  - openapi/zocdoc-credentials-api-openapi.yml\n  - openapi/zocdoc-facilities-api-openapi.yml\n  - openapi/zocdoc-insurance-reference-api-openapi.yml\n  - openapi/zocdoc-provider-locations-api-openapi.yml\n  - openapi/zocdoc-providers-api-openapi.yml\n  - openapi/zocdoc-reference-api-openapi.yml\n  - openapi/zocdoc-reviews-api-openapi.yml\n  - openapi/zocdoc-schedulable-entities-api-openapi.yml\n  - openapi/zocdoc-specialties-api-openapi.yml\n  - openapi/zocdoc-visit-reasons-api-openapi.yml\n  - openapi/zocdoc-webhook-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/scopes/zocdoc-scopes.yml
summary_line: 10 scopes · clientCredentials/authorizationCode
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
