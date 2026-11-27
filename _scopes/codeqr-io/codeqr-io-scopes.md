---
api_specs:
- filename: codeqr-io-analytics-api-openapi.yml
  format: yaml
  label: CodeQR Analytics API
  slug: codeqr-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-analytics-api-openapi.yml
- filename: codeqr-io-domains-api-openapi.yml
  format: yaml
  label: CodeQR Domains API
  slug: codeqr-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-domains-api-openapi.yml
- filename: codeqr-io-events-api-openapi.yml
  format: yaml
  label: CodeQR Events API
  slug: codeqr-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-events-api-openapi.yml
- filename: codeqr-io-folders-api-openapi.yml
  format: yaml
  label: CodeQR Folders API
  slug: codeqr-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-folders-api-openapi.yml
- filename: codeqr-io-links-api-openapi.yml
  format: yaml
  label: CodeQR Links API
  slug: codeqr-io-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-links-api-openapi.yml
- filename: codeqr-io-projects-api-openapi.yml
  format: yaml
  label: CodeQR Projects API
  slug: codeqr-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-projects-api-openapi.yml
- filename: codeqr-io-qr-codes-api-openapi.yml
  format: yaml
  label: CodeQR QR Codes API
  slug: codeqr-io-qr-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-qr-codes-api-openapi.yml
- filename: codeqr-io-tags-api-openapi.yml
  format: yaml
  label: CodeQR Tags API
  slug: codeqr-io-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-tags-api-openapi.yml
- filename: codeqr-io-track-api-openapi.yml
  format: yaml
  label: CodeQR Track API
  slug: codeqr-io-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeqr-io/openapi/codeqr-io-track-api-openapi.yml
authorization_urls:
- https://app.codeqr.io/oauth/authorize
description: ''
docs: https://docs.codeqr.io/integrations/quickstart.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: CodeQR Scopes
name_suffix: OAuth Scopes
note: Scopes are not declared in the OpenAPI (bearer only); MCP connection uses scope mcp:tools per https://docs.codeqr.io/mcp/introduction.md
overview: 'CodeQR publishes 17 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CodeQR API on a user''s behalf.


  Tokens are issued from https://api.codeqr.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CodeQR
provider_slug: codeqr-io
schemes: []
scope_count: 17
scope_names:
- projects.read
- projects.write
- links.read
- links.write
- qrcodes.read
- qrcodes.write
- tags.read
- tags.write
- pages.read
- pages.write
- analytics.read
- domains.read
- domains.write
- conversions.write
- webhooks.read
- webhooks.write
- user.read
scopes:
- description: Read access to projects.
  flows: []
  scope: projects.read
- description: Write access to projects.
  flows: []
  scope: projects.write
- description: Read access to links.
  flows: []
  scope: links.read
- description: Write access to links.
  flows: []
  scope: links.write
- description: Read access to QR Codes.
  flows: []
  scope: qrcodes.read
- description: Write access to QR Codes.
  flows: []
  scope: qrcodes.write
- description: Read access to tags.
  flows: []
  scope: tags.read
- description: Write access to tags.
  flows: []
  scope: tags.write
- description: Read access to pages.
  flows: []
  scope: pages.read
- description: Write access to pages.
  flows: []
  scope: pages.write
- description: Read access to analytics.
  flows: []
  scope: analytics.read
- description: Read access to domains.
  flows: []
  scope: domains.read
- description: Write access to domains.
  flows: []
  scope: domains.write
- description: Record lead and sale conversion events on your behalf.
  flows: []
  scope: conversions.write
- description: Read access to webhooks.
  flows: []
  scope: webhooks.read
- description: Write access to webhooks.
  flows: []
  scope: webhooks.write
- description: Read access to user information. This scope is included by default.
  flows: []
  scope: user.read
slug: codeqr-io-scopes
source_filename: codeqr-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.codeqr.io/integrations/quickstart.md\ndocs: https://docs.codeqr.io/integrations/quickstart.md\nauthorization_url: https://app.codeqr.io/oauth/authorize\ntoken_url: https://api.codeqr.io/oauth/token\nscopes:\n- name: projects.read\n  description: Read access to projects.\n- name: projects.write\n  description: Write access to projects.\n- name: links.read\n  description: Read access to links.\n- name: links.write\n  description: Write access to links.\n- name: qrcodes.read\n  description: Read access to QR Codes.\n- name: qrcodes.write\n  description: Write access to QR Codes.\n- name: tags.read\n  description: Read access to tags.\n- name: tags.write\n  description: Write access to tags.\n- name: pages.read\n  description: Read access to pages.\n- name: pages.write\n  description: Write access to pages.\n- name: analytics.read\n  description: Read access to analytics.\n- name: domains.read\n  description: Read\
  \ access to domains.\n- name: domains.write\n  description: Write access to domains.\n- name: conversions.write\n  description: Record lead and sale conversion events on your behalf.\n- name: webhooks.read\n  description: Read access to webhooks.\n- name: webhooks.write\n  description: Write access to webhooks.\n- name: user.read\n  description: Read access to user information. This scope is included by default.\nnote: Scopes are not declared in the OpenAPI (bearer only); MCP connection uses scope mcp:tools per https://docs.codeqr.io/mcp/introduction.md\n"
source_yaml_url: https://artifacts.apis.io/codeqr-io/scopes/codeqr-io-scopes.yml
summary_line: 17 scopes
tags:
- Company
- QR Codes
- Short Links
- URL Shorteners
- Link Management
- Analytics
- Marketing
- MCP
token_bound: false
token_urls:
- https://api.codeqr.io/oauth/token
---
