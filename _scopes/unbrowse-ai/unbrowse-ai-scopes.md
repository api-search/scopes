---
api_specs:
- filename: unbrowse-ai-account-api-openapi.yml
  format: yaml
  label: unbrowse-ai Account API
  slug: unbrowse-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-account-api-openapi.yml
- filename: unbrowse-ai-apps-tools-api-openapi.yml
  format: yaml
  label: unbrowse-ai Apps & tools API
  slug: unbrowse-ai-apps-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-apps-tools-api-openapi.yml
- filename: unbrowse-ai-capabilities-api-openapi.yml
  format: yaml
  label: unbrowse-ai Capabilities API
  slug: unbrowse-ai-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-capabilities-api-openapi.yml
- filename: unbrowse-ai-connected-apps-api-openapi.yml
  format: yaml
  label: unbrowse-ai Connected apps API
  slug: unbrowse-ai-connected-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-connected-apps-api-openapi.yml
- filename: unbrowse-ai-indexing-api-openapi.yml
  format: yaml
  label: unbrowse-ai Indexing API
  slug: unbrowse-ai-indexing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-indexing-api-openapi.yml
- filename: unbrowse-ai-learning-api-openapi.yml
  format: yaml
  label: unbrowse-ai Learning API
  slug: unbrowse-ai-learning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-learning-api-openapi.yml
- filename: unbrowse-ai-logins-vault-api-openapi.yml
  format: yaml
  label: unbrowse-ai Logins & vault API
  slug: unbrowse-ai-logins-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-logins-vault-api-openapi.yml
- filename: unbrowse-ai-marketplace-api-openapi.yml
  format: yaml
  label: unbrowse-ai Marketplace API
  slug: unbrowse-ai-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-marketplace-api-openapi.yml
- filename: unbrowse-ai-orgs-api-openapi.yml
  format: yaml
  label: unbrowse-ai Orgs API
  slug: unbrowse-ai-orgs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-orgs-api-openapi.yml
- filename: unbrowse-ai-pages-api-openapi.yml
  format: yaml
  label: unbrowse-ai Pages API
  slug: unbrowse-ai-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-pages-api-openapi.yml
- filename: unbrowse-ai-replays-api-openapi.yml
  format: yaml
  label: unbrowse-ai Replays API
  slug: unbrowse-ai-replays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-replays-api-openapi.yml
- filename: unbrowse-ai-runs-api-openapi.yml
  format: yaml
  label: unbrowse-ai Runs API
  slug: unbrowse-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-runs-api-openapi.yml
- filename: unbrowse-ai-saved-queries-api-openapi.yml
  format: yaml
  label: unbrowse-ai Saved queries API
  slug: unbrowse-ai-saved-queries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-saved-queries-api-openapi.yml
- filename: unbrowse-ai-sites-api-openapi.yml
  format: yaml
  label: unbrowse-ai Sites API
  slug: unbrowse-ai-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-sites-api-openapi.yml
authorization_urls:
- https://api.unbrowse.ai/authorize
- https://unbrowse.ai/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Unbrowse Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'unbrowse-ai publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the unbrowse-ai API on a user''s behalf.


  Tokens are issued from https://api.unbrowse.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: unbrowse-ai
provider_slug: unbrowse-ai
schemes:
- description: 'Authorization code with PKCE (S256). Clients may register dynamically at /oauth/register. Discovery: /.well-known/oauth-authorization-server; the REST API''s protected-resource metadata is /.well-known/oauth-protected-resource/api.'
  flows:
  - authorizationUrl: https://api.unbrowse.ai/authorize
    flow: authorizationCode
    tokenUrl: https://api.unbrowse.ai/oauth/token
  name: oauth2
  source: openapi/unbrowse-ai-openapi.json
- description: 'Authorization code with PKCE (S256). Clients may register dynamically at /oauth/register. Discovery: /.well-known/oauth-authorization-server; the REST API''s protected-resource metadata is /.well-known/oauth-protected-resource/api.'
  flows:
  - authorizationUrl: https://unbrowse.ai/authorize
    flow: authorizationCode
    tokenUrl: https://unbrowse.ai/oauth/token
  name: oauth2
  source: openapi/unbrowse-ai-openapi2.json
scope_count: 1
scope_names:
- unbrowse
scopes:
- description: Run tasks and read results on the user's behalf, with their kept logins.
  flows:
  - authorizationCode
  scope: unbrowse
slug: unbrowse-ai-scopes
source_filename: unbrowse-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/unbrowse-ai-openapi.json, openapi/unbrowse-ai-openapi2.json\nschemes:\n- name: oauth2\n  source: openapi/unbrowse-ai-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.unbrowse.ai/authorize\n    tokenUrl: https://api.unbrowse.ai/oauth/token\n  description: 'Authorization code with PKCE (S256). Clients may register dynamically at /oauth/register.\n    Discovery: /.well-known/oauth-authorization-server; the REST API''s protected-resource metadata\n    is /.well-known/oauth-protected-resource/api.'\n- name: oauth2\n  source: openapi/unbrowse-ai-openapi2.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://unbrowse.ai/authorize\n    tokenUrl: https://unbrowse.ai/oauth/token\n  description: 'Authorization code with PKCE (S256). Clients may register dynamically at /oauth/register.\n    Discovery: /.well-known/oauth-authorization-server; the REST API''s protected-resource\
  \ metadata\n    is /.well-known/oauth-protected-resource/api.'\nscopes:\n- scope: unbrowse\n  description: Run tasks and read results on the user's behalf, with their kept logins.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/unbrowse-ai-openapi.json\n  - openapi/unbrowse-ai-openapi2.json\n"
source_yaml_url: https://artifacts.apis.io/unbrowse-ai/scopes/unbrowse-ai-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- AI Agents
- Developer Tools
token_bound: false
token_urls:
- https://api.unbrowse.ai/oauth/token
- https://unbrowse.ai/oauth/token
---
