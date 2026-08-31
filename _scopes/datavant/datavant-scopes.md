---
api_specs:
- filename: datavant-configuration-api-openapi.yml
  format: yaml
  label: Datavant Configuration API
  slug: datavant-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-configuration-api-openapi.yml
- filename: datavant-documents-api-openapi.yml
  format: yaml
  label: Datavant Documents API
  slug: datavant-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-documents-api-openapi.yml
- filename: datavant-oauth2-api-openapi.yml
  format: yaml
  label: Datavant Oauth2 API
  slug: datavant-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-oauth2-api-openapi.yml
- filename: datavant-order-queries-api-openapi.yml
  format: yaml
  label: Datavant Order Queries API
  slug: datavant-order-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-order-queries-api-openapi.yml
- filename: datavant-orders-api-openapi.yml
  format: yaml
  label: Datavant Orders API
  slug: datavant-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-orders-api-openapi.yml
- filename: datavant-prematch-api-openapi.yml
  format: yaml
  label: Datavant Prematch API
  slug: datavant-prematch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-prematch-api-openapi.yml
- filename: datavant-projects-api-openapi.yml
  format: yaml
  label: Datavant Projects API
  slug: datavant-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-projects-api-openapi.yml
- filename: datavant-visits-api-openapi.yml
  format: yaml
  label: Datavant Visits API
  slug: datavant-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-visits-api-openapi.yml
authorization_urls:
- https://datavant.auth0.com/authorize
description: ''
docs: https://auth.datavant.com/.well-known/openid-configuration
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Datavant Scopes
name_suffix: OAuth Scopes
note: 'The Datavant REST API declares an oauth2 clientCredentials scheme with an EMPTY scopes map, and no operation narrows security[], so the REST contract publishes ZERO API scopes - a token is all-or-nothing across all 54 operations. The scopes recorded below are the OIDC scopes advertised by Datavant''s Auth0 tenant (probed anonymously at auth.datavant.com/.well-known/openid-configuration and captured verbatim to well-known/datavant-openid-configuration.json). They are identity/profile scopes for the Portal login flow, NOT authorization scopes for the record-retrieval API. This distinction is the finding: there is no published least-privilege surface for the REST API.'
overview: 'Datavant uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.datavant.io/v2/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Datavant
provider_slug: datavant
schemes:
- flows:
  - flow: clientCredentials
    refreshUrl: https://api.datavant.io/v2/oauth2/token
    scopes_declared: 0
    tokenUrl: https://api.datavant.io/v2/oauth2/token
  kind: api
  name: oauth2
  source: openapi/datavant-rest-api-openapi.yml
- flows:
  - authorizationUrl: https://datavant.auth0.com/authorize
    flow: authorizationCode
    scopes_declared: 14
    tokenUrl: https://datavant.auth0.com/oauth/token
  issuer: https://datavant.auth0.com/
  kind: identity
  name: auth0-oidc
  source: well-known/datavant-openid-configuration.json
scope_count: 0
scope_names: []
scopes: []
slug: datavant-scopes
source_filename: datavant-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: openapi/datavant-rest-api-openapi.yml\ndocs: https://auth.datavant.com/.well-known/openid-configuration\nnote: >-\n  The Datavant REST API declares an oauth2 clientCredentials scheme with an EMPTY scopes map,\n  and no operation narrows security[], so the REST contract publishes ZERO API scopes - a\n  token is all-or-nothing across all 54 operations. The scopes recorded below are the OIDC\n  scopes advertised by Datavant's Auth0 tenant (probed anonymously at\n  auth.datavant.com/.well-known/openid-configuration and captured verbatim to\n  well-known/datavant-openid-configuration.json). They are identity/profile scopes for the\n  Portal login flow, NOT authorization scopes for the record-retrieval API. This distinction\n  is the finding: there is no published least-privilege surface for the REST API.\nschemes:\n  - name: oauth2\n    source: openapi/datavant-rest-api-openapi.yml\n    kind: api\n    flows:\n      - flow: clientCredentials\n\
  \        tokenUrl: https://api.datavant.io/v2/oauth2/token\n        refreshUrl: https://api.datavant.io/v2/oauth2/token\n        scopes_declared: 0\n  - name: auth0-oidc\n    source: well-known/datavant-openid-configuration.json\n    kind: identity\n    issuer: https://datavant.auth0.com/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://datavant.auth0.com/authorize\n        tokenUrl: https://datavant.auth0.com/oauth/token\n        scopes_declared: 14\napi_scopes: []\napi_scope_count: 0\nidentity_scopes:\n  - scope: openid\n    description: Request an ID token (OIDC core).\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n  - scope: profile\n    description: Basic profile claims.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n  - scope: offline_access\n    description: Issue a refresh token.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n\
  \  - scope: name\n    description: Full name claim.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n  - scope: given_name\n    description: Given name claim.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n  - scope: family_name\n    description: Family name claim.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n  - scope: nickname\n    description: Nickname claim.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n  - scope: email\n    description: Email address claim.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n  - scope: email_verified\n    description: Email verification status claim.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n  - scope: picture\n    description: Profile picture claim.\n    flows: [authorizationCode]\n\
  \    sources: [well-known/datavant-openid-configuration.json]\n  - scope: created_at\n    description: Account creation timestamp claim.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n  - scope: identities\n    description: Linked identity providers claim.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n  - scope: phone\n    description: Phone number claim.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\n  - scope: address\n    description: Address claim.\n    flows: [authorizationCode]\n    sources: [well-known/datavant-openid-configuration.json]\nidentity_scope_count: 14\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/scopes/datavant-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Healthcare
- United States
- Interoperability
- Health Data
- De-Identification
- Tokenization
- Real-World Data
- Record Retrieval
- Data Connectivity
- Life Sciences
- HIPAA
- Medical Records
- Release of Information
- Privacy
- Authentication
- Health Information Exchange
token_urls:
- https://api.datavant.io/v2/oauth2/token
- https://datavant.auth0.com/oauth/token
---
