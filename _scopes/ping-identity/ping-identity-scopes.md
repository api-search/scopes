---
api_specs:
- filename: ping-identity-openapi.yaml
  format: yaml
  label: PingOne Platform API
  slug: pingone-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-openapi.yaml
authorization_urls:
- /as/authorize
description: ''
docs: https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles.html
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ping Identity Scopes
name_suffix: OAuth Scopes
note: PingOne documents OIDC scopes and PingOne API self-management scopes (user-only); administrative access to the PingOne platform APIs is granted through roles assigned to worker applications rather than OAuth scopes.
overview: 'Ping Identity publishes 26 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ping Identity API on a user''s behalf.


  Tokens are issued from /as/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ping Identity
provider_slug: ping-identity
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /as/token
  - authorizationUrl: /as/authorize
    flow: authorizationCode
    tokenUrl: /as/token
  name: oauth2
  source: openapi/ping-identity-openapi.yaml
scope_count: 26
scope_names:
- openid
- profile
- email
- address
- phone
- p1:read:user
- p1:update:user
- p1:update:userMfaEnabled
- p1:create:device
- p1:read:device
- p1:update:device
- p1:delete:device
- p1:read:userPassword
- p1:reset:userPassword
- p1:validate:userPassword
- p1:read:userLinkedAccounts
- p1:delete:userLinkedAccounts
- p1:create:pairingKey
- p1:read:pairingKey
- p1:delete:pairingKey
- p1:read:sessions
- p1:delete:sessions
- p1:read:userConsent
- p1:verify:user
- p1:read:oauthConsent
- p1:update:oauthConsent
scopes:
- description: Required scope that tells the authorization server the incoming request is an OpenID Connect request.
  flows: []
  scope: openid
- description: Grants access to end-user profile claims including name, family name, given name, middle name, preferred username, nickname, picture, timezone, locale, profile, website, gender, birthdate, and updated timestamp.
  flows: []
  scope: profile
- description: Grants access to the email and email_verified claims.
  flows: []
  scope: email
- description: Grants access to address claims including street address, locality, region, postal code, country, and formatted address.
  flows: []
  scope: address
- description: Grants access to the phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Users can retrieve their own user identity and all attributes.
  flows: []
  scope: p1:read:user
- description: Users can modify the attributes of their own user identity.
  flows: []
  scope: p1:update:user
- description: Users can enable and disable multi-factor authentication for their own user identity.
  flows: []
  scope: p1:update:userMfaEnabled
- description: Users can create multi-factor authentication devices for their own user identity.
  flows: []
  scope: p1:create:device
- description: Users can retrieve multi-factor authentication devices for their own user identity.
  flows: []
  scope: p1:read:device
- description: Users can update multi-factor authentication devices for their own user identity.
  flows: []
  scope: p1:update:device
- description: Users can delete multi-factor authentication devices for their own user identity.
  flows: []
  scope: p1:delete:device
- description: Users can read the password state for their own user identity.
  flows: []
  scope: p1:read:userPassword
- description: Users can reset the password for their own user identity.
  flows: []
  scope: p1:reset:userPassword
- description: Users can validate the password for their own user identity.
  flows: []
  scope: p1:validate:userPassword
- description: Users can read linked accounts for their own user identity.
  flows: []
  scope: p1:read:userLinkedAccounts
- description: Users can delete linked accounts for their own user identity.
  flows: []
  scope: p1:delete:userLinkedAccounts
- description: Users can create a pairing key for their own user identity.
  flows: []
  scope: p1:create:pairingKey
- description: Users can read a pairing key for their own user identity.
  flows: []
  scope: p1:read:pairingKey
- description: Users can delete a pairing key for their own user identity.
  flows: []
  scope: p1:delete:pairingKey
- description: Users can read sessions for their own user identity.
  flows: []
  scope: p1:read:sessions
- description: Users can delete sessions for their own user identity.
  flows: []
  scope: p1:delete:sessions
- description: Users can read consents for their own user identity.
  flows: []
  scope: p1:read:userConsent
- description: Users can verify their own user identity.
  flows: []
  scope: p1:verify:user
- description: Users can read oauth scope consents for their own user identity.
  flows: []
  scope: p1:read:oauthConsent
- description: Users can update oauth scope consents for their own user identity.
  flows: []
  scope: p1:update:oauthConsent
slug: ping-identity-scopes
source_filename: ping-identity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/ping-identity-openapi.yaml\ndocs: https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles.html\nnote: PingOne documents OIDC scopes and PingOne API self-management scopes (user-only);\n  administrative access to the PingOne platform APIs is granted through roles assigned\n  to worker applications rather than OAuth scopes.\nschemes:\n- name: oauth2\n  source: openapi/ping-identity-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /as/token\n  - flow: authorizationCode\n    authorizationUrl: /as/authorize\n    tokenUrl: /as/token\nscopes:\n- scope: openid\n  description: Required scope that tells the authorization server the incoming request\n    is an OpenID Connect request.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/openid-connect-oidc-scopes.html\n\
  - scope: profile\n  description: Grants access to end-user profile claims including name, family name,\n    given name, middle name, preferred username, nickname, picture, timezone, locale,\n    profile, website, gender, birthdate, and updated timestamp.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/openid-connect-oidc-scopes.html\n- scope: email\n  description: Grants access to the email and email_verified claims.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/openid-connect-oidc-scopes.html\n- scope: address\n  description: Grants access to address claims including street address, locality,\n    region, postal code, country, and formatted address.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/openid-connect-oidc-scopes.html\n\
  - scope: phone\n  description: Grants access to the phone_number and phone_number_verified claims.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/openid-connect-oidc-scopes.html\n- scope: p1:read:user\n  description: Users can retrieve their own user identity and all attributes.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:update:user\n  description: Users can modify the attributes of their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:update:userMfaEnabled\n  description: Users can enable and disable multi-factor authentication for their\n    own user\
  \ identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:create:device\n  description: Users can create multi-factor authentication devices for their own\n    user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:read:device\n  description: Users can retrieve multi-factor authentication devices for their own\n    user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:update:device\n  description: Users can update multi-factor authentication devices for their own\n    user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n\
  - scope: p1:delete:device\n  description: Users can delete multi-factor authentication devices for their own\n    user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:read:userPassword\n  description: Users can read the password state for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:reset:userPassword\n  description: Users can reset the password for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:validate:userPassword\n  description: Users can validate the password for\
  \ their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:read:userLinkedAccounts\n  description: Users can read linked accounts for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:delete:userLinkedAccounts\n  description: Users can delete linked accounts for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:create:pairingKey\n  description: Users can create a pairing key for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n\
  - scope: p1:read:pairingKey\n  description: Users can read a pairing key for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:delete:pairingKey\n  description: Users can delete a pairing key for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:read:sessions\n  description: Users can read sessions for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:delete:sessions\n  description: Users can delete sessions for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n\
  - scope: p1:read:userConsent\n  description: Users can read consents for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:verify:user\n  description: Users can verify their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:read:oauthConsent\n  description: Users can read oauth scope consents for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n- scope: p1:update:oauthConsent\n  description: Users can update oauth scope consents for their own user identity.\n  sources:\n  - https://developer.pingidentity.com/pingone-api/foundations/pingone-roles-scopes-and-permissions/access-services-through-scopes-and-roles/pingone-self-management-scopes.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/scopes/ping-identity-scopes.yml
summary_line: 26 scopes · clientCredentials/authorizationCode
tags:
- Identity
- Authentication
- Authorization
- SSO
- MFA
token_urls:
- /as/token
---
