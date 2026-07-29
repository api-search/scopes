---
authorization_urls:
- https://gateway.ieso.ca/oauth2/v1/authorize
description: ''
docs: https://www.ieso.ca/sector-participants/technical-interfaces
flows:
- authorizationCode
- implicit
- password
- deviceCode
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Ieso Scopes
name_suffix: OAuth Scopes
note: IESO publishes no OpenAPI and no API authorization scope reference. The only scope surface in the estate that can be read anonymously is the Okta identity provider at gateway.ieso.ca, whose OIDC discovery document advertises the stock OpenID Connect scope set for interactive participant login. These are identity scopes, not API permission scopes — none of IESO's documented APIs (Reports REST, MIM SOAP, Online IESO Appian) use OAuth 2.0 bearer tokens issued against these scopes; they use HTTP Basic, Appian API keys, and UserID/password with IP allow-listing respectively. Recorded here because it is the real, verified scope surface; nothing has been inferred or invented.
overview: 'IESO publishes 7 OAuth 2.0 scopes via the authorizationCode, implicit, password, deviceCode, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the IESO API on a user''s behalf.


  Tokens are issued from https://gateway.ieso.ca/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IESO
provider_slug: ieso
schemes:
- applies_to: interactive participant login (reports.ieso.ca, online.ieso.ca)
  flows:
  - authorizationUrl: https://gateway.ieso.ca/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://gateway.ieso.ca/oauth2/v1/token
  - authorizationUrl: https://gateway.ieso.ca/oauth2/v1/authorize
    flow: implicit
  - flow: password
    tokenUrl: https://gateway.ieso.ca/oauth2/v1/token
  - deviceAuthorizationUrl: https://gateway.ieso.ca/oauth2/v1/device/authorize
    flow: deviceCode
    tokenUrl: https://gateway.ieso.ca/oauth2/v1/token
  - flow: refreshToken
    tokenUrl: https://gateway.ieso.ca/oauth2/v1/token
  issuer: https://gateway.ieso.ca
  name: ieso-gateway
  source: well-known/ieso-openid-configuration.json
  type: openIdConnect
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- groups
scopes:
- description: Required OpenID Connect scope; requests an ID token for the authenticated participant user.
  flows: []
  scope: openid
- description: Standard OIDC profile claims (name, preferred_username, locale, updated_at).
  flows: []
  scope: profile
- description: Standard OIDC email and email_verified claims.
  flows: []
  scope: email
- description: Standard OIDC postal address claim.
  flows: []
  scope: address
- description: Standard OIDC phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Requests a refresh token so the session can be renewed without re-authentication.
  flows: []
  scope: offline_access
- description: Okta group membership claim. In an IESO deployment this is the closest thing to an authorization signal, since participant entitlements are administered as group/role membership by the organization's Rights Administrator rather than as API scopes.
  flows: []
  scope: groups
slug: ieso-scopes
source_filename: ieso-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://gateway.ieso.ca/.well-known/openid-configuration\ndocs: https://www.ieso.ca/sector-participants/technical-interfaces\nnote: >-\n  IESO publishes no OpenAPI and no API authorization scope reference. The only scope surface in the\n  estate that can be read anonymously is the Okta identity provider at gateway.ieso.ca, whose OIDC\n  discovery document advertises the stock OpenID Connect scope set for interactive participant login.\n  These are identity scopes, not API permission scopes — none of IESO's documented APIs (Reports REST,\n  MIM SOAP, Online IESO Appian) use OAuth 2.0 bearer tokens issued against these scopes; they use HTTP\n  Basic, Appian API keys, and UserID/password with IP allow-listing respectively. Recorded here\n  because it is the real, verified scope surface; nothing has been inferred or invented.\nschemes:\n- name: ieso-gateway\n  type: openIdConnect\n  issuer: https://gateway.ieso.ca\n  source: well-known/ieso-openid-configuration.json\n\
  \  applies_to: interactive participant login (reports.ieso.ca, online.ieso.ca)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://gateway.ieso.ca/oauth2/v1/authorize\n    tokenUrl: https://gateway.ieso.ca/oauth2/v1/token\n  - flow: implicit\n    authorizationUrl: https://gateway.ieso.ca/oauth2/v1/authorize\n  - flow: password\n    tokenUrl: https://gateway.ieso.ca/oauth2/v1/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://gateway.ieso.ca/oauth2/v1/device/authorize\n    tokenUrl: https://gateway.ieso.ca/oauth2/v1/token\n  - flow: refreshToken\n    tokenUrl: https://gateway.ieso.ca/oauth2/v1/token\nscopes:\n- scope: openid\n  description: Required OpenID Connect scope; requests an ID token for the authenticated participant user.\n  kind: identity\n  sources: [well-known/ieso-openid-configuration.json]\n- scope: profile\n  description: Standard OIDC profile claims (name, preferred_username, locale, updated_at).\n  kind: identity\n  sources: [well-known/ieso-openid-configuration.json]\n\
  - scope: email\n  description: Standard OIDC email and email_verified claims.\n  kind: identity\n  sources: [well-known/ieso-openid-configuration.json]\n- scope: address\n  description: Standard OIDC postal address claim.\n  kind: identity\n  sources: [well-known/ieso-openid-configuration.json]\n- scope: phone\n  description: Standard OIDC phone_number and phone_number_verified claims.\n  kind: identity\n  sources: [well-known/ieso-openid-configuration.json]\n- scope: offline_access\n  description: Requests a refresh token so the session can be renewed without re-authentication.\n  kind: session\n  sources: [well-known/ieso-openid-configuration.json]\n- scope: groups\n  description: >-\n    Okta group membership claim. In an IESO deployment this is the closest thing to an authorization\n    signal, since participant entitlements are administered as group/role membership by the\n    organization's Rights Administrator rather than as API scopes.\n  kind: authorization\n  sources: [well-known/ieso-openid-configuration.json]\n\
  api_permission_scopes: none_published\ngaps:\n- >-\n  No per-API scope catalogue exists. Entitlements to the Reports API, MIM web services and the Online\n  IESO APIs are granted as machine-account permissions by IESO staff and the participant's Rights\n  Administrator, not as OAuth scopes a client can request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ieso/refs/heads/main/scopes/ieso-scopes.yml
summary_line: 7 scopes · authorizationCode/implicit/password/deviceCode/refreshToken
tags:
- Energy
- Canada
- Electricity
- Energy Markets
- Grid
- System Operator
- Market Data
- Open Data
- Ontario
- Demand Response
- Renewables
token_urls:
- https://gateway.ieso.ca/oauth2/v1/token
---
