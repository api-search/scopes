---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Project44 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'project44 publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the project44 API on a user''s behalf.


  Tokens are issued from https://api.project44.com/api/v4/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: project44
provider_slug: project44
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.project44.com/api/v4/oauth2/token
  name: oauth2
  source: openapi/project44-tracking-openapi.yml
scope_count: 3
scope_names:
- tracking.read
- tracking.write
- webhooks.write
scopes:
- description: Read shipment tracking data
  flows:
  - clientCredentials
  scope: tracking.read
- description: Create and manage shipments
  flows:
  - clientCredentials
  scope: tracking.write
- description: Manage webhook subscriptions
  flows:
  - clientCredentials
  scope: webhooks.write
slug: project44-scopes
source_filename: project44-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/project44-tracking-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/project44-tracking-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.project44.com/api/v4/oauth2/token\nscopes:\n- scope: tracking.read\n  description: Read shipment tracking data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/project44-tracking-openapi.yml\n- scope: tracking.write\n  description: Create and manage shipments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/project44-tracking-openapi.yml\n- scope: webhooks.write\n  description: Manage webhook subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/project44-tracking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/project44/refs/heads/main/scopes/project44-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Logistics
- Supply Chain Visibility
- Tracking
- Freight
- Multi-modal
token_urls:
- https://api.project44.com/api/v4/oauth2/token
---
