---
api_specs:
- filename: b-well-users-api-openapi.yml
  format: yaml
  label: b.well Users API
  slug: b-well-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/openapi/b-well-users-api-openapi.yml
- filename: b-well-webhook-api-openapi.yml
  format: yaml
  label: b.well Webhook API
  slug: b-well-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/openapi/b-well-webhook-api-openapi.yml
authorization_urls:
- https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/authorize
- https://client-sandbox-fhir.auth.us-east-1.amazoncognito.com/oauth2/authorize
description: ''
docs: https://developer.bwell.com/docs/system-auth
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: B Well Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'b.well publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the b.well API on a user''s behalf.


  Tokens are issued from https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: b.well
provider_slug: b-well
schemes:
- file: well-known/b-well-smart-configuration.json
  flows:
  - authorizationUrl: https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/token
  name: SMART on FHIR / OAuth 2.0 (production)
  source: https://fhir.icanbwell.com/.well-known/smart-configuration
- file: well-known/b-well-smart-configuration-sandbox.json
  flows:
  - authorizationUrl: https://client-sandbox-fhir.auth.us-east-1.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://client-sandbox-fhir.auth.us-east-1.amazoncognito.com/oauth2/token
  name: SMART on FHIR / OAuth 2.0 (client-sandbox)
  source: https://fhir.client-sandbox.icanbwell.com/.well-known/smart-configuration
scope_count: 4
scope_names:
- openid
- profile
- email
- phone
scopes:
- description: OpenID Connect — issue an ID token identifying the authenticated subject.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the subject's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the subject's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access to the subject's phone number claim.
  flows:
  - authorizationCode
  scope: phone
slug: b-well-scopes
source_filename: b-well-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://fhir.icanbwell.com/.well-known/smart-configuration\ndocs: https://developer.bwell.com/docs/system-auth\nnotes: >-\n  b.well documents scope-based authorization but does not publish a scope reference\n  page. Client IDs are \"assigned specific scopes during onboarding based on your\n  integration requirements\", so the full scope vocabulary is negotiated per customer\n  and is not publicly enumerable. The scopes recorded below are the ones actually\n  advertised anonymously in the SMART-on-FHIR configuration documents served by the\n  production and sandbox FHIR hosts — the identity scopes of the underlying AWS\n  Cognito authorization server. No SMART clinical scopes (patient/*.read and the\n  like) are advertised there.\nschemes:\n- name: SMART on FHIR / OAuth 2.0 (production)\n  source: https://fhir.icanbwell.com/.well-known/smart-configuration\n  file: well-known/b-well-smart-configuration.json\n  flows:\n  - flow:\
  \ authorizationCode\n    authorizationUrl: https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/authorize\n    tokenUrl: https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/token\n- name: SMART on FHIR / OAuth 2.0 (client-sandbox)\n  source: https://fhir.client-sandbox.icanbwell.com/.well-known/smart-configuration\n  file: well-known/b-well-smart-configuration-sandbox.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://client-sandbox-fhir.auth.us-east-1.amazoncognito.com/oauth2/authorize\n    tokenUrl: https://client-sandbox-fhir.auth.us-east-1.amazoncognito.com/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect — issue an ID token identifying the authenticated subject.\n  flows: [authorizationCode]\n  sources: [well-known/b-well-smart-configuration.json, well-known/b-well-smart-configuration-sandbox.json]\n- scope: profile\n\
  \  description: Access to the subject's basic profile claims.\n  flows: [authorizationCode]\n  sources: [well-known/b-well-smart-configuration.json, well-known/b-well-smart-configuration-sandbox.json]\n- scope: email\n  description: Access to the subject's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/b-well-smart-configuration.json, well-known/b-well-smart-configuration-sandbox.json]\n- scope: phone\n  description: Access to the subject's phone number claim.\n  flows: [authorizationCode]\n  sources: [well-known/b-well-smart-configuration.json, well-known/b-well-smart-configuration-sandbox.json]\ngaps:\n- issue: no published scope reference\n  detail: >-\n    Neither developer.bwell.com nor the SMART configuration enumerates the data-access\n    scopes granted to a client credentials integration. An integrator cannot see, before\n    onboarding, which scopes exist or what each one unlocks.\n  fixable_by: b.well\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/scopes/b-well-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Company
- Health
- Healthcare
- Digital Health
- FHIR
- Health Data
- Interoperability
- Patient Access
- Health Records
- MCP
token_urls:
- https://fhir-bwell.auth.us-east-1.amazoncognito.com/oauth2/token
- https://client-sandbox-fhir.auth.us-east-1.amazoncognito.com/oauth2/token
---
