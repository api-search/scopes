---
api_specs:
- filename: linkedmash-com-analytics-api-openapi.yml
  format: yaml
  label: LinkedMash Analytics API
  slug: linkedmash-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-analytics-api-openapi.yml
- filename: linkedmash-com-bookmarks-api-openapi.yml
  format: yaml
  label: LinkedMash Bookmarks API
  slug: linkedmash-com-bookmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-bookmarks-api-openapi.yml
- filename: linkedmash-com-drafts-api-openapi.yml
  format: yaml
  label: LinkedMash Drafts API
  slug: linkedmash-com-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-drafts-api-openapi.yml
- filename: linkedmash-com-labels-api-openapi.yml
  format: yaml
  label: LinkedMash Labels API
  slug: linkedmash-com-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-labels-api-openapi.yml
- filename: linkedmash-com-media-api-openapi.yml
  format: yaml
  label: LinkedMash Media API
  slug: linkedmash-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-media-api-openapi.yml
- filename: linkedmash-com-queue-api-openapi.yml
  format: yaml
  label: LinkedMash Queue API
  slug: linkedmash-com-queue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-queue-api-openapi.yml
- filename: linkedmash-com-schedule-api-openapi.yml
  format: yaml
  label: LinkedMash Schedule API
  slug: linkedmash-com-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-schedule-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: LinkedMash Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LinkedMash publishes 7 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the LinkedMash API on a user''s behalf.


  Tokens are issued from https://api.linkedmash.com/auth/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LinkedMash
provider_slug: linkedmash-com
schemes:
- description: Short-lived, permission-scoped machine token using an existing LinkedMash API key id and secret as the confidential client credentials.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.linkedmash.com/auth/oauth/token
  name: oauthClientCredentials
  source: openapi/linkedmash-com-openapi.json
scope_count: 7
scope_names:
- analytics:read
- content:read
- content:write
- exports:read
- exports:write
- library:read
- library:write
scopes:
- description: Read account, post, and growth analytics.
  flows:
  - clientCredentials
  scope: analytics:read
- description: Read drafts, publishing queues, schedules, and media metadata.
  flows:
  - clientCredentials
  scope: content:read
- description: Create, update, delete, schedule, and publish content or media.
  flows:
  - clientCredentials
  scope: content:write
- description: Read export job status.
  flows:
  - clientCredentials
  scope: exports:read
- description: Create PDF, CSV, and JSON exports.
  flows:
  - clientCredentials
  scope: exports:write
- description: Read saved posts, labels, authors, smart folders, memories, digests, and interests.
  flows:
  - clientCredentials
  scope: library:read
- description: Manage labels, smart folders, memories, saved-post state, and interest corrections.
  flows:
  - clientCredentials
  scope: library:write
slug: linkedmash-com-scopes
source_filename: linkedmash-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/linkedmash-com-openapi.json\nschemes:\n- name: oauthClientCredentials\n  source: openapi/linkedmash-com-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.linkedmash.com/auth/oauth/token\n  description: Short-lived, permission-scoped machine token using an existing LinkedMash API\n    key id and secret as the confidential client credentials.\nscopes:\n- scope: analytics:read\n  description: Read account, post, and growth analytics.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/linkedmash-com-openapi.json\n- scope: content:read\n  description: Read drafts, publishing queues, schedules, and media metadata.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/linkedmash-com-openapi.json\n- scope: content:write\n  description: Create, update, delete, schedule, and publish content or media.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/linkedmash-com-openapi.json\n\
  - scope: exports:read\n  description: Read export job status.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/linkedmash-com-openapi.json\n- scope: exports:write\n  description: Create PDF, CSV, and JSON exports.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/linkedmash-com-openapi.json\n- scope: library:read\n  description: Read saved posts, labels, authors, smart folders, memories, digests, and interests.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/linkedmash-com-openapi.json\n- scope: library:write\n  description: Manage labels, smart folders, memories, saved-post state, and interest corrections.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/linkedmash-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/linkedmash-com/scopes/linkedmash-com-scopes.yml
summary_line: 7 scopes · clientCredentials
tags:
- LinkedIn Integration
- Content Management
- Data Export
- AI Integration
- Productivity
token_bound: false
token_urls:
- https://api.linkedmash.com/auth/oauth/token
---
