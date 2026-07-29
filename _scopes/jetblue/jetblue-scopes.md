---
authorization_urls:
- https://accounts.jetblue.com/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Jetblue Scopes
name_suffix: OAuth Scopes
note: Scopes are read verbatim from the anonymous discovery documents of accounts.jetblue.com (Okta). The OIDC discovery document advertises only the standard OpenID Connect scope set; the RFC 8414 authorization-server document additionally advertises the Okta org management scope namespace (okta.*), which is Okta platform default surface for the org's own administration API, not a JetBlue product scope. JetBlue publishes no scope or permission reference of its own, and no JetBlue business scopes (booking, flight status, TrueBlue, NDC) appear anywhere in the discovery documents.
overview: 'JetBlue publishes 7 OAuth 2.0 scopes via the authorizationCode, implicit, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the JetBlue API on a user''s behalf.


  Tokens are issued from https://accounts.jetblue.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: JetBlue
provider_slug: jetblue
schemes:
- flows:
  - authorizationUrl: https://accounts.jetblue.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://accounts.jetblue.com/oauth2/v1/token
  - authorizationUrl: https://accounts.jetblue.com/oauth2/v1/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://accounts.jetblue.com/oauth2/v1/device/authorize
    flow: deviceCode
    tokenUrl: https://accounts.jetblue.com/oauth2/v1/token
  issuer: https://accounts.jetblue.com
  name: JetBlueAccountsOIDC
  source: well-known/jetblue-openid-configuration.json
  vendor: Okta
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
- description: Request an OpenID Connect ID token for the signed-in JetBlue account.
  flows: []
  scope: openid
- description: Basic profile claims (name, preferred_username, locale, updated_at).
  flows: []
  scope: profile
- description: Email address and email_verified claim.
  flows: []
  scope: email
- description: Postal address claim.
  flows: []
  scope: address
- description: Phone number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Issue a refresh token so the client can renew access without re-authentication.
  flows: []
  scope: offline_access
- description: Group memberships claim for the account.
  flows: []
  scope: groups
slug: jetblue-scopes
source_filename: jetblue-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: https://accounts.jetblue.com/.well-known/openid-configuration\nalso_source: https://accounts.jetblue.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Scopes are read verbatim from the anonymous discovery documents of\n  accounts.jetblue.com (Okta). The OIDC discovery document advertises only the\n  standard OpenID Connect scope set; the RFC 8414 authorization-server\n  document additionally advertises the Okta org management scope namespace\n  (okta.*), which is Okta platform default surface for the org's own\n  administration API, not a JetBlue product scope. JetBlue publishes no scope\n  or permission reference of its own, and no JetBlue business scopes (booking,\n  flight status, TrueBlue, NDC) appear anywhere in the discovery documents.\nschemes:\n- name: JetBlueAccountsOIDC\n  issuer: https://accounts.jetblue.com\n  vendor: Okta\n  source: well-known/jetblue-openid-configuration.json\n  flows:\n  - flow:\
  \ authorizationCode\n    authorizationUrl: https://accounts.jetblue.com/oauth2/v1/authorize\n    tokenUrl: https://accounts.jetblue.com/oauth2/v1/token\n  - flow: implicit\n    authorizationUrl: https://accounts.jetblue.com/oauth2/v1/authorize\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://accounts.jetblue.com/oauth2/v1/device/authorize\n    tokenUrl: https://accounts.jetblue.com/oauth2/v1/token\nscopes:\n- scope: openid\n  description: Request an OpenID Connect ID token for the signed-in JetBlue account.\n  category: oidc-standard\n  sources:\n  - well-known/jetblue-openid-configuration.json\n- scope: profile\n  description: Basic profile claims (name, preferred_username, locale, updated_at).\n  category: oidc-standard\n  sources:\n  - well-known/jetblue-openid-configuration.json\n- scope: email\n  description: Email address and email_verified claim.\n  category: oidc-standard\n  sources:\n  - well-known/jetblue-openid-configuration.json\n- scope: address\n  description: Postal\
  \ address claim.\n  category: oidc-standard\n  sources:\n  - well-known/jetblue-openid-configuration.json\n- scope: phone\n  description: Phone number and phone_number_verified claims.\n  category: oidc-standard\n  sources:\n  - well-known/jetblue-openid-configuration.json\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without re-authentication.\n  category: oidc-standard\n  sources:\n  - well-known/jetblue-openid-configuration.json\n- scope: groups\n  description: Group memberships claim for the account.\n  category: okta-standard\n  sources:\n  - well-known/jetblue-openid-configuration.json\nokta_management_scopes:\n  note: >-\n    Advertised by the RFC 8414 authorization-server metadata as the Okta org\n    management API scope namespace. Recorded for completeness — these govern\n    Okta tenant administration, not JetBlue travel functionality, and are not\n    grantable to outside parties.\n  source: well-known/jetblue-oauth-authorization-server.json\n\
  \  namespaces:\n  - okta.users.*\n  - okta.groups.*\n  - okta.apps.*\n  - okta.clients.*\n  - okta.policies.*\n  - okta.idps.*\n  - okta.factors.*\n  - okta.sessions.*\n  - okta.logs.read\n  - okta.events.read\n  - okta.roles.*\n  - okta.orgs.*\n  - okta.domains.*\n  - okta.brands.*\n  - okta.schemas.*\n  - okta.templates.*\n  - okta.trustedOrigins.*\n  - okta.networkZones.*\n  - okta.behaviors.*\n  - okta.threatInsights.*\n  - okta.riskProviders.*\n  - okta.inlineHooks.*\n  - okta.eventHooks.*\n  - okta.linkedObjects.*\n  - okta.profileMappings.*\n  - okta.userTypes.*\n  - okta.appGrants.*\n  - okta.agentPools.*\n  - okta.reports.*\n  - okta.features.*\n  - okta.certificateAuthorities.*\n  - okta.principalRateLimits.*\n  - okta.rateLimits.*\n  - okta.directories.*\n  - okta.apiTokens.*\n  - okta.accessRequests.tasks.*\n  - okta.governance.assignmentCandidates.read\n  - okta.personal.adminSettings.*\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetblue/refs/heads/main/scopes/jetblue-scopes.yml
summary_line: 7 scopes · authorizationCode/implicit/deviceCode
tags:
- Travel
- United States
- Aviation
- Airline
- Distribution
- NDC
- GDS
- Booking
- Loyalty
token_urls:
- https://accounts.jetblue.com/oauth2/v1/token
---
