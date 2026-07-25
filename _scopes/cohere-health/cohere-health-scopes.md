---
authorization_urls:
- https://login.coherehealth.com/oauth2/v1/authorize
description: ''
docs: https://www.coherehealth.com/utilization-management/api-based
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cohere Health Scopes
name_suffix: OAuth Scopes
note: These are the standard OIDC scopes advertised by the Cohere platform login host (login.coherehealth.com, an Okta-backed identity tenant) that governs access to the Cohere Unify platform / provider portal. They are NOT the per-health-plan SMART-on-FHIR API scopes for the CRD/DTR/PAS FHIR APIs, which are provisioned per tenant and not published anonymously (SMART on FHIR patient/*, user/*, system/* scopes per the Da Vinci implementation guides).
overview: 'Cohere Health publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cohere Health API on a user''s behalf.


  Tokens are issued from https://login.coherehealth.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cohere Health
provider_slug: cohere-health
schemes:
- flows:
  - authorizationUrl: https://login.coherehealth.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://login.coherehealth.com/oauth2/v1/token
  name: OpenIDConnect
  source: well-known/cohere-health-openid-configuration.json
scope_count: 7
scope_names:
- openid
- email
- profile
- address
- phone
- groups
- offline_access
scopes:
- description: OpenID Connect sign-in; returns an ID token identifying the user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access to the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's address claim.
  flows:
  - authorizationCode
  scope: address
- description: Access to the user's phone number claim.
  flows:
  - authorizationCode
  scope: phone
- description: Access to the user's group memberships.
  flows:
  - authorizationCode
  scope: groups
- description: Issue a refresh token so the client can obtain new access tokens without re-prompting.
  flows:
  - authorizationCode
  scope: offline_access
slug: cohere-health-scopes
source_filename: cohere-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://login.coherehealth.com/.well-known/openid-configuration\ndocs: https://www.coherehealth.com/utilization-management/api-based\nnote: >-\n  These are the standard OIDC scopes advertised by the Cohere platform login\n  host (login.coherehealth.com, an Okta-backed identity tenant) that governs\n  access to the Cohere Unify platform / provider portal. They are NOT the\n  per-health-plan SMART-on-FHIR API scopes for the CRD/DTR/PAS FHIR APIs, which\n  are provisioned per tenant and not published anonymously (SMART on FHIR\n  patient/*, user/*, system/* scopes per the Da Vinci implementation guides).\nschemes:\n  - name: OpenIDConnect\n    source: well-known/cohere-health-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.coherehealth.com/oauth2/v1/authorize\n        tokenUrl: https://login.coherehealth.com/oauth2/v1/token\nscopes:\n  - scope: openid\n    description:\
  \ OpenID Connect sign-in; returns an ID token identifying the user.\n    flows: [authorizationCode]\n  - scope: email\n    description: Access to the user's email address claim.\n    flows: [authorizationCode]\n  - scope: profile\n    description: Access to the user's basic profile claims.\n    flows: [authorizationCode]\n  - scope: address\n    description: Access to the user's address claim.\n    flows: [authorizationCode]\n  - scope: phone\n    description: Access to the user's phone number claim.\n    flows: [authorizationCode]\n  - scope: groups\n    description: Access to the user's group memberships.\n    flows: [authorizationCode]\n  - scope: offline_access\n    description: Issue a refresh token so the client can obtain new access tokens without re-prompting.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cohere-health/refs/heads/main/scopes/cohere-health-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Healthcare
- United States
- Prior Authorization
- Utilization Management
- Payer
- FHIR
- HL7
- Da Vinci
- SMART on FHIR
- Interoperability
token_urls:
- https://login.coherehealth.com/oauth2/v1/token
---
