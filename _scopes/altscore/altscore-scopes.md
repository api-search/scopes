---
authorization_urls:
- https://auth.altscore.ai/oauth/authorize
description: OAuth 2.0 / OpenID Connect scopes and grant types advertised by AltScore's Frontegg-backed identity service. These are the identity-layer scopes exposed through OIDC discovery; product/API authorization is enforced per-tenant on the resource servers rather than through fine-grained OAuth scopes.
docs: https://auth.altscore.ai/.well-known/openid-configuration
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Altscore Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AltScore publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AltScore API on a user''s behalf.


  Tokens are issued from https://auth.altscore.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AltScore
provider_slug: altscore
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.altscore.ai/oauth/token
  - authorizationUrl: https://auth.altscore.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.altscore.ai/oauth/token
  issuer: https://auth.altscore.ai
  name: OpenIDConnect
  source: https://auth.altscore.ai/.well-known/openid-configuration
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email claim.
  flows:
  - authorizationCode
  scope: email
slug: altscore-scopes
source_filename: altscore-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://auth.altscore.ai/.well-known/openid-configuration\ndocs: https://auth.altscore.ai/.well-known/openid-configuration\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes and grant types advertised by AltScore's\n  Frontegg-backed identity service. These are the identity-layer scopes exposed\n  through OIDC discovery; product/API authorization is enforced per-tenant on\n  the resource servers rather than through fine-grained OAuth scopes.\nschemes:\n- name: OpenIDConnect\n  source: https://auth.altscore.ai/.well-known/openid-configuration\n  issuer: https://auth.altscore.ai\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.altscore.ai/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.altscore.ai/oauth/authorize\n    tokenUrl: https://auth.altscore.ai/oauth/token\ngrant_types_supported:\n- authorization_code\n- refresh_token\n- client_credentials\n- urn:ietf:params:oauth:grant-type:token-exchange\n\
  - urn:ietf:params:oauth:grant-type:device_code\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to the user's basic profile claims.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the user's email claim.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altscore/refs/heads/main/scopes/altscore-scopes.yml
summary_line: 3 scopes · clientCredentials/authorizationCode
tags:
- Company
- Credit
- Lending
- Fintech
- Credit Scoring
- Underwriting
- KYC
- Financial Services
- Latin America
- Data Aggregation
- Workflows
- Decisioning
token_urls:
- https://auth.altscore.ai/oauth/token
---
