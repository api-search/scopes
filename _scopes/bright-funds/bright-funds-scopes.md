---
authorization_urls:
- https://www.brightfunds.org/oauth/authorize
description: ''
docs: https://www.brightfunds.org/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Bright Funds Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bright Funds publishes 7 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bright Funds API on a user''s behalf.


  Tokens are issued from https://www.brightfunds.org/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bright Funds
provider_slug: bright-funds
schemes:
- flows:
  - authorizationUrl: https://www.brightfunds.org/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.brightfunds.org/oauth/token
  - flow: clientCredentials
    tokenUrl: https://www.brightfunds.org/oauth/token
  name: OAuth2
  source: well-known/bright-funds-openid-configuration.json
scope_count: 7
scope_names:
- openid
- profile
- email
- name
- offline_access
- write
- update
scopes:
- description: OpenID Connect authentication; issue an id_token for the subject.
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's profile claims (name, given_name, family_name, zoneinfo, updated_at).
  flows:
  - authorizationCode
  scope: profile
- description: Access the user's email claim.
  flows:
  - authorizationCode
  scope: email
- description: Access the user's name claim.
  flows:
  - authorizationCode
  scope: name
- description: Issue a refresh_token for long-lived access without the user present.
  flows:
  - authorizationCode
  scope: offline_access
- description: Write access to the Bright Funds platform resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: write
- description: Update access to the Bright Funds platform resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: update
slug: bright-funds-scopes
source_filename: bright-funds-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.brightfunds.org/.well-known/openid-configuration\ndocs: https://www.brightfunds.org/.well-known/openid-configuration\nschemes:\n- name: OAuth2\n  source: well-known/bright-funds-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.brightfunds.org/oauth/authorize\n    tokenUrl: https://www.brightfunds.org/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://www.brightfunds.org/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an id_token for the subject.\n  flows: [authorizationCode]\n  sources: [well-known/bright-funds-openid-configuration.json]\n- scope: profile\n  description: Access the user's profile claims (name, given_name, family_name, zoneinfo, updated_at).\n  flows: [authorizationCode]\n  sources: [well-known/bright-funds-openid-configuration.json]\n- scope: email\n  description: Access the user's email claim.\n\
  \  flows: [authorizationCode]\n  sources: [well-known/bright-funds-openid-configuration.json]\n- scope: name\n  description: Access the user's name claim.\n  flows: [authorizationCode]\n  sources: [well-known/bright-funds-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh_token for long-lived access without the user present.\n  flows: [authorizationCode]\n  sources: [well-known/bright-funds-openid-configuration.json]\n- scope: write\n  description: Write access to the Bright Funds platform resources.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/bright-funds-openid-configuration.json]\n- scope: update\n  description: Update access to the Bright Funds platform resources.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/bright-funds-openid-configuration.json]\nnotes: >-\n  Scopes are taken verbatim from the published scopes_supported list in the OIDC discovery\n  document. Flow-to-scope mapping is inferred\
  \ (the discovery doc does not per-scope-map flows);\n  standard OIDC scopes bind to the authorization_code flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-funds/refs/heads/main/scopes/bright-funds-scopes.yml
summary_line: 7 scopes · authorizationCode/clientCredentials
tags:
- Company
- Workplace Giving
- Corporate Social Responsibility
- Employee Engagement
- Nonprofits
- Grants Management
- Donations
- Volunteering
- OAuth
- OpenID Connect
token_urls:
- https://www.brightfunds.org/oauth/token
---
