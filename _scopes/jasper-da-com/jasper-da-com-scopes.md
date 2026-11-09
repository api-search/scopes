---
api_specs:
- filename: jasper-da-com-attachments-api-openapi.yml
  format: yaml
  label: Jasper Attachments API
  slug: jasper-da-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-attachments-api-openapi.yml
- filename: jasper-da-com-audiences-api-openapi.yml
  format: yaml
  label: Jasper Audiences API
  slug: jasper-da-com-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-audiences-api-openapi.yml
- filename: jasper-da-com-command-api-openapi.yml
  format: yaml
  label: Jasper Command API
  slug: jasper-da-com-command-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-command-api-openapi.yml
- filename: jasper-da-com-context-sources-api-openapi.yml
  format: yaml
  label: Jasper Context Sources API
  slug: jasper-da-com-context-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-context-sources-api-openapi.yml
- filename: jasper-da-com-documents-api-openapi.yml
  format: yaml
  label: Jasper Documents API
  slug: jasper-da-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-documents-api-openapi.yml
- filename: jasper-da-com-geo-api-openapi.yml
  format: yaml
  label: Jasper GEO API
  slug: jasper-da-com-geo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-geo-api-openapi.yml
- filename: jasper-da-com-image-templates-api-openapi.yml
  format: yaml
  label: Jasper Image Templates API
  slug: jasper-da-com-image-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-image-templates-api-openapi.yml
- filename: jasper-da-com-images-api-openapi.yml
  format: yaml
  label: Jasper Images API
  slug: jasper-da-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-images-api-openapi.yml
- filename: jasper-da-com-knowledge-api-openapi.yml
  format: yaml
  label: Jasper Knowledge API
  slug: jasper-da-com-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-knowledge-api-openapi.yml
- filename: jasper-da-com-products-api-openapi.yml
  format: yaml
  label: Jasper Products API
  slug: jasper-da-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-products-api-openapi.yml
- filename: jasper-da-com-projects-api-openapi.yml
  format: yaml
  label: Jasper Projects API
  slug: jasper-da-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-projects-api-openapi.yml
- filename: jasper-da-com-styles-api-openapi.yml
  format: yaml
  label: Jasper Styles API
  slug: jasper-da-com-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-styles-api-openapi.yml
- filename: jasper-da-com-tasks-api-openapi.yml
  format: yaml
  label: Jasper Tasks API
  slug: jasper-da-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-tasks-api-openapi.yml
- filename: jasper-da-com-templates-api-openapi.yml
  format: yaml
  label: Jasper Templates API
  slug: jasper-da-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-templates-api-openapi.yml
- filename: jasper-da-com-usage-api-openapi.yml
  format: yaml
  label: Jasper Usage API
  slug: jasper-da-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-usage-api-openapi.yml
- filename: jasper-da-com-users-api-openapi.yml
  format: yaml
  label: Jasper Users API
  slug: jasper-da-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-users-api-openapi.yml
- filename: jasper-da-com-voices-api-openapi.yml
  format: yaml
  label: Jasper Voices API
  slug: jasper-da-com-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-voices-api-openapi.yml
authorization_urls:
- https://api.jasper.ai/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Jasper Da Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Jasper publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jasper API on a user''s behalf.


  Tokens are issued from https://api.jasper.ai/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jasper
provider_slug: jasper-da-com
schemes:
- description: User-level authentication using OAuth bearer tokens in the Authorization header.
  flows:
  - authorizationUrl: https://api.jasper.ai/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.jasper.ai/oauth2/token
  name: oauth2
  source: openapi/jasper-da-com-api-openapi.yml
scope_count: 2
scope_names:
- user
- user:read
scopes:
- description: Read and write user information
  flows:
  - authorizationCode
  scope: user
- description: Read user information
  flows:
  - authorizationCode
  scope: user:read
slug: jasper-da-com-scopes
source_filename: jasper-da-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: derived\nsource: openapi/jasper-da-com-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/jasper-da-com-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.jasper.ai/oauth2/authorize\n    tokenUrl: https://api.jasper.ai/oauth2/token\n  description: User-level authentication using OAuth bearer tokens in the Authorization header.\nscopes:\n- scope: user\n  description: Read and write user information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jasper-da-com-api-openapi.yml\n- scope: user:read\n  description: Read user information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jasper-da-com-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/jasper-da-com/scopes/jasper-da-com-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Artificial Intelligence
- Marketing
- Automation
- Content
- Platform
- Company
token_bound: false
token_urls:
- https://api.jasper.ai/oauth2/token
---
