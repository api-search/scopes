---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Warner Bros Discovery Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Warner Bros. Discovery publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Warner Bros. Discovery API on a user''s behalf.


  Tokens are issued from https://auth.warnermedia.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Warner Bros. Discovery
provider_slug: warner-bros-discovery
schemes:
- description: OAuth 2.0 client credentials flow for partner authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.warnermedia.com/oauth/token
  name: OAuth2
  source: openapi/warner-bros-discovery-content-partner-openapi.yml
scope_count: 4
scope_names:
- content:read
- content:write
- metadata:read
- metadata:write
scopes:
- description: Read content delivery information
  flows:
  - clientCredentials
  scope: content:read
- description: Submit content deliveries
  flows:
  - clientCredentials
  scope: content:write
- description: Read metadata submissions
  flows:
  - clientCredentials
  scope: metadata:read
- description: Submit metadata
  flows:
  - clientCredentials
  scope: metadata:write
slug: warner-bros-discovery-scopes
source_filename: warner-bros-discovery-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/warner-bros-discovery-content-partner-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/warner-bros-discovery-content-partner-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.warnermedia.com/oauth/token\n  description: OAuth 2.0 client credentials flow for partner authentication\nscopes:\n- scope: content:read\n  description: Read content delivery information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/warner-bros-discovery-content-partner-openapi.yml\n- scope: content:write\n  description: Submit content deliveries\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/warner-bros-discovery-content-partner-openapi.yml\n- scope: metadata:read\n  description: Read metadata submissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/warner-bros-discovery-content-partner-openapi.yml\n- scope: metadata:write\n  description: Submit metadata\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/warner-bros-discovery-content-partner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warner-bros-discovery/refs/heads/main/scopes/warner-bros-discovery-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Entertainment
- Media
- Streaming
- Content
- Television
- Film
token_urls:
- https://auth.warnermedia.com/oauth/token
---
