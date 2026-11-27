---
api_specs:
- filename: listdrop-co-discovery-api-openapi.yml
  format: yaml
  label: ListDrop Discovery API
  slug: listdrop-co-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-discovery-api-openapi.yml
- filename: listdrop-co-feedback-api-openapi.yml
  format: yaml
  label: ListDrop Feedback API
  slug: listdrop-co-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-feedback-api-openapi.yml
- filename: listdrop-co-lists-api-openapi.yml
  format: yaml
  label: ListDrop Lists API
  slug: listdrop-co-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-lists-api-openapi.yml
- filename: listdrop-co-read-api-openapi.yml
  format: yaml
  label: ListDrop Read API
  slug: listdrop-co-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-read-api-openapi.yml
- filename: listdrop-co-webhooks-api-openapi.yml
  format: yaml
  label: ListDrop Webhooks API
  slug: listdrop-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-webhooks-api-openapi.yml
authorization_urls:
- https://www.listdrop.co/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: ListDrop Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ListDrop publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ListDrop API on a user''s behalf.


  Tokens are issued from https://www.listdrop.co/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ListDrop
provider_slug: listdrop-co
schemes:
- description: 'OAuth 2.1: authorization-code + PKCE (S256), public clients via RFC 7591 dynamic registration at https://www.listdrop.co/api/oauth/register. Metadata: https://www.listdrop.co/.well-known/oauth-authorization-server'
  flows:
  - authorizationUrl: https://www.listdrop.co/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.listdrop.co/api/oauth/token
  name: listdropOAuth
  source: openapi/listdrop-co-openapi.json
scope_count: 2
scope_names:
- lists:read
- lists:write
scopes:
- description: Read the user's own lists, including private ones
  flows:
  - authorizationCode
  scope: lists:read
- description: Create lists in the user's account (created private)
  flows:
  - authorizationCode
  scope: lists:write
slug: listdrop-co-scopes
source_filename: listdrop-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/listdrop-co-openapi.json\nschemes:\n- name: listdropOAuth\n  source: openapi/listdrop-co-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.listdrop.co/oauth/authorize\n    tokenUrl: https://www.listdrop.co/api/oauth/token\n  description: 'OAuth 2.1: authorization-code + PKCE (S256), public clients via RFC 7591 dynamic\n    registration at https://www.listdrop.co/api/oauth/register. Metadata: https://www.listdrop.co/.well-known/oauth-authorization-server'\nscopes:\n- scope: lists:read\n  description: Read the user's own lists, including private ones\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/listdrop-co-openapi.json\n- scope: lists:write\n  description: Create lists in the user's account (created private)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/listdrop-co-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/listdrop-co/scopes/listdrop-co-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Social
- List
- Community
- Artificial Intelligence
- Platform
token_bound: false
token_urls:
- https://www.listdrop.co/api/oauth/token
---
