---
api_specs:
- filename: medplum-fhir-api-openapi.yml
  format: yaml
  label: Medplum Fhir API
  slug: medplum-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medplum/refs/heads/main/openapi/medplum-fhir-api-openapi.yml
authorization_urls:
- https://api.medplum.com/oauth2/authorize
description: 'Medplum''s OpenAPI does not declare an oauth2 securityScheme with a scopes map (only http basic/bearer + openIdConnect are declared), so no baseline could be mechanically derived by derive-oauth-scopes.py (0 providers with oauth2 schemes found). This file is built entirely from two live, provider-served surfaces: the RFC 8414 authorization-server metadata document (probed) and the SMART Scopes documentation page (searched).'
docs: https://www.medplum.com/docs/access/smart-scopes
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Medplum Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Medplum publishes 12 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Medplum API on a user''s behalf.


  Tokens are issued from https://api.medplum.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Medplum
provider_slug: medplum
schemes:
- flows:
  - authorizationUrl: https://api.medplum.com/oauth2/authorize
    flow: authorizationCode
    introspectionUrl: https://api.medplum.com/oauth2/introspect
    registrationUrl: https://api.medplum.com/oauth2/register
    tokenUrl: https://api.medplum.com/oauth2/token
    userinfoUrl: https://api.medplum.com/oauth2/userinfo
  - flow: clientCredentials
    tokenUrl: https://api.medplum.com/oauth2/token
  issuer: https://api.medplum.com/
  name: Medplum OAuth2 / OIDC
  source: probed https://api.medplum.com/.well-known/oauth-authorization-server
scope_count: 12
scope_names:
- openid
- profile
- email
- phone
- address
- patient/*.rs
- user/*.cruds
- fhirUser
- launch
- launch/patient
- offline_access
- online_access
scopes:
- description: OpenID Connect base scope; required to obtain an id_token.
  flows: []
  scope: openid
- description: Access to the authenticated user's profile claims.
  flows: []
  scope: profile
- description: Access to the authenticated user's email claim.
  flows: []
  scope: email
- description: Access to the authenticated user's phone claim.
  flows: []
  scope: phone
- description: Access to the authenticated user's address claim.
  flows: []
  scope: address
- description: Read and search any FHIR resource type within the launch-context patient's compartment (SMART v2 fine-grained scope syntax).
  flows: []
  scope: patient/*.rs
- description: Create, read, update, delete, and search any FHIR resource type as the authenticated user (SMART v2 fine-grained scope syntax; e.g. user/Encounter.cu grants write-only access to Encounter).
  flows: []
  scope: user/*.cruds
- description: Grants the client the authenticated user's FHIR resource reference (fhirUser claim).
  flows: []
  scope: fhirUser
- description: EHR-launch context scope (SMART App Launch, provider/EHR-initiated launch).
  flows: []
  scope: launch
- description: Standalone-launch context scope that resolves the launch patient context.
  flows: []
  scope: launch/patient
- description: Requests a refresh token so the client can obtain new access tokens without re-authentication.
  flows: []
  scope: offline_access
- description: Requests an access token valid only for the current session (no refresh token).
  flows: []
  scope: online_access
slug: medplum-scopes
source_filename: medplum-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: probed https://api.medplum.com/.well-known/oauth-authorization-server + https://api.medplum.com/.well-known/openid-configuration\ndocs: https://www.medplum.com/docs/access/smart-scopes\ndescription: >-\n  Medplum's OpenAPI does not declare an oauth2 securityScheme with a scopes map (only http\n  basic/bearer + openIdConnect are declared), so no baseline could be mechanically derived by\n  derive-oauth-scopes.py (0 providers with oauth2 schemes found). This file is built entirely\n  from two live, provider-served surfaces: the RFC 8414 authorization-server metadata document\n  (probed) and the SMART Scopes documentation page (searched).\nschemes:\n  - name: Medplum OAuth2 / OIDC\n    source: probed https://api.medplum.com/.well-known/oauth-authorization-server\n    issuer: https://api.medplum.com/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.medplum.com/oauth2/authorize\n        tokenUrl:\
  \ https://api.medplum.com/oauth2/token\n        userinfoUrl: https://api.medplum.com/oauth2/userinfo\n        introspectionUrl: https://api.medplum.com/oauth2/introspect\n        registrationUrl: https://api.medplum.com/oauth2/register\n      - flow: clientCredentials\n        tokenUrl: https://api.medplum.com/oauth2/token\ngrant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - \"urn:ietf:params:oauth:grant-type:token-exchange\"\nscopes:\n  # OIDC scopes advertised live by the authorization-server metadata document.\n  - scope: openid\n    description: OpenID Connect base scope; required to obtain an id_token.\n    sources: [probed oauth-authorization-server]\n  - scope: profile\n    description: Access to the authenticated user's profile claims.\n    sources: [probed oauth-authorization-server]\n  - scope: email\n    description: Access to the authenticated user's email claim.\n    sources: [probed oauth-authorization-server]\n  - scope: phone\n\
  \    description: Access to the authenticated user's phone claim.\n    sources: [probed oauth-authorization-server]\n  - scope: address\n    description: Access to the authenticated user's address claim.\n    sources: [probed oauth-authorization-server]\n  # SMART App Launch 2.0.0 scopes documented at docs/access/smart-scopes.\n  - scope: \"patient/*.rs\"\n    description: >-\n      Read and search any FHIR resource type within the launch-context patient's compartment\n      (SMART v2 fine-grained scope syntax).\n    sources: [docs]\n  - scope: \"user/*.cruds\"\n    description: >-\n      Create, read, update, delete, and search any FHIR resource type as the authenticated user\n      (SMART v2 fine-grained scope syntax; e.g. user/Encounter.cu grants write-only access to\n      Encounter).\n    sources: [docs]\n  - scope: fhirUser\n    description: Grants the client the authenticated user's FHIR resource reference (fhirUser claim).\n    sources: [docs]\n  - scope: launch\n    description:\
  \ EHR-launch context scope (SMART App Launch, provider/EHR-initiated launch).\n    sources: [docs]\n  - scope: launch/patient\n    description: Standalone-launch context scope that resolves the launch patient context.\n    sources: [docs]\n  - scope: offline_access\n    description: Requests a refresh token so the client can obtain new access tokens without re-authentication.\n    sources: [docs]\n  - scope: online_access\n    description: Requests an access token valid only for the current session (no refresh token).\n    sources: [docs]\nnotes: >-\n  Medplum documents SMART App Launch 2.0.0 support with the fine-grained (v2) scope syntax\n  (\"patient/Observation.r\", \"user/*.cruds\", etc.) rather than only the coarse v1 syntax\n  (\"patient/*.read\"). ClientApplication.signInForm.showScopeSelection controls whether the\n  end-user sees a scope-consent screen; ONC 170.315(g)(10) requires granular scope selection be\n  offered to patient-facing apps.\nstandard: SMART App Launch 2.0.0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medplum/refs/heads/main/scopes/medplum-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials
tags:
- Healthcare
- FHIR
- Open-Source
- Developer Platform
- HIPAA
- SMART on FHIR
- Clinical
- Interoperability
token_urls:
- https://api.medplum.com/oauth2/token
---
