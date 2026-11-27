---
api_specs:
- filename: everypage-co-account-api-openapi.yml
  format: yaml
  label: EveryPage Account API
  slug: everypage-co-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-account-api-openapi.yml
- filename: everypage-co-embedding-api-openapi.yml
  format: yaml
  label: EveryPage Embedding API
  slug: everypage-co-embedding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-embedding-api-openapi.yml
- filename: everypage-co-events-api-openapi.yml
  format: yaml
  label: EveryPage Events API
  slug: everypage-co-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-events-api-openapi.yml
- filename: everypage-co-files-api-openapi.yml
  format: yaml
  label: EveryPage Files API
  slug: everypage-co-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-files-api-openapi.yml
- filename: everypage-co-oauth-api-openapi.yml
  format: yaml
  label: EveryPage OAuth API
  slug: everypage-co-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-oauth-api-openapi.yml
- filename: everypage-co-variants-api-openapi.yml
  format: yaml
  label: EveryPage Variants API
  slug: everypage-co-variants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-variants-api-openapi.yml
- filename: everypage-co-webhooks-api-openapi.yml
  format: yaml
  label: EveryPage Webhooks API
  slug: everypage-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/everypage-co/openapi/everypage-co-webhooks-api-openapi.yml
authorization_urls:
- https://everypage.co/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: EveryPage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EveryPage publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the EveryPage API on a user''s behalf.


  Tokens are issued from https://everypage.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EveryPage
provider_slug: everypage-co
schemes:
- description: Authorization Code + PKCE (S256 only, no plain). Client authentication on the token and revoke endpoints via HTTP Basic or `client_id`/`client_secret` body params; public clients send `client_id` alone. Refresh tokens rotate on every refresh (the previous one is retired; reusing it revokes the token family) and may be down-scoped with `scope`. Each operation lists the scope it requires.
  flows:
  - authorizationUrl: https://everypage.co/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://everypage.co/oauth/token
  name: oauth2
  source: openapi/everypage-openapi.json
scope_count: 5
scope_names:
- files:read
- files:write
- profile
- readership:read
- webhooks:manage
scopes:
- description: See your files and share links
  flows:
  - authorizationCode
  scope: files:read
- description: Upload, configure, and delete files
  flows:
  - authorizationCode
  scope: files:write
- description: See your account email and plan
  flows:
  - authorizationCode
  scope: profile
- description: See who read your documents
  flows:
  - authorizationCode
  scope: readership:read
- description: Create, list, test, and delete webhook subscriptions
  flows:
  - authorizationCode
  scope: webhooks:manage
slug: everypage-co-scopes
source_filename: everypage-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/everypage-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/everypage-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://everypage.co/oauth/authorize\n    tokenUrl: https://everypage.co/oauth/token\n  description: Authorization Code + PKCE (S256 only, no plain). Client authentication on the\n    token and revoke endpoints via HTTP Basic or `client_id`/`client_secret` body params; public\n    clients send `client_id` alone. Refresh tokens rotate on every refresh (the previous one\n    is retired; reusing it revokes the token family) and may be down-scoped with `scope`. Each\n    operation lists the scope it requires.\nscopes:\n- scope: files:read\n  description: See your files and share links\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/everypage-openapi.json\n- scope: files:write\n  description: Upload, configure, and delete files\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/everypage-openapi.json\n- scope: profile\n  description: See your account email and plan\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/everypage-openapi.json\n- scope: readership:read\n  description: See who read your documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/everypage-openapi.json\n- scope: webhooks:manage\n  description: Create, list, test, and delete webhook subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/everypage-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/everypage-co/scopes/everypage-co-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- PDF
- Document Sharing
- ReaderAnalytics
- Privacy
- Software-as-a-Service
token_bound: false
token_urls:
- https://everypage.co/oauth/token
---
