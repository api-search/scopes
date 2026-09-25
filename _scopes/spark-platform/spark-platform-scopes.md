---
authorization_urls:
- https://sparkplatform.com/openid/authorize
description: 'Spark Platform''s OAuth/OIDC scope surface, read from the live OpenID Connect discovery document (HTTP 200, harvested verbatim to authentication/spark-platform-openid-configuration.json). Scopes govern the identity surface only — the seven advertised scopes are the standard OIDC set plus two vendor scopes, RESO and FBS. Data authorization on the Spark API and RESO Web API is not scope-based: it is governed by the role assigned to the API key (IDX, VOW, Private, Public, Portal) and by the MLS data plans the developer has been approved for. No published scope-to-resource reference page was found, so scope descriptions below the standard OIDC four are recorded as undocumented rather than guessed.'
docs: https://sparkplatform.com/docs/authentication/openid_connect_authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Spark Platform Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Spark Platform publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Spark Platform API on a user''s behalf.


  Tokens are issued from https://sparkplatform.com/openid/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spark Platform
provider_slug: spark-platform
schemes:
- flows:
  - authorizationUrl: https://sparkplatform.com/openid/authorize
    flow: authorizationCode
    revocationUrl: https://sparkplatform.com/openid/revoke
    tokenUrl: https://sparkplatform.com/openid/token
  issuer: https://sparkplatform.com
  name: Spark OpenID Connect
  source: https://sparkplatform.com/.well-known/openid-configuration
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- RESO
- FBS
scopes:
- description: Standard OIDC scope — requests an ID token for the authenticating flexmls member.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC profile claims (name, given_name, family_name, middle_name, preferred_username, picture, website, zoneinfo) plus Spark's MemberNameSuffix.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Standard OIDC address claim.
  flows:
  - authorizationCode
  scope: address
- description: Standard OIDC phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  scope: phone
- description: Vendor scope. Advertised in scopes_supported; no published description was found. Associated with the RESO-standard member identity claims (MemberMlsId, MemberNrdsId, MemberStateLicense, MemberAOR, MemberAORkey, MemberPrimaryAorId, MemberPrimaryAorKey, MemberType, MemberStatus, OfficeKey, OfficeMlsId).
  flows:
  - authorizationCode
  scope: RESO
- description: Vendor scope. Advertised in scopes_supported; no published description was found. Associated with the Flexmls-proprietary claims (FlexmlsMemberType, UserType, UserLevel, mls_system_access, user_is_visible, user_is_enabled, user_is_active, user_is_billable, user_profile_visible).
  flows:
  - authorizationCode
  scope: FBS
slug: spark-platform-scopes
source_filename: spark-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://sparkplatform.com/.well-known/openid-configuration\ndocs: https://sparkplatform.com/docs/authentication/openid_connect_authentication\ndescription: >-\n  Spark Platform's OAuth/OIDC scope surface, read from the live OpenID Connect discovery\n  document (HTTP 200, harvested verbatim to\n  authentication/spark-platform-openid-configuration.json). Scopes govern the identity surface\n  only — the seven advertised scopes are the standard OIDC set plus two vendor scopes, RESO and\n  FBS. Data authorization on the Spark API and RESO Web API is not scope-based: it is governed\n  by the role assigned to the API key (IDX, VOW, Private, Public, Portal) and by the MLS data\n  plans the developer has been approved for. No published scope-to-resource reference page was\n  found, so scope descriptions below the standard OIDC four are recorded as undocumented rather\n  than guessed.\nschemes:\n  - name: Spark OpenID Connect\n    type:\
  \ openIdConnect\n    source: https://sparkplatform.com/.well-known/openid-configuration\n    issuer: https://sparkplatform.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://sparkplatform.com/openid/authorize\n        tokenUrl: https://sparkplatform.com/openid/token\n        revocationUrl: https://sparkplatform.com/openid/revoke\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n\nscopes:\n  - {scope: openid, description: \"Standard OIDC scope — requests an ID token for the authenticating flexmls member.\", flows: [authorizationCode], sources: [.well-known/openid-configuration]}\n  - {scope: profile, description: \"Standard OIDC profile claims (name, given_name, family_name, middle_name, preferred_username, picture, website, zoneinfo) plus Spark's MemberNameSuffix.\", flows: [authorizationCode], sources: [.well-known/openid-configuration]}\n  - {scope: email, description: Standard OIDC email and email_verified claims., flows: [authorizationCode],\
  \ sources: [.well-known/openid-configuration]}\n  - {scope: address, description: Standard OIDC address claim., flows: [authorizationCode], sources: [.well-known/openid-configuration]}\n  - {scope: phone, description: Standard OIDC phone_number and phone_number_verified claims., flows: [authorizationCode], sources: [.well-known/openid-configuration]}\n  - {scope: RESO, description: \"Vendor scope. Advertised in scopes_supported; no published description was found. Associated with the RESO-standard member identity claims (MemberMlsId, MemberNrdsId, MemberStateLicense, MemberAOR, MemberAORkey, MemberPrimaryAorId, MemberPrimaryAorKey, MemberType, MemberStatus, OfficeKey, OfficeMlsId).\", flows: [authorizationCode], sources: [.well-known/openid-configuration], documented: false}\n  - {scope: FBS, description: \"Vendor scope. Advertised in scopes_supported; no published description was found. Associated with the Flexmls-proprietary claims (FlexmlsMemberType, UserType, UserLevel, mls_system_access,\
  \ user_is_visible, user_is_enabled, user_is_active, user_is_billable, user_profile_visible).\", flows: [authorizationCode], sources: [.well-known/openid-configuration], documented: false}\n\nclaims_supported:\n  standard: [sub, iss, name, given_name, family_name, middle_name, preferred_username, website, address, phone_number, phone_number_verified, picture, email, email_verified, zoneinfo]\n  real_estate: [MemberNameSuffix, MemberMlsId, MemberNrdsId, MemberStateLicense, MemberAOR, MemberAORkey, MemberPrimaryAorId, MemberPrimaryAorKey, MemberType, MemberStatus, OfficeKey, Office, OfficeMlsId, FlexmlsMemberType, UserType, UserLevel, mls_system_access, user_is_visible, user_profile_visible, user_is_enabled, user_is_active, user_is_billable]\n\nnotes:\n  - OIDC keys require separate MLS approval beyond the standard developer registration.\n  - >-\n    Data-level authorization is role-based, not scope-based — see\n    authentication/spark-platform-authentication.yml and\n    https://sparkplatform.com/docs/supporting_documentation/roles.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spark-platform/refs/heads/main/scopes/spark-platform-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Real Estate
- United States
- MLS
- RESO
- Property Listings
- IDX
- PropTech
- Listing Data Infrastructure
- OData
token_urls:
- https://sparkplatform.com/openid/token
---
