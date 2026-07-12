---
authorization_urls:
- https://auth.dotloop.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Dotloop Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'dotloop publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the dotloop API on a user''s behalf.


  Tokens are issued from https://auth.dotloop.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: dotloop
provider_slug: dotloop
schemes:
- description: OAuth2 authorization code flow. Access tokens are short-lived (typically 12 hours) and passed as a Bearer token. Scopes include account:read, profile:read, profile:write, loop:read, loop:write, contact:read, contact:write, and template:read.
  flows:
  - authorizationUrl: https://auth.dotloop.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.dotloop.com/oauth/token
  name: oauth2
  source: openapi/dotloop-openapi.yml
scope_count: 8
scope_names:
- account:read
- contact:read
- contact:write
- loop:read
- loop:write
- profile:read
- profile:write
- template:read
scopes:
- description: Read account details.
  flows:
  - authorizationCode
  scope: account:read
- description: Read contacts.
  flows:
  - authorizationCode
  scope: contact:read
- description: Create, update, and delete contacts.
  flows:
  - authorizationCode
  scope: contact:write
- description: Read loops, details, folders, documents, participants, tasks, and activities.
  flows:
  - authorizationCode
  scope: loop:read
- description: Create and update loops and their contents.
  flows:
  - authorizationCode
  scope: loop:write
- description: Read profiles.
  flows:
  - authorizationCode
  scope: profile:read
- description: Create and update profiles.
  flows:
  - authorizationCode
  scope: profile:write
- description: Read loop templates.
  flows:
  - authorizationCode
  scope: template:read
slug: dotloop-scopes
source_filename: dotloop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dotloop-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/dotloop-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.dotloop.com/oauth/authorize\n    tokenUrl: https://auth.dotloop.com/oauth/token\n  description: OAuth2 authorization code flow. Access tokens are short-lived (typically 12 hours)\n    and passed as a Bearer token. Scopes include account:read, profile:read, profile:write,\n    loop:read, loop:write, contact:read, contact:write, and template:read.\nscopes:\n- scope: account:read\n  description: Read account details.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dotloop-openapi.yml\n- scope: contact:read\n  description: Read contacts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dotloop-openapi.yml\n- scope: contact:write\n  description: Create, update, and delete contacts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dotloop-openapi.yml\n\
  - scope: loop:read\n  description: Read loops, details, folders, documents, participants, tasks, and activities.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dotloop-openapi.yml\n- scope: loop:write\n  description: Create and update loops and their contents.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dotloop-openapi.yml\n- scope: profile:read\n  description: Read profiles.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dotloop-openapi.yml\n- scope: profile:write\n  description: Create and update profiles.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dotloop-openapi.yml\n- scope: template:read\n  description: Read loop templates.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dotloop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/scopes/dotloop-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Real Estate
- Transaction Management
- Loops
- Documents
- E-Signature
- Zillow Group
token_urls:
- https://auth.dotloop.com/oauth/token
---
