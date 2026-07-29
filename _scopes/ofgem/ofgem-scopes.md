---
authorization_urls:
- https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/authorize
- https://epre-api.ofgem.gov.uk/authenticate/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ofgem Scopes
name_suffix: OAuth Scopes
note: 'Ofgem publishes no API and therefore no developer-facing scope reference. The scopes recorded here are the OAuth 2.0 / OpenID Connect scopes the two internal register applications request of their own identity providers. They are not grantable to third-party clients: neither register offers client registration, an application route or a partner programme. This artifact exists so the auth surface is recorded honestly, not because a scope catalogue is on offer.'
overview: 'Ofgem publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ofgem API on a user''s behalf.


  Tokens are issued from https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ofgem
provider_slug: ofgem
schemes:
- discovery_scopes_supported:
  - openid
  flows:
  - authorizationUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/authorize
    flow: authorizationCode
    pkce: true
    tokenUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/token
  name: RER (Renewable Electricity Register) - Azure AD B2C
  source: well-known/ofgem-rer-openid-configuration.json
- discovery_scopes_supported: null
  flows:
  - authorizationUrl: https://epre-api.ofgem.gov.uk/authenticate/
    flow: authorizationCode
    pkce: true
    tokenUrl: https://epre-api.ofgem.gov.uk/tokens/
  name: EPR (Electronic Public Register) - AWS Cognito
  source: https://epr.ofgem.gov.uk/ofgem-live-v4.20.31-28588873106-3-1/index.js
scope_count: 5
scope_names:
- openid
- profile
- email
- offline_access
- https://pk8sprdofgemcloudb2c.onmicrosoft.com/rercoreservices/user_impersonation
scopes:
- description: Standard OpenID Connect scope; requests an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC claim set - name and profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC claim - email address. Requested by the EPR only.
  flows:
  - authorizationCode
  scope: email
- description: Refresh-token issuance. Requested by the RER only.
  flows:
  - authorizationCode
  scope: offline_access
- description: Application scope for the RER core services API, delegated user impersonation. Issued only to the register's own first-party client.
  flows:
  - authorizationCode
  scope: https://pk8sprdofgemcloudb2c.onmicrosoft.com/rercoreservices/user_impersonation
slug: ofgem-scopes
source_filename: ofgem-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  well-known/ofgem-rer-openid-configuration.json (live OIDC discovery, HTTP 200) and\n  the Renewable Electricity Register / Electronic Public Register authorization\n  requests observed on 2026-07-27.\ndocs: null\nnote: >-\n  Ofgem publishes no API and therefore no developer-facing scope reference. The\n  scopes recorded here are the OAuth 2.0 / OpenID Connect scopes the two internal\n  register applications request of their own identity providers. They are not\n  grantable to third-party clients: neither register offers client registration, an\n  application route or a partner programme. This artifact exists so the auth surface\n  is recorded honestly, not because a scope catalogue is on offer.\nschemes:\n- name: RER (Renewable Electricity Register) - Azure AD B2C\n  source: well-known/ofgem-rer-openid-configuration.json\n  discovery_scopes_supported: [openid]\n  flows:\n  - flow: authorizationCode\n    pkce: true\n \
  \   authorizationUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/authorize\n    tokenUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/token\n- name: EPR (Electronic Public Register) - AWS Cognito\n  source: https://epr.ofgem.gov.uk/ofgem-live-v4.20.31-28588873106-3-1/index.js\n  discovery_scopes_supported: null\n  flows:\n  - flow: authorizationCode\n    pkce: true\n    authorizationUrl: https://epre-api.ofgem.gov.uk/authenticate/\n    tokenUrl: https://epre-api.ofgem.gov.uk/tokens/\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token.\n  flows: [authorizationCode]\n  schemes: [RER, EPR]\n  sources: [well-known/ofgem-rer-openid-configuration.json, epr bundle]\n- scope: profile\n  description: Standard OIDC claim set - name and profile claims.\n  flows: [authorizationCode]\n  schemes: [RER, EPR]\n  sources: [rer authorize\
  \ request, epr bundle]\n- scope: email\n  description: Standard OIDC claim - email address. Requested by the EPR only.\n  flows: [authorizationCode]\n  schemes: [EPR]\n  sources: [epr bundle]\n- scope: offline_access\n  description: Refresh-token issuance. Requested by the RER only.\n  flows: [authorizationCode]\n  schemes: [RER]\n  sources: [rer authorize request]\n- scope: https://pk8sprdofgemcloudb2c.onmicrosoft.com/rercoreservices/user_impersonation\n  description: >-\n    Application scope for the RER core services API, delegated user impersonation.\n    Issued only to the register's own first-party client.\n  flows: [authorizationCode]\n  schemes: [RER]\n  sources: [rer authorize request]\nclaims_supported:\n  rer: [name, email, oid, sub, tid, tfp, iss, iat, exp, aud, acr, nonce, auth_time]\nthird_party_grants: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ofgem/refs/heads/main/scopes/ofgem-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Energy Markets
- Regulator
- Smart Metering
- Open Data
- Energy Regulation
- Renewables
- Great Britain
token_urls:
- https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/token
- https://epre-api.ofgem.gov.uk/tokens/
---
