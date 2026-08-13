---
api_specs:
- filename: dust-identity-apid-openapi.yml
  format: yaml
  label: DUST API
  slug: dust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dust-identity/refs/heads/main/openapi/dust-identity-apid-openapi.yml
authorization_urls:
- https://authd.dustid.io/api/auth/oauth2/authorize
description: ''
docs: https://docs.dustid.io/api/authentication/
flows:
- authorizationCode
- refreshToken
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Dust Identity Scopes
name_suffix: OAuth Scopes
note: 'The DUST API''s own OpenAPI declares a single `Bearer` http/JWT scheme with no oauth2 block, so the mechanical derivation from the spec found zero scopes. The scope surface is instead published by AuthD, the account service, in its OpenID Connect discovery document — which is anonymous and was fetched directly. Two facts a consumer needs: (1) the DUST API does not perform per-scope authorization on /api/v1/* — authorization is evaluated from the Service Account''s team memberships and grants, named by the Dust-Ctx-Org-Id / Dust-Ctx-Team-Id context headers, not from token scopes; (2) the non-OIDC entries in scopes_supported below, `read:widgets` and `write:widgets`, are the stock placeholder scopes shipped by the underlying auth library and do not correspond to any documented DUST capability. They are recorded verbatim because the provider serves them, and flagged because an integrator should not build against them.'
overview: 'Dust Identity publishes 6 OAuth 2.0 scopes via the authorizationCode, refreshToken, and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dust Identity API on a user''s behalf.


  Tokens are issued from https://authd.dustid.io/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dust Identity
provider_slug: dust-identity
schemes:
- end_session_endpoint: https://authd.dustid.io/api/auth/oauth2/end-session
  flows:
  - authorizationUrl: https://authd.dustid.io/api/auth/oauth2/authorize
    flow: authorizationCode
    pkce:
    - S256
    response_modes:
    - query
    response_types:
    - code
    tokenUrl: https://authd.dustid.io/api/auth/oauth2/token
  - flow: refreshToken
    tokenUrl: https://authd.dustid.io/api/auth/oauth2/token
  - flow: clientCredentials
    note: The Service Account client_credentials endpoint is documented on the authentication page but is not listed in the OIDC discovery document, which advertises only authorization_code and refresh_token. This is the grant enterprise middleware (SAP Integration Suite, MuleSoft, Boomi) is directed to use.
    source: https://docs.dustid.io/api/authentication/
    tokenUrl: https://authd.dustid.io/api/auth/dust/service-accounts/token
  id_token_signing_alg:
  - EdDSA
  introspection_endpoint: https://authd.dustid.io/api/auth/oauth2/introspect
  issuer: https://authd.dustid.io/api/auth
  jwks_uri: https://authd.dustid.io/api/auth/jwks
  name: DUST AuthD OpenID Connect
  revocation_endpoint: https://authd.dustid.io/api/auth/oauth2/revoke
  source: well-known/dust-identity-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  userinfo_endpoint: https://authd.dustid.io/api/auth/oauth2/userinfo
scope_count: 6
scope_names:
- openid
- email
- profile
- offline_access
- read:widgets
- write:widgets
scopes:
- description: Standard OpenID Connect scope — request an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Release the `email` and `email_verified` claims.
  flows:
  - authorizationCode
  scope: email
- description: Release the `name`, `picture`, `given_name` and `family_name` claims.
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh token so the client can renew without user interaction.
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
- description: ''
  flows:
  - authorizationCode
  scope: read:widgets
- description: ''
  flows:
  - authorizationCode
  scope: write:widgets
slug: dust-identity-scopes
source_filename: dust-identity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://authd.dustid.io/.well-known/openid-configuration\ndocs: https://docs.dustid.io/api/authentication/\nnote: >-\n  The DUST API's own OpenAPI declares a single `Bearer` http/JWT scheme with no oauth2\n  block, so the mechanical derivation from the spec found zero scopes. The scope surface\n  is instead published by AuthD, the account service, in its OpenID Connect discovery\n  document — which is anonymous and was fetched directly. Two facts a consumer needs:\n  (1) the DUST API does not perform per-scope authorization on /api/v1/* — authorization\n  is evaluated from the Service Account's team memberships and grants, named by the\n  Dust-Ctx-Org-Id / Dust-Ctx-Team-Id context headers, not from token scopes; (2) the\n  non-OIDC entries in scopes_supported below, `read:widgets` and `write:widgets`, are\n  the stock placeholder scopes shipped by the underlying auth library and do not\n  correspond to any documented DUST capability.\
  \ They are recorded verbatim because the\n  provider serves them, and flagged because an integrator should not build against them.\nschemes:\n- name: DUST AuthD OpenID Connect\n  source: well-known/dust-identity-openid-configuration.json\n  issuer: https://authd.dustid.io/api/auth\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authd.dustid.io/api/auth/oauth2/authorize\n    tokenUrl: https://authd.dustid.io/api/auth/oauth2/token\n    pkce: [S256]\n    response_types: [code]\n    response_modes: [query]\n  - flow: refreshToken\n    tokenUrl: https://authd.dustid.io/api/auth/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://authd.dustid.io/api/auth/dust/service-accounts/token\n    source: https://docs.dustid.io/api/authentication/\n    note: >-\n      The Service Account client_credentials endpoint is documented on the authentication\n      page but is not listed in the OIDC discovery document, which advertises only\n      authorization_code and refresh_token.\
  \ This is the grant enterprise middleware\n      (SAP Integration Suite, MuleSoft, Boomi) is directed to use.\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  introspection_endpoint: https://authd.dustid.io/api/auth/oauth2/introspect\n  revocation_endpoint: https://authd.dustid.io/api/auth/oauth2/revoke\n  userinfo_endpoint: https://authd.dustid.io/api/auth/oauth2/userinfo\n  jwks_uri: https://authd.dustid.io/api/auth/jwks\n  end_session_endpoint: https://authd.dustid.io/api/auth/oauth2/end-session\n  id_token_signing_alg: [EdDSA]\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope — request an ID token.\n  flows: [authorizationCode]\n  standard: oidc\n  sources: [well-known/dust-identity-openid-configuration.json]\n- scope: email\n  description: Release the `email` and `email_verified` claims.\n  flows: [authorizationCode]\n  standard: oidc\n  sources: [well-known/dust-identity-openid-configuration.json]\n- scope: profile\n  description:\
  \ Release the `name`, `picture`, `given_name` and `family_name` claims.\n  flows: [authorizationCode]\n  standard: oidc\n  sources: [well-known/dust-identity-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can renew without user interaction.\n  flows: [authorizationCode, refreshToken]\n  standard: oidc\n  sources: [well-known/dust-identity-openid-configuration.json]\n- scope: read:widgets\n  description: null\n  flows: [authorizationCode]\n  standard: null\n  status: placeholder\n  sources: [well-known/dust-identity-openid-configuration.json]\n  note: >-\n    Advertised in scopes_supported but undocumented and unmapped to any DUST resource.\n    \"Widgets\" is the stock example scope of the auth library; DUST has no widget\n    resource. Do not build against it.\n- scope: write:widgets\n  description: null\n  flows: [authorizationCode]\n  standard: null\n  status: placeholder\n  sources: [well-known/dust-identity-openid-configuration.json]\n\
  \  note: See read:widgets — placeholder scope, not a DUST capability.\nclaims_supported: [sub, iss, aud, exp, iat, sid, scope, azp, email, email_verified,\n  name, picture, family_name, given_name]\nacr_values_supported: [urn:mace:incommon:iap:bronze]\nprompt_values_supported: [login, consent, create, select_account, none]\nauthorization_model:\n  api_authorization: team-membership\n  detail: >-\n    /api/v1/* authorization is evaluated for the caller acting in the team named by the\n    Dust-Ctx-Team-Id header — what it can list, read and write is that team's own records\n    plus whatever has been shared with it. OAuth scopes do not gate DUST API operations.\n  see: conventions/dust-identity-conventions.yml\nsummary:\n  scope_count: 6\n  oidc_standard_scopes: 4\n  dust_specific_scopes: 0\n  placeholder_scopes: 2\n  api_gated_by_scopes: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dust-identity/refs/heads/main/scopes/dust-identity-scopes.yml
summary_line: 6 scopes · authorizationCode/refreshToken/clientCredentials
tags:
- Authentication
- Identity
- Supply Chain
- Traceability
- Provenance
- Anti-Counterfeiting
- Asset Tracking
- Aerospace and Defense
- Manufacturing
- Security
token_urls:
- https://authd.dustid.io/api/auth/oauth2/token
- https://authd.dustid.io/api/auth/dust/service-accounts/token
---
