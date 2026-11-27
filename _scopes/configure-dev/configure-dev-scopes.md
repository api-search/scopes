---
api_specs:
- filename: configure-dev-auth-api-openapi.yml
  format: yaml
  label: Configure Auth API
  slug: configure-dev-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-auth-api-openapi.yml
- filename: configure-dev-connectors-api-openapi.yml
  format: yaml
  label: Configure Connectors API
  slug: configure-dev-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-connectors-api-openapi.yml
- filename: configure-dev-files-api-openapi.yml
  format: yaml
  label: Configure Files API
  slug: configure-dev-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-files-api-openapi.yml
- filename: configure-dev-import-api-openapi.yml
  format: yaml
  label: Configure Import API
  slug: configure-dev-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-import-api-openapi.yml
- filename: configure-dev-profile-api-openapi.yml
  format: yaml
  label: Configure Profile API
  slug: configure-dev-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-profile-api-openapi.yml
- filename: configure-dev-web-api-openapi.yml
  format: yaml
  label: Configure Web API
  slug: configure-dev-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-web-api-openapi.yml
- filename: configure-dev-webhooks-api-openapi.yml
  format: yaml
  label: Configure Webhooks API
  slug: configure-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configure-dev/openapi/configure-dev-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.configure.dev/oidc.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Configure Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares no oauth2 scheme; scopes come from the OIDC and Sign in with Configure docs. If the authorization request omits scope, the scopes registered for the client apply (a client made with POST /v1/sso/client registers openid, email and profile).
overview: 'Configure publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Configure API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Configure
provider_slug: configure-dev
schemes: []
scope_count: 7
scope_names:
- openid
- email
- profile
- profile.read
- profile.search
- profile.remember
- profile.commit
scopes:
- description: OpenID Connect sign-in; an id_token is in the token response when openid was in the scope.
  flows: []
  scope: openid
- description: ID token carries email and email_verified; asks the hosted flow for a proven mailbox (Gmail or Outlook) if the account has none.
  flows: []
  scope: email
- description: Standard OIDC profile claims.
  flows: []
  scope: profile
- description: Read the user's approved Configure profile (seen on the sign-in button and token response).
  flows: []
  scope: profile.read
- description: Search the user's profile.
  flows: []
  scope: profile.search
- description: Save memories to the user's profile.
  flows: []
  scope: profile.remember
- description: Commit conversation turns to the profile.
  flows: []
  scope: profile.commit
slug: configure-dev-scopes
source_filename: configure-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.configure.dev/oidc.md\ndocs: https://docs.configure.dev/oidc.md\nnote: The OpenAPI declares no oauth2 scheme; scopes come from the OIDC and Sign in with Configure docs. If the authorization request omits scope, the scopes registered for the client apply (a client made with POST /v1/sso/client registers openid, email and profile).\nscopes:\n- name: openid\n  description: OpenID Connect sign-in; an id_token is in the token response when openid was in the scope.\n- name: email\n  description: ID token carries email and email_verified; asks the hosted flow for a proven mailbox (Gmail or Outlook) if the account has none.\n- name: profile\n  description: Standard OIDC profile claims.\n- name: profile.read\n  description: Read the user's approved Configure profile (seen on the sign-in button and token response).\n- name: profile.search\n  description: Search the user's profile.\n- name: profile.remember\n  description:\
  \ Save memories to the user's profile.\n- name: profile.commit\n  description: Commit conversation turns to the profile.\n"
source_yaml_url: https://artifacts.apis.io/configure-dev/scopes/configure-dev-scopes.yml
summary_line: 7 scopes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Memory
- Personalization
- User Context
- MCP
token_bound: false
token_urls: []
---
