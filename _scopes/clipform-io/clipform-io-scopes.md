---
api_specs:
- filename: clipform-io-analytics-api-openapi.yml
  format: yaml
  label: Clipform Analytics API
  slug: clipform-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-analytics-api-openapi.yml
- filename: clipform-io-authentication-api-openapi.yml
  format: yaml
  label: Clipform Authentication API
  slug: clipform-io-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-authentication-api-openapi.yml
- filename: clipform-io-dynamic-links-api-openapi.yml
  format: yaml
  label: Clipform Dynamic Links API
  slug: clipform-io-dynamic-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-dynamic-links-api-openapi.yml
- filename: clipform-io-forms-api-openapi.yml
  format: yaml
  label: Clipform Forms API
  slug: clipform-io-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-forms-api-openapi.yml
- filename: clipform-io-integrations-api-openapi.yml
  format: yaml
  label: Clipform Integrations API
  slug: clipform-io-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-integrations-api-openapi.yml
- filename: clipform-io-node-media-api-openapi.yml
  format: yaml
  label: Clipform Node Media API
  slug: clipform-io-node-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-node-media-api-openapi.yml
- filename: clipform-io-nodes-api-openapi.yml
  format: yaml
  label: Clipform Nodes API
  slug: clipform-io-nodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-nodes-api-openapi.yml
- filename: clipform-io-tags-api-openapi.yml
  format: yaml
  label: Clipform Tags API
  slug: clipform-io-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-tags-api-openapi.yml
- filename: clipform-io-tracked-links-api-openapi.yml
  format: yaml
  label: Clipform Tracked Links API
  slug: clipform-io-tracked-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-tracked-links-api-openapi.yml
- filename: clipform-io-webhooks-api-openapi.yml
  format: yaml
  label: Clipform Webhooks API
  slug: clipform-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipform-io/openapi/clipform-io-webhooks-api-openapi.yml
authorization_urls:
- https://api.clipform.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Clipform Scopes
name_suffix: OAuth Scopes
note: No scopes reference page found in the docs; the OAuth docs page listed in llms.txt returned 404. Scopes are from the OpenAPI only.
overview: 'Clipform publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clipform API on a user''s behalf.


  Tokens are issued from https://api.clipform.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clipform
provider_slug: clipform-io
schemes:
- description: Authorization-code OAuth for installed apps acting on a user's workspace. Access tokens (cf_at_*) are passed as Bearer tokens and authorize the Integrations operations. They are opaque, single-audience, server-side records. Client credentials are issued per app - contact support@clipform.io.
  flows:
  - authorizationUrl: https://api.clipform.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.clipform.io/oauth/token
  name: oauth2
  source: openapi/clipform-io-openapi.yml
scope_count: 3
scope_names:
- forms:read
- responses:read
- webhooks:manage
scopes:
- description: Read the workspace's forms.
  flows:
  - authorizationCode
  scope: forms:read
- description: Read the workspace's form responses.
  flows:
  - authorizationCode
  scope: responses:read
- description: Subscribe and unsubscribe webhook endpoints.
  flows:
  - authorizationCode
  scope: webhooks:manage
slug: clipform-io-scopes
source_filename: clipform-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/clipform-io-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/clipform-io-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.clipform.io/oauth/authorize\n    tokenUrl: https://api.clipform.io/oauth/token\n  description: Authorization-code OAuth for installed apps acting on a user's workspace. Access tokens\n    (cf_at_*) are passed as Bearer tokens and authorize the Integrations operations. They are opaque,\n    single-audience, server-side records. Client credentials are issued per app - contact support@clipform.io.\nscopes:\n- scope: forms:read\n  description: Read the workspace's forms.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/clipform-io-openapi.yml\n- scope: responses:read\n  description: Read the workspace's form responses.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/clipform-io-openapi.yml\n- scope: webhooks:manage\n  description: Subscribe\
  \ and unsubscribe webhook endpoints.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/clipform-io-openapi.yml\nnote: No scopes reference page found in the docs; the OAuth docs page listed in llms.txt returned 404.\n  Scopes are from the OpenAPI only.\n"
source_yaml_url: https://artifacts.apis.io/clipform-io/scopes/clipform-io-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Forms
- Form Builder
- Video
- Surveys
- Webhook
- MCP
- Lead Capture
token_bound: false
token_urls:
- https://api.clipform.io/oauth/token
---
