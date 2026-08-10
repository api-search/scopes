---
api_specs:
- filename: buoy-health-complaints-api-openapi.yml
  format: yaml
  label: Buoy Health Complaints API
  slug: buoy-health-complaints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-complaints-api-openapi.yml
- filename: buoy-health-intents-api-openapi.yml
  format: yaml
  label: Buoy Health Intents API
  slug: buoy-health-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-intents-api-openapi.yml
- filename: buoy-health-interviews-api-openapi.yml
  format: yaml
  label: Buoy Health Interviews API
  slug: buoy-health-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-interviews-api-openapi.yml
- filename: buoy-health-queries-api-openapi.yml
  format: yaml
  label: Buoy Health Queries API
  slug: buoy-health-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-queries-api-openapi.yml
- filename: buoy-health-questions-api-openapi.yml
  format: yaml
  label: Buoy Health Questions API
  slug: buoy-health-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-questions-api-openapi.yml
- filename: buoy-health-results-api-openapi.yml
  format: yaml
  label: Buoy Health Results API
  slug: buoy-health-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/openapi/buoy-health-results-api-openapi.yml
authorization_urls:
- https://auth.sandbox.buoyhealth.com/authorize
description: ''
docs: https://buoyhealth.readme.io/reference/interviews_anonymous
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Buoy Health Scopes
name_suffix: OAuth Scopes
note: 'The OpenAPI declares a single oauth2 authorizationCode scheme ("Bearer") with an EMPTY scopes map, and no operation carries a scope requirement — the Symptom Checker API is scope-flat: a valid bearer token grants the whole 19-operation surface. The scopes below are the ones the authorization server itself advertises in its anonymous RFC 8414 / OIDC discovery documents; they are OIDC identity scopes issued by the Auth0-backed issuer, NOT Buoy API resource scopes. No public Buoy scope or permissions reference page was found.'
overview: 'Buoy Health publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Buoy Health API on a user''s behalf.


  Tokens are issued from https://auth.sandbox.buoyhealth.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Buoy Health
provider_slug: buoy-health
schemes:
- description: '[Full documentation for the Buoy Auth API is found here.](https://sandbox.buoyhealth.com/auth/redoc/)'
  flows:
  - authorizationUrl: https://auth.sandbox.buoyhealth.com/authorize
    flow: authorizationCode
    scopes: []
    tokenUrl: https://auth.sandbox.buoyhealth.com/oauth/token
  name: Bearer
  source: openapi/buoy-health-symptom-checker-openapi.yml
  type: oauth2
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- name
- given_name
- family_name
- nickname
- email
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Request an OpenID Connect ID token for the authenticating subject.
  flows: []
  scope: openid
- description: Basic profile claims for the authenticating subject.
  flows: []
  scope: profile
- description: Issue a refresh token so the client can renew access without user interaction.
  flows: []
  scope: offline_access
- description: The subject's full name claim.
  flows: []
  scope: name
- description: The subject's given name claim.
  flows: []
  scope: given_name
- description: The subject's family name claim.
  flows: []
  scope: family_name
- description: The subject's nickname claim.
  flows: []
  scope: nickname
- description: The subject's email address claim.
  flows: []
  scope: email
- description: Whether the subject's email address has been verified.
  flows: []
  scope: email_verified
- description: The subject's profile picture claim.
  flows: []
  scope: picture
- description: When the subject's identity record was created.
  flows: []
  scope: created_at
- description: Linked identity-provider records for the subject.
  flows: []
  scope: identities
- description: The subject's phone number claim.
  flows: []
  scope: phone
- description: The subject's address claim.
  flows: []
  scope: address
slug: buoy-health-scopes
source_filename: buoy-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: https://auth.buoyhealth.com/.well-known/openid-configuration\ndocs: https://buoyhealth.readme.io/reference/interviews_anonymous\nnote: >-\n  The OpenAPI declares a single oauth2 authorizationCode scheme (\"Bearer\") with an EMPTY scopes map,\n  and no operation carries a scope requirement — the Symptom Checker API is scope-flat: a valid bearer\n  token grants the whole 19-operation surface. The scopes below are the ones the authorization server\n  itself advertises in its anonymous RFC 8414 / OIDC discovery documents; they are OIDC identity\n  scopes issued by the Auth0-backed issuer, NOT Buoy API resource scopes. No public Buoy scope or\n  permissions reference page was found.\nschemes:\n- name: Bearer\n  source: openapi/buoy-health-symptom-checker-openapi.yml\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.sandbox.buoyhealth.com/authorize\n    tokenUrl: https://auth.sandbox.buoyhealth.com/oauth/token\n\
  \    scopes: []\n  description: '[Full documentation for the Buoy Auth API is found here.](https://sandbox.buoyhealth.com/auth/redoc/)'\nissuers:\n- environment: production\n  issuer: https://auth.buoyhealth.com/\n  discovery: https://auth.buoyhealth.com/.well-known/openid-configuration\n  http_status: 200\n- environment: sandbox\n  issuer: https://auth.sandbox.buoyhealth.com/\n  discovery: https://auth.sandbox.buoyhealth.com/.well-known/openid-configuration\n  http_status: 200\nscopes:\n- scope: openid\n  description: Request an OpenID Connect ID token for the authenticating subject.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims for the authenticating subject.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without user interaction.\n  kind: oidc-identity\n  sources:\
  \ [well-known/buoy-health-openid-configuration.json]\n- scope: name\n  description: The subject's full name claim.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n- scope: given_name\n  description: The subject's given name claim.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n- scope: family_name\n  description: The subject's family name claim.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n- scope: nickname\n  description: The subject's nickname claim.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n- scope: email\n  description: The subject's email address claim.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n- scope: email_verified\n  description: Whether the subject's email address has been verified.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n\
  - scope: picture\n  description: The subject's profile picture claim.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n- scope: created_at\n  description: When the subject's identity record was created.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n- scope: identities\n  description: Linked identity-provider records for the subject.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n- scope: phone\n  description: The subject's phone number claim.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\n- scope: address\n  description: The subject's address claim.\n  kind: oidc-identity\n  sources: [well-known/buoy-health-openid-configuration.json]\nx-evidence:\n- url: https://auth.buoyhealth.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-08'\n- url: https://auth.buoyhealth.com/.well-known/oauth-authorization-server\n\
  \  http_status: 200\n  fetched: '2026-08-08'\n- url: https://auth.sandbox.buoyhealth.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-08'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buoy-health/refs/heads/main/scopes/buoy-health-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- symptom-checker
- medical-triage
- digital-health
- healthcare
- clinical-ai
- care-navigation
- patient-engagement
- diagnosis
- telehealth
- oauth2
token_urls:
- https://auth.sandbox.buoyhealth.com/oauth/token
---
