---
api_specs:
- filename: medblocks-platform-openapi.json
  format: json
  label: Medblocks Platform API
  slug: medblocks-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medblocks/refs/heads/main/openapi/medblocks-platform-openapi.json
- filename: medblocks-public-site-openapi.json
  format: json
  label: Medblocks Public Site API
  slug: medblocks-public-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medblocks/refs/heads/main/openapi/medblocks-public-site-openapi.json
authorization_urls: []
description: ''
docs: https://medblocks.com/docs/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Medblocks Scopes
name_suffix: OAuth Scopes
note: These scopes are NOT declared in openapi/medblocks-platform-openapi.json, which secures every operation with a single bearer API key (BearerAuth). They belong to the OAuth authorization server that fronts the hosted MCP server, and they were read from the provider's own RFC 8414 and RFC 9728 metadata documents plus the RFC 6750 challenge the MCP endpoint returns to an unauthenticated caller. The three tick boxes a user sees on the consent screen are a product-level grouping over these scopes; the mapping between the two is not published, so the consent grouping is recorded separately rather than asserted against individual scopes.
overview: 'Medblocks uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Medblocks
provider_slug: medblocks
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: medblocks-scopes
source_filename: medblocks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  https://app.medblocks.com/.well-known/oauth-authorization-server,\n  https://app.medblocks.com/.well-known/oauth-protected-resource/mcp,\n  WWW-Authenticate challenge from POST https://app.medblocks.com/mcp\ndocs: https://medblocks.com/docs/mcp\nnote: >-\n  These scopes are NOT declared in openapi/medblocks-platform-openapi.json, which secures every\n  operation with a single bearer API key (BearerAuth). They belong to the OAuth authorization\n  server that fronts the hosted MCP server, and they were read from the provider's own RFC 8414\n  and RFC 9728 metadata documents plus the RFC 6750 challenge the MCP endpoint returns to an\n  unauthenticated caller. The three tick boxes a user sees on the consent screen are a\n  product-level grouping over these scopes; the mapping between the two is not published, so the\n  consent grouping is recorded separately rather than asserted against individual scopes.\nauthorization_server:\n\
  \  issuer: https://app.medblocks.com/api/auth\n  authorization_endpoint: https://app.medblocks.com/api/auth/oauth2/authorize\n  token_endpoint: https://app.medblocks.com/api/auth/oauth2/token\n  jwks_uri: https://app.medblocks.com/api/auth/jwks\n  registration_endpoint: https://app.medblocks.com/api/auth/oauth2/register\n  introspection_endpoint: https://app.medblocks.com/api/auth/oauth2/introspect\n  revocation_endpoint: https://app.medblocks.com/api/auth/oauth2/revoke\n  userinfo_endpoint: https://app.medblocks.com/api/auth/oauth2/userinfo\n  end_session_endpoint: https://app.medblocks.com/api/auth/oauth2/end-session\n  grant_types: [authorization_code, client_credentials, refresh_token]\n  code_challenge_methods: [S256]\n  id_token_signing_alg: [EdDSA]\nprotected_resource:\n  resource: https://app.medblocks.com/mcp\n  authorization_servers: [https://app.medblocks.com/api/auth]\n  bearer_methods: [header]\nscope_count: 10\nscopes:\n- name: openid\n  description: OpenID Connect authentication;\
  \ issues an ID token identifying the signed-in user.\n  category: identity\n- name: profile\n  description: Standard OIDC profile claims (name, picture, family_name, given_name).\n  category: identity\n- name: email\n  description: Standard OIDC email claims (email, email_verified).\n  category: identity\n- name: offline_access\n  description: Issues a refresh token so the client can keep access without re-prompting.\n  category: session\n- name: patients:read\n  description: Read patients (the \"people\" in the MCP surface) in the workspace.\n  category: patients\n  rest_equivalent: [api.listPatients, api.getPatient]\n- name: patients:write\n  description: Create, update and delete patients in the workspace.\n  category: patients\n  rest_equivalent: [api.createPatient, api.updatePatient, api.deletePatient]\n- name: patient_sessions:read\n  description: Read patient authorization sessions and their status.\n  category: patient-sessions\n  rest_equivalent: [api.listPatientSessionsForPatient,\
  \ api.retrievePatientSession]\n- name: patient_sessions:write\n  description: Start a patient authorization session against one or more sources.\n  category: patient-sessions\n  rest_equivalent: [api.initPatientSession]\n- name: connections:read\n  description: Read the EHR/FHIR source catalog and the workspace's configured connections.\n  category: connections\n  rest_equivalent: [api.listFhirSources, api.getFhirSource]\n- name: fhir:read\n  description: Read the patient's stored FHIR records.\n  category: records\n  rest_equivalent: [api.getPatientRecords]\nconsent_screen:\n  note: >-\n    Interactive OAuth users are shown three tick boxes rather than raw scopes. All three are\n    ticked by default and a user may grant fewer than requested; identity and workspace\n    visibility are granted without a prompt.\n  choices:\n  - label: Connect your healthcare facilities\n    default: on\n  - label: Read your health records\n    default: on\n  - label: Manage people and delete data\n   \
  \ default: on\n    destructive: true\napi_key_alternative: >-\n  A developer client may send an mb_sk_ API key as a bearer token instead of running the OAuth\n  flow. The docs state a key uses the permissions stamped on it rather than these consent\n  scopes, and that a key connection stays bound to the workspace that minted it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medblocks/refs/heads/main/scopes/medblocks-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Health
- Healthcare
- FHIR
- openEHR
- Interoperability
- Electronic Health Records
- Patient Access
- Health Data
- SMART on FHIR
- Webhooks
- Model Context Protocol
- Company
token_urls: []
---
