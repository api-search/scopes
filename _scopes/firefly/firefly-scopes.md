---
authorization_urls: []
description: 'The complete scopes_supported list published by Firefly''s Auth0 custom-domain tenant, read verbatim from the live OpenID Connect discovery document (HTTP 200, 2026-08-12) and saved at well-known/firefly-openid-configuration.json. IMPORTANT READING NOTE: every scope below is a standard OpenID Connect / Auth0 profile claim scope. Firefly publishes NO product or resource scopes (nothing shaped like campaign:read, inventory:write, reporting:export), and no scope reference page exists anywhere on fireflyon.com. Authorization for the advertiser dashboard gateway (audience https://gw.fireflyon.com) is therefore not expressed through discoverable scopes; whatever permission model it uses is not publicly readable. This artifact records the identity scopes that ARE published, and records the absence of API scopes as the finding.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Firefly Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Firefly publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Firefly API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Firefly
provider_slug: firefly
schemes:
- grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://auth.fireflyon.com/
  name: firefly-dashboard-oidc
  openIdConnectUrl: https://auth.fireflyon.com/.well-known/openid-configuration
  pkce: S256
  type: openIdConnect
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- email
- address
- phone
- name
- given_name
- family_name
- nickname
- picture
- email_verified
- created_at
- identities
scopes:
- description: Standard OIDC scope — requests an ID token for the authenticated subject.
  flows: []
  scope: openid
- description: Standard OIDC scope — the default profile claim set (name, family_name, given_name, nickname, picture, updated_at).
  flows: []
  scope: profile
- description: Standard OIDC scope — requests a refresh token for long-lived access.
  flows: []
  scope: offline_access
- description: Standard OIDC scope — releases the email claim.
  flows: []
  scope: email
- description: Standard OIDC scope — releases the address claim.
  flows: []
  scope: address
- description: Standard OIDC scope — releases the phone_number claim.
  flows: []
  scope: phone
- description: Auth0 granular profile scope — releases the name claim alone.
  flows: []
  scope: name
- description: Auth0 granular profile scope — releases the given_name claim alone.
  flows: []
  scope: given_name
- description: Auth0 granular profile scope — releases the family_name claim alone.
  flows: []
  scope: family_name
- description: Auth0 granular profile scope — releases the nickname claim alone.
  flows: []
  scope: nickname
- description: Auth0 granular profile scope — releases the picture claim alone.
  flows: []
  scope: picture
- description: Auth0 granular profile scope — releases the email_verified claim alone.
  flows: []
  scope: email_verified
- description: Auth0 granular profile scope — releases the account created_at claim.
  flows: []
  scope: created_at
- description: Auth0 granular profile scope — releases the linked-identities claim.
  flows: []
  scope: identities
slug: firefly-scopes
source_filename: firefly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://auth.fireflyon.com/.well-known/openid-configuration\ndocs: null\ndescription: >-\n  The complete scopes_supported list published by Firefly's Auth0 custom-domain tenant,\n  read verbatim from the live OpenID Connect discovery document (HTTP 200, 2026-08-12)\n  and saved at well-known/firefly-openid-configuration.json. IMPORTANT READING NOTE:\n  every scope below is a standard OpenID Connect / Auth0 profile claim scope. Firefly\n  publishes NO product or resource scopes (nothing shaped like campaign:read,\n  inventory:write, reporting:export), and no scope reference page exists anywhere on\n  fireflyon.com. Authorization for the advertiser dashboard gateway\n  (audience https://gw.fireflyon.com) is therefore not expressed through discoverable\n  scopes; whatever permission model it uses is not publicly readable. This artifact\n  records the identity scopes that ARE published, and records the absence of API scopes\n  as\
  \ the finding.\nschemes:\n- name: firefly-dashboard-oidc\n  type: openIdConnect\n  issuer: https://auth.fireflyon.com/\n  openIdConnectUrl: https://auth.fireflyon.com/.well-known/openid-configuration\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  pkce: S256\nscope_count: 14\nscopes:\n- scope: openid\n  description: Standard OIDC scope — requests an ID token for the authenticated subject.\n  standard: openid-connect-core\n  schemes: [firefly-dashboard-oidc]\n- scope: profile\n  description: Standard OIDC scope — the default profile claim set (name, family_name, given_name, nickname, picture, updated_at).\n  standard: openid-connect-core\n  schemes: [firefly-dashboard-oidc]\n- scope: offline_access\n  description: Standard OIDC scope — requests a refresh token for long-lived access.\n  standard: openid-connect-core\n  schemes: [firefly-dashboard-oidc]\n- scope: email\n  description: Standard OIDC scope\
  \ — releases the email claim.\n  standard: openid-connect-core\n  schemes: [firefly-dashboard-oidc]\n- scope: address\n  description: Standard OIDC scope — releases the address claim.\n  standard: openid-connect-core\n  schemes: [firefly-dashboard-oidc]\n- scope: phone\n  description: Standard OIDC scope — releases the phone_number claim.\n  standard: openid-connect-core\n  schemes: [firefly-dashboard-oidc]\n- scope: name\n  description: Auth0 granular profile scope — releases the name claim alone.\n  standard: auth0-profile-scope\n  schemes: [firefly-dashboard-oidc]\n- scope: given_name\n  description: Auth0 granular profile scope — releases the given_name claim alone.\n  standard: auth0-profile-scope\n  schemes: [firefly-dashboard-oidc]\n- scope: family_name\n  description: Auth0 granular profile scope — releases the family_name claim alone.\n  standard: auth0-profile-scope\n  schemes: [firefly-dashboard-oidc]\n- scope: nickname\n  description: Auth0 granular profile scope — releases\
  \ the nickname claim alone.\n  standard: auth0-profile-scope\n  schemes: [firefly-dashboard-oidc]\n- scope: picture\n  description: Auth0 granular profile scope — releases the picture claim alone.\n  standard: auth0-profile-scope\n  schemes: [firefly-dashboard-oidc]\n- scope: email_verified\n  description: Auth0 granular profile scope — releases the email_verified claim alone.\n  standard: auth0-profile-scope\n  schemes: [firefly-dashboard-oidc]\n- scope: created_at\n  description: Auth0 granular profile scope — releases the account created_at claim.\n  standard: auth0-profile-scope\n  schemes: [firefly-dashboard-oidc]\n- scope: identities\n  description: Auth0 granular profile scope — releases the linked-identities claim.\n  standard: auth0-profile-scope\n  schemes: [firefly-dashboard-oidc]\nfindings:\n- id: no-product-scopes-published\n  severity: informational\n  detail: >-\n    Zero of the 14 published scopes describe a Firefly resource. An integrator or agent\n    cannot determine,\
  \ from anything Firefly publishes, what an access token for\n    https://gw.fireflyon.com is permitted to do.\n  evidence:\n  - url: https://auth.fireflyon.com/.well-known/openid-configuration\n    status: 200\n  - url: https://app-gw.api.fireflyon.com/.well-known/oauth-protected-resource\n    status: 404\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - url: https://auth.fireflyon.com/.well-known/openid-configuration\n    status: 200\n  - url: https://auth.fireflyon.com/.well-known/oauth-authorization-server\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firefly/refs/heads/main/scopes/firefly-scopes.yml
summary_line: 14 scopes
tags:
- Company
- Advertising
- Digital Out Of Home
- DOOH
- Mobility
- Advertising Technology
- AdTech
- Marketing
- Measurements
- Programmatic Advertising
token_urls: []
---
