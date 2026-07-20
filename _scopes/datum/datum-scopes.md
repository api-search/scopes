---
authorization_urls: []
description: ''
docs: https://www.datum.net/docs/datumctl/auth/logging-in.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Datum Scopes
name_suffix: OAuth Scopes
note: These are the standard OIDC scopes advertised by the Datum identity provider (auth.datum.net). Resource-level authorization on the Datum Cloud control-plane API is enforced via RBAC on the bearer token rather than fine-grained OAuth scopes.
overview: 'Datum publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Datum API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Datum
provider_slug: datum
schemes:
- authorizationUrl: https://auth.datum.net/oauth/v2/authorize
  name: OAuth2
  source: well-known/datum-openid-configuration.json
  tokenUrl: https://auth.datum.net/oauth/v2/token
scope_count: 6
scope_names:
- openid
- profile
- email
- phone
- address
- offline_access
scopes:
- description: OIDC authentication — issue an ID token.
  flows: []
  scope: openid
- description: Access to the user's basic profile claims (name, preferred_username, locale).
  flows: []
  scope: profile
- description: Access to the user's email address and verification status.
  flows: []
  scope: email
- description: Access to the user's phone number and verification status.
  flows: []
  scope: phone
- description: Access to the user's address claim.
  flows: []
  scope: address
- description: Issue a refresh token for long-lived, offline access.
  flows: []
  scope: offline_access
slug: datum-scopes
source_filename: datum-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.datum.net/.well-known/openid-configuration\ndocs: https://www.datum.net/docs/datumctl/auth/logging-in.md\nschemes:\n- name: OAuth2\n  source: well-known/datum-openid-configuration.json\n  authorizationUrl: https://auth.datum.net/oauth/v2/authorize\n  tokenUrl: https://auth.datum.net/oauth/v2/token\nscopes:\n- scope: openid\n  description: OIDC authentication — issue an ID token.\n- scope: profile\n  description: Access to the user's basic profile claims (name, preferred_username, locale).\n- scope: email\n  description: Access to the user's email address and verification status.\n- scope: phone\n  description: Access to the user's phone number and verification status.\n- scope: address\n  description: Access to the user's address claim.\n- scope: offline_access\n  description: Issue a refresh token for long-lived, offline access.\nnote: >-\n  These are the standard OIDC scopes advertised by the Datum identity provider\n\
  \  (auth.datum.net). Resource-level authorization on the Datum Cloud control-plane\n  API is enforced via RBAC on the bearer token rather than fine-grained OAuth\n  scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datum/refs/heads/main/scopes/datum-scopes.yml
summary_line: 6 scopes
tags:
- Company
- Data
- Cloud
- Networking
- Edge
- AI
- DNS
- Infrastructure
- CDN
- Developer Tools
token_urls: []
---
