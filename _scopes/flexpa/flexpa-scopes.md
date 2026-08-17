---
api_specs:
- filename: flexpa-access-tokens-api-openapi.yml
  format: yaml
  label: Flexpa Access Tokens API
  slug: flexpa-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-access-tokens-api-openapi.yml
- filename: flexpa-claims-data-api-openapi.yml
  format: yaml
  label: Flexpa Claims Data API
  slug: flexpa-claims-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-claims-data-api-openapi.yml
- filename: flexpa-fhir-api-openapi.yml
  format: yaml
  label: Flexpa FHIR API
  slug: flexpa-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-fhir-api-openapi.yml
- filename: flexpa-link-api-openapi.yml
  format: yaml
  label: Flexpa Link API
  slug: flexpa-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-link-api-openapi.yml
authorization_urls:
- https://api.flexpa.com/oauth/authorize
description: ''
docs: https://www.flexpa.com/docs/consent
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Flexpa Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Flexpa uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.flexpa.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flexpa
provider_slug: flexpa
schemes:
- flows:
  - authorizationUrl: https://api.flexpa.com/oauth/authorize
    flow: authorizationCode
    note: Produces a Patient Access Token via the Flexpa Consent experience.
    pkce: S256
    tokenUrl: https://api.flexpa.com/oauth/token
  - flow: clientCredentials
    note: Produces an Application Access Token (server-to-server), authenticated with HTTP Basic using publishable key as username and secret key as password.
    tokenUrl: https://api.flexpa.com/oauth/token
  - flow: refreshToken
    tokenUrl: https://api.flexpa.com/oauth/token
  issuer: https://api.flexpa.com
  jwks_uri: https://api.flexpa.com/.well-known/jwks.json
  name: OAuth 2.0 / SMART on FHIR
  registration_endpoint: https://api.flexpa.com/oauth/register
  source: https://api.flexpa.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - client_secret_basic
  - none
scope_count: 0
scope_names: []
scopes: []
slug: flexpa-scopes
source_filename: flexpa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://api.flexpa.com/.well-known/oauth-authorization-server\ndocs: https://www.flexpa.com/docs/consent\nprovider: Flexpa\nproviderId: flexpa\nsummary: >-\n  Flexpa's OAuth scope surface is SMART on FHIR's, not a bespoke permission\n  taxonomy: exactly two scopes are advertised by the authorization server, and\n  both were read from live discovery documents rather than inferred. The captured\n  OpenAPI declares only a bearer scheme, so this artifact is the only place the\n  scope contract is recorded.\nschemes:\n- name: OAuth 2.0 / SMART on FHIR\n  source: https://api.flexpa.com/.well-known/oauth-authorization-server\n  issuer: https://api.flexpa.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.flexpa.com/oauth/authorize\n    tokenUrl: https://api.flexpa.com/oauth/token\n    pkce: S256\n    note: Produces a Patient Access Token via the Flexpa Consent experience.\n  - flow: clientCredentials\n \
  \   tokenUrl: https://api.flexpa.com/oauth/token\n    note: >-\n      Produces an Application Access Token (server-to-server), authenticated with\n      HTTP Basic using publishable key as username and secret key as password.\n  - flow: refreshToken\n    tokenUrl: https://api.flexpa.com/oauth/token\n  registration_endpoint: https://api.flexpa.com/oauth/register\n  jwks_uri: https://api.flexpa.com/.well-known/jwks.json\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - none\nscopes:\n- name: launch/patient\n  description: >-\n    SMART on FHIR standalone patient launch context. Required on every\n    authorization URL; grants read access to the authorizing patient's compartment\n    (Patient, Coverage, ExplanationOfBenefit and the clinical resources Flexpa\n    derives).\n  required: true\n  surfaces:\n  - https://api.flexpa.com/fhir\n  - https://api.flexpa.com/mcp\n- name: offline_access\n  description: >-\n    Issues a refresh token so the application can continue retrieving\
  \ the\n    patient's data after the initial access token expires. Corresponds to the\n    permission-offline SMART capability.\n  required: false\n  surfaces:\n  - https://api.flexpa.com/fhir\n  - https://api.flexpa.com/mcp\nsmart_capabilities:\n- launch-standalone\n- client-public\n- client-confidential-symmetric\n- context-standalone-patient\n- permission-offline\n- permission-patient\nnotes: >-\n  Scope granularity is patient-compartment-wide; there is no per-resource scope\n  (no patient/ExplanationOfBenefit.read style scopes) and no scope that\n  distinguishes claims from clinical data. The MCP server at\n  https://api.flexpa.com/mcp is protected by the same two scopes, per\n  /.well-known/oauth-protected-resource.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/scopes/flexpa-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Healthcare
- FHIR
- Patient Access
- Claims Data
- Health Insurance
token_urls:
- https://api.flexpa.com/oauth/token
---
