---
authorization_urls:
- https://auth.komodohealth.com/authorize
description: 'OAuth 2.0 / OpenID Connect scopes advertised by Komodo Health''s authorization server. Read verbatim from the anonymous OIDC discovery document at auth.komodohealth.com (issuer https://auth.komodohealth.com/), which was discovered from the `WWW-Authenticate: Bearer realm="auth.komodohealth.com"` challenge returned by the Kong gateway at api.komodohealth.com.

  IMPORTANT READING NOTE: every scope below is a standard OpenID Connect identity scope or claim scope. Komodo does NOT advertise resource scopes for its own API (nothing like `read:cohorts` or `write:apps`), and publishes no scopes/permissions reference page. Platform authorization is expressed instead as Komodo account membership plus RBAC/FGA grantable roles on Komodo Apps and secrets. Treat this file as "what the authorization server advertises", not as a Komodo API permission model — that model is not published.'
docs: ''
flows:
- deviceCode
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Komodo Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Komodo Health publishes 14 OAuth 2.0 scopes via the deviceCode, clientCredentials, and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Komodo Health API on a user''s behalf.


  Tokens are issued from https://auth.komodohealth.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Komodo Health
provider_slug: komodo-health
schemes:
- flows:
  - device_authorization_endpoint: https://auth.komodohealth.com/oauth/device/code
    flow: deviceCode
    grant_type: urn:ietf:params:oauth:grant-type:device_code
    tokenUrl: https://auth.komodohealth.com/oauth/token
    used_by: '`komodo login` — interactive web login (RFC 8628)'
  - flow: clientCredentials
    grant_type: client_credentials
    tokenUrl: https://auth.komodohealth.com/oauth/token
    used_by: service principals — machine-to-machine
  - authorizationUrl: https://auth.komodohealth.com/authorize
    flow: authorizationCode
    grant_type: authorization_code
    pkce:
    - S256
    - plain
    tokenUrl: https://auth.komodohealth.com/oauth/token
  name: KomodoOAuth2
  source: https://auth.komodohealth.com/.well-known/openid-configuration
  type: oauth2
scope_count: 14
scope_names:
- openid
- profile
- email
- email_verified
- offline_access
- name
- given_name
- family_name
- nickname
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Request an ID token — OpenID Connect core.
  flows: []
  scope: openid
- description: Basic profile claims (name, given_name, family_name, nickname, picture).
  flows: []
  scope: profile
- description: Email address claim.
  flows: []
  scope: email
- description: Email verification status claim.
  flows: []
  scope: email_verified
- description: Issue a refresh token — used by the CLI to persist a session in ~/.komodo/credentials.
  flows: []
  scope: offline_access
- description: Full name claim.
  flows: []
  scope: name
- description: Given name claim.
  flows: []
  scope: given_name
- description: Family name claim.
  flows: []
  scope: family_name
- description: Nickname claim.
  flows: []
  scope: nickname
- description: Profile picture claim.
  flows: []
  scope: picture
- description: Account creation timestamp claim.
  flows: []
  scope: created_at
- description: Linked identity provider records claim.
  flows: []
  scope: identities
- description: Phone number claim.
  flows: []
  scope: phone
- description: Address claim.
  flows: []
  scope: address
slug: komodo-health-scopes
source_filename: komodo-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: https://auth.komodohealth.com/.well-known/openid-configuration\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by Komodo Health's authorization\n  server. Read verbatim from the anonymous OIDC discovery document at\n  auth.komodohealth.com (issuer https://auth.komodohealth.com/), which was\n  discovered from the `WWW-Authenticate: Bearer realm=\"auth.komodohealth.com\"`\n  challenge returned by the Kong gateway at api.komodohealth.com.\n\n  IMPORTANT READING NOTE: every scope below is a standard OpenID Connect\n  identity scope or claim scope. Komodo does NOT advertise resource scopes for\n  its own API (nothing like `read:cohorts` or `write:apps`), and publishes no\n  scopes/permissions reference page. Platform authorization is expressed instead\n  as Komodo account membership plus RBAC/FGA grantable roles on Komodo Apps and\n  secrets. Treat this file as \"what the authorization server advertises\", not as\n\
  \  a Komodo API permission model — that model is not published.\ndocs: null\ndocs_note: >-\n  No scopes or permissions reference page exists in the Marmot Development Kit\n  documentation (checked docs.komodohealth.com guides + reference, 2026-08-15).\n\nissuer: https://auth.komodohealth.com/\nprovider: Auth0-backed, operated on a Komodo-owned host\n\nschemes:\n  - name: KomodoOAuth2\n    type: oauth2\n    source: https://auth.komodohealth.com/.well-known/openid-configuration\n    flows:\n      - flow: deviceCode\n        grant_type: urn:ietf:params:oauth:grant-type:device_code\n        device_authorization_endpoint: https://auth.komodohealth.com/oauth/device/code\n        tokenUrl: https://auth.komodohealth.com/oauth/token\n        used_by: '`komodo login` — interactive web login (RFC 8628)'\n      - flow: clientCredentials\n        grant_type: client_credentials\n        tokenUrl: https://auth.komodohealth.com/oauth/token\n        used_by: service principals — machine-to-machine\n  \
  \    - flow: authorizationCode\n        grant_type: authorization_code\n        authorizationUrl: https://auth.komodohealth.com/authorize\n        tokenUrl: https://auth.komodohealth.com/oauth/token\n        pkce: [S256, plain]\n\nscopes:\n  - scope: openid\n    description: Request an ID token — OpenID Connect core.\n    kind: oidc-core\n  - scope: profile\n    description: Basic profile claims (name, given_name, family_name, nickname, picture).\n    kind: oidc-core\n  - scope: email\n    description: Email address claim.\n    kind: oidc-core\n  - scope: email_verified\n    description: Email verification status claim.\n    kind: oidc-claim\n  - scope: offline_access\n    description: Issue a refresh token — used by the CLI to persist a session in ~/.komodo/credentials.\n    kind: oidc-core\n  - scope: name\n    description: Full name claim.\n    kind: oidc-claim\n  - scope: given_name\n    description: Given name claim.\n    kind: oidc-claim\n  - scope: family_name\n    description:\
  \ Family name claim.\n    kind: oidc-claim\n  - scope: nickname\n    description: Nickname claim.\n    kind: oidc-claim\n  - scope: picture\n    description: Profile picture claim.\n    kind: oidc-claim\n  - scope: created_at\n    description: Account creation timestamp claim.\n    kind: oidc-claim\n  - scope: identities\n    description: Linked identity provider records claim.\n    kind: oidc-claim\n  - scope: phone\n    description: Phone number claim.\n    kind: oidc-claim\n  - scope: address\n    description: Address claim.\n    kind: oidc-claim\n\nresource_scopes:\n  published: false\n  note: >-\n    No Komodo-specific API resource scopes are advertised in discovery or\n    documented anywhere public. Access to the per-account Snowflake warehouse is\n    governed by Komodo account selection and the account's data subscriptions;\n    access to Komodo Apps and secrets is governed by RBAC/FGA grantable roles\n    (see the App Builder sharing tools in mcp/komodo-health-mcp.yml).\n\ncross_references:\n\
  \  authentication: authentication/komodo-health-authentication.yml\n  well_known: well-known/komodo-health-well-known.yml\n  raw_discovery: well-known/komodo-health-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/komodo-health/refs/heads/main/scopes/komodo-health-scopes.yml
summary_line: 14 scopes · deviceCode/clientCredentials/authorizationCode
tags:
- Company
- Healthcare
- Health Data
- Life Sciences
- Real-World Data
- Healthcare Analytics
- Artificial Intelligence
- Data
- Snowflake
- MCP
token_urls:
- https://auth.komodohealth.com/oauth/token
---
