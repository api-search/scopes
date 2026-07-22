---
authorization_urls:
- https://app.matik.io/oauth/authorize
description: ''
docs: https://developer.matik.io/guides/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Matik Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Matik publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Matik API on a user''s behalf.


  Tokens are issued from https://app.matik.io/api/v1/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Matik
provider_slug: matik
schemes:
- flows:
  - authorizationUrl: https://app.matik.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.matik.io/api/v1/oauth/token/
  name: OAuth2
  source: https://developer.matik.io/guides/oauth
scope_count: 2
scope_names:
- producer
- consumer
scopes:
- description: Administrative access. Create and manage templates, data sources, and dynamic content, and perform producer-level operations.
  flows:
  - authorizationCode
  scope: producer
- description: End-user access. Generate presentations, documents, and spreadsheets from existing templates and run dynamic content.
  flows:
  - authorizationCode
  scope: consumer
slug: matik-scopes
source_filename: matik-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.matik.io/guides/oauth\ndocs: https://developer.matik.io/guides/oauth\nschemes:\n  - name: OAuth2\n    source: https://developer.matik.io/guides/oauth\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.matik.io/oauth/authorize\n        tokenUrl: https://app.matik.io/api/v1/oauth/token/\nscopes:\n  - scope: producer\n    description: >-\n      Administrative access. Create and manage templates, data sources, and dynamic\n      content, and perform producer-level operations.\n    flows: [authorizationCode]\n    sources: [https://developer.matik.io/guides/oauth]\n  - scope: consumer\n    description: >-\n      End-user access. Generate presentations, documents, and spreadsheets from\n      existing templates and run dynamic content.\n    flows: [authorizationCode]\n    sources: [https://developer.matik.io/guides/oauth]\nnotes: >-\n  Scopes may be requested together (\"producer\
  \ consumer\") or individually. Client\n  credentials are registered with the scopes the integration needs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matik/refs/heads/main/scopes/matik-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Content Automation
- Presentations
- Documents
- Data-Driven Content
- Sales Enablement
- Customer Success
- Revenue Operations
- AI
- MCP
token_urls:
- https://app.matik.io/api/v1/oauth/token/
---
