---
authorization_urls:
- https://www.meetcleo.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cleo Scopes
name_suffix: OAuth Scopes
note: Scopes read verbatim from the scopes_supported array of Cleo's published RFC 8414 Authorization Server Metadata document. Cleo publishes no scope reference page and no OpenAPI, so no description text exists — the descriptions below are deliberately left null rather than invented. The three scope strings themselves are exactly as Cleo serves them.
overview: 'Cleo publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cleo API on a user''s behalf.


  Tokens are issued from https://www.meetcleo.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cleo
provider_slug: cleo
schemes:
- flows:
  - authorizationUrl: https://www.meetcleo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.meetcleo.com/oauth/token
  name: OAuth2
  source: https://www.meetcleo.com/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- read
- write:create
- write:delete
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: read
- description: ''
  flows:
  - authorizationCode
  scope: write:create
- description: ''
  flows:
  - authorizationCode
  scope: write:delete
slug: cleo-scopes
source_filename: cleo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://www.meetcleo.com/.well-known/oauth-authorization-server\nnote: >-\n  Scopes read verbatim from the scopes_supported array of Cleo's published RFC 8414\n  Authorization Server Metadata document. Cleo publishes no scope reference page and no\n  OpenAPI, so no description text exists — the descriptions below are deliberately left\n  null rather than invented. The three scope strings themselves are exactly as Cleo\n  serves them.\ndocs: null\ncaveat: >-\n  This authorization server's authorization_endpoint redirects to an internal admin\n  sign-in (/admin_log_in). These are not scopes an outside developer can request; they\n  are recorded as published fact about Cleo's deployment.\nschemes:\n  - name: OAuth2\n    source: https://www.meetcleo.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.meetcleo.com/oauth/authorize\n        tokenUrl: https://www.meetcleo.com/oauth/token\n\
  scopes:\n  - scope: read\n    description: null\n    flows: [authorizationCode]\n    sources: ['https://www.meetcleo.com/.well-known/oauth-authorization-server']\n  - scope: 'write:create'\n    description: null\n    flows: [authorizationCode]\n    sources: ['https://www.meetcleo.com/.well-known/oauth-authorization-server']\n  - scope: 'write:delete'\n    description: null\n    flows: [authorizationCode]\n    sources: ['https://www.meetcleo.com/.well-known/oauth-authorization-server']\nscope_count: 3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleo/refs/heads/main/scopes/cleo-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Artificial Intelligence
- Banking
- Budgeting
- Cash Advance
- Consumer Finance
- Financial Assistant
- Personal Finance
token_urls:
- https://www.meetcleo.com/oauth/token
---
