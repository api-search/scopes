---
authorization_urls:
- https://aescape-8ocoec.zitadel.cloud/oauth/v2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
- implicit
kind: oauth-scopes
layout: scope
method: probed
name: Aescape Scopes
name_suffix: OAuth Scopes
note: Scopes are read verbatim from scopes_supported in the OIDC discovery document of Aescape's production Zitadel tenant. Aescape publishes no OpenAPI and no public scopes/permissions reference page, so this is the complete publicly advertised scope surface. These are the standard OpenID Connect scopes; no Aescape-specific application scopes (for example massage session, booking or device scopes) are publicly advertised.
overview: 'Aescape publishes 6 OAuth 2.0 scopes via the authorizationCode, clientCredentials, deviceCode, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aescape API on a user''s behalf.


  Tokens are issued from https://aescape-8ocoec.zitadel.cloud/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aescape
provider_slug: aescape
schemes:
- flows:
  - authorizationUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/token
  - flow: clientCredentials
    tokenUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/token
  - deviceAuthorizationUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/device_authorization
    flow: deviceCode
    tokenUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/token
  - authorizationUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/authorize
    flow: implicit
  issuer: https://aescape-8ocoec.zitadel.cloud
  name: AescapeOIDC
  source: well-known/aescape-openid-configuration.json
scope_count: 6
scope_names:
- openid
- profile
- email
- phone
- address
- offline_access
scopes:
- description: Required OpenID Connect scope; requests an ID token identifying the end user.
  flows: []
  scope: openid
- description: Access to the end user's default profile claims — name, family_name, given_name, preferred_username, locale.
  flows: []
  scope: profile
- description: Access to the email and email_verified claims.
  flows: []
  scope: email
- description: Access to the phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Access to the end user's address claim.
  flows: []
  scope: address
- description: Requests a refresh token so the client can obtain new access tokens without the end user present.
  flows: []
  scope: offline_access
slug: aescape-scopes
source_filename: aescape-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://aescape-8ocoec.zitadel.cloud/.well-known/openid-configuration\nnote: >-\n  Scopes are read verbatim from scopes_supported in the OIDC discovery document of\n  Aescape's production Zitadel tenant. Aescape publishes no OpenAPI and no public\n  scopes/permissions reference page, so this is the complete publicly advertised\n  scope surface. These are the standard OpenID Connect scopes; no Aescape-specific\n  application scopes (for example massage session, booking or device scopes) are\n  publicly advertised.\ndocs: null\nschemes:\n- name: AescapeOIDC\n  source: well-known/aescape-openid-configuration.json\n  issuer: https://aescape-8ocoec.zitadel.cloud\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/authorize\n    tokenUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/token\n\
  \  - flow: deviceCode\n    deviceAuthorizationUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/device_authorization\n    tokenUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/token\n  - flow: implicit\n    authorizationUrl: https://aescape-8ocoec.zitadel.cloud/oauth/v2/authorize\nscopes:\n- scope: openid\n  description: Required OpenID Connect scope; requests an ID token identifying the\n    end user.\n  standard: OpenID Connect Core 1.0\n  sources: [well-known/aescape-openid-configuration.json]\n- scope: profile\n  description: Access to the end user's default profile claims — name, family_name,\n    given_name, preferred_username, locale.\n  standard: OpenID Connect Core 1.0\n  sources: [well-known/aescape-openid-configuration.json]\n- scope: email\n  description: Access to the email and email_verified claims.\n  standard: OpenID Connect Core 1.0\n  sources: [well-known/aescape-openid-configuration.json]\n- scope: phone\n  description: Access to the phone_number and phone_number_verified\
  \ claims.\n  standard: OpenID Connect Core 1.0\n  sources: [well-known/aescape-openid-configuration.json]\n- scope: address\n  description: Access to the end user's address claim.\n  standard: OpenID Connect Core 1.0\n  sources: [well-known/aescape-openid-configuration.json]\n- scope: offline_access\n  description: Requests a refresh token so the client can obtain new access tokens\n    without the end user present.\n  standard: OpenID Connect Core 1.0\n  sources: [well-known/aescape-openid-configuration.json]\ncoverage:\n  scopes_total: 6\n  standard_oidc: 6\n  application_specific: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aescape/refs/heads/main/scopes/aescape-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials/deviceCode/implicit
tags:
- Company
- Robotics
- Health and Wellness
- Fitness
- Massage
- Artificial Intelligence
- Consumer Hardware
- Hospitality
- Recovery
- Identity
token_urls:
- https://aescape-8ocoec.zitadel.cloud/oauth/v2/token
---
