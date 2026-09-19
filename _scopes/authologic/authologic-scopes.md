---
api_specs:
- filename: authologic-aml-api-openapi.yml
  format: yaml
  label: Authologic AML API
  slug: authologic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-aml-api-openapi.yml
- filename: authologic-advanced-api-openapi.yml
  format: yaml
  label: Authologic Advanced API
  slug: authologic-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-advanced-api-openapi.yml
- filename: authologic-affordability-assessment-api-openapi.yml
  format: yaml
  label: Authologic Affordability assessment API
  slug: authologic-affordability-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-affordability-assessment-api-openapi.yml
- filename: authologic-aml-api-openapi.yml
  format: yaml
  label: Authologic AML API
  slug: authologic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-aml-api-openapi.yml
- filename: authologic-bank-api-openapi.yml
  format: yaml
  label: Authologic Bank API
  slug: authologic-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-bank-api-openapi.yml
- filename: authologic-conversation-api-openapi.yml
  format: yaml
  label: Authologic Conversation API
  slug: authologic-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-conversation-api-openapi.yml
- filename: authologic-database-verification-api-openapi.yml
  format: yaml
  label: Authologic Database Verification API
  slug: authologic-database-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-database-verification-api-openapi.yml
- filename: authologic-enterprise-integration-api-openapi.yml
  format: yaml
  label: Authologic Enterprise Integration API
  slug: authologic-enterprise-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-enterprise-integration-api-openapi.yml
- filename: authologic-metadata-api-openapi.yml
  format: yaml
  label: Authologic Metadata API
  slug: authologic-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/openapi/authologic-metadata-api-openapi.yml
authorization_urls: []
description: Authologic operates an OAuth 2.0 authorization server but publishes no scopes. This artifact records that measured absence rather than omitting the file, because "OAuth exists but is unscoped" is a materially different fact from "no OAuth".
docs: https://developer.authologic.com/docs/technical/implementation
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Authologic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Authologic uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sandbox.authologic.com/api/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Authologic
provider_slug: authologic
schemes:
- flows:
  - flow: clientCredentials
    scopes: {}
    tokenUrl: https://sandbox.authologic.com/api/oauth2/token
  name: oauth2
  source: openapi/authologic-customer-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: authologic-scopes
source_filename: authologic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: openapi/authologic-customer-api-openapi.yml (components.securitySchemes.oauth2),\n  well-known/authologic-sandbox-oauth-authorization-server.json (RFC 8414, probed 2026-09-14),\n  https://developer.authologic.com/sitemap.xml (95 URLs, no scopes or permissions page),\n  https://developer.authologic.com/docs/technical/implementation\ndocs: https://developer.authologic.com/docs/technical/implementation\nspecification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Authologic\nproviderId: authologic\nscope_count: 0\ndescription: >-\n  Authologic operates an OAuth 2.0 authorization server but publishes no scopes. This artifact records\n  that measured absence rather than omitting the file, because \"OAuth exists but is unscoped\" is a\n  materially different fact from \"no OAuth\".\nschemes:\n  - name: oauth2\n    source: openapi/authologic-customer-api-openapi.yml\n    flows:\n      - flow: clientCredentials\n\
  \        tokenUrl: https://sandbox.authologic.com/api/oauth2/token\n        scopes: {}\nscopes: []\nfindings:\n  - >-\n    The clientCredentials flow in the contract declares an EMPTY scopes object. No operation carries a\n    per-operation scope requirement — security is declared once at the document level as\n    [{apiKey: []}, {oauth2: []}] and every operation inherits it with an empty scope list.\n  - >-\n    The RFC 8414 authorization server metadata at\n    https://sandbox.authologic.com/.well-known/oauth-authorization-server omits scopes_supported\n    entirely. An RFC 8414 server that supported scopes would normally advertise them there.\n  - >-\n    No scopes, permissions or roles reference page exists in the developer documentation. All 95 URLs in\n    the sitemap were checked; the implementation notes cover authentication without mentioning scopes.\n  - >-\n    Authorization is therefore account- and environment-scoped. A credential is entitled to the products\n    the account\
  \ has contracted for, in the environment the key belongs to. There is no way to mint a\n    narrower token — a token that can read a conversation can also create one and delete its data.\nimplication_for_agents: >-\n  Least privilege is not achievable on this API today. An agent given credentials to read verification\n  results holds the same authority as one permitted to create billable conversations and to issue\n  DELETE_DATA. The mitigation available now is operational, not contractual: separate accounts per use\n  case, and the mTLS/DPoP binding the authorization server advertises (see\n  authentication/authologic-authentication.yml) to at least bind the credential to a workload.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authologic/refs/heads/main/scopes/authologic-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AML
- Digital Identity
- eID
- Identity Verification
- KYB
- KYC
- Liveness Check
token_urls:
- https://sandbox.authologic.com/api/oauth2/token
---
