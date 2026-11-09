---
api_specs:
- filename: aginera-ai-billing-api-openapi.yml
  format: yaml
  label: Aginera Billing API
  slug: aginera-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-billing-api-openapi.yml
- filename: aginera-ai-cad-api-openapi.yml
  format: yaml
  label: Aginera CAD API
  slug: aginera-ai-cad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-cad-api-openapi.yml
- filename: aginera-ai-clients-api-openapi.yml
  format: yaml
  label: Aginera Clients API
  slug: aginera-ai-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-clients-api-openapi.yml
- filename: aginera-ai-documents-api-openapi.yml
  format: yaml
  label: Aginera Documents API
  slug: aginera-ai-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-documents-api-openapi.yml
- filename: aginera-ai-exports-api-openapi.yml
  format: yaml
  label: Aginera Exports API
  slug: aginera-ai-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-exports-api-openapi.yml
- filename: aginera-ai-projects-api-openapi.yml
  format: yaml
  label: Aginera Projects API
  slug: aginera-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-projects-api-openapi.yml
- filename: aginera-ai-reference-api-openapi.yml
  format: yaml
  label: Aginera Reference API
  slug: aginera-ai-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-reference-api-openapi.yml
- filename: aginera-ai-takeoffs-api-openapi.yml
  format: yaml
  label: Aginera Takeoffs API
  slug: aginera-ai-takeoffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-takeoffs-api-openapi.yml
- filename: aginera-ai-usage-api-openapi.yml
  format: yaml
  label: Aginera Usage API
  slug: aginera-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-usage-api-openapi.yml
authorization_urls:
- https://auth.aginera.ai/oauth/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Aginera Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aginera publishes 25 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aginera API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/65f567a9-6e6a-4f81-863c-aea4ece1f8eb/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aginera
provider_slug: aginera-ai
schemes:
- description: Client credentials (service mode, Microsoft Entra ID tenant of Aginera; request scope=api://<aginera-api-app-id>/.default; granular scopes are attached to the credential) or authorization code + PKCE (delegated mode via the Aginera authorization server; scopes are consented by the user).
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/65f567a9-6e6a-4f81-863c-aea4ece1f8eb/oauth2/v2.0/token
  - authorizationUrl: https://auth.aginera.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.aginera.ai/oauth/token
  name: oauth2
  source: openapi/aginera-ai-openapi.json
- description: Client credentials (service mode, Microsoft Entra ID tenant of Aginera; request scope=api://<aginera-api-app-id>/.default; granular scopes are attached to the credential) or authorization code + PKCE (delegated mode via the Aginera authorization server; scopes are consented by the user).
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/65f567a9-6e6a-4f81-863c-aea4ece1f8eb/oauth2/v2.0/token
  - authorizationUrl: https://auth.aginera.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.aginera.ai/oauth/token
  name: oauth2
  source: openapi/aginera-openapi.json
- description: Client credentials (service mode, Microsoft Entra ID tenant of Aginera; request scope=api://<aginera-api-app-id>/.default; granular scopes are attached to the credential) or authorization code + PKCE (delegated mode via the Aginera authorization server; scopes are consented by the user).
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/65f567a9-6e6a-4f81-863c-aea4ece1f8eb/oauth2/v2.0/token
  - authorizationUrl: https://auth.aginera.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.aginera.ai/oauth/token
  name: oauth2
  source: openapi/aginera-openapi.yaml
scope_count: 25
scope_names:
- billing:read
- billing:write
- bim:generate
- bim:read
- cad:convert
- clash:run
- documents:delete
- documents:read
- documents:write
- estimates:generate
- estimates:read
- events:read
- exports:create
- exports:read
- interior:generate
- interior:read
- projects:delete
- projects:read
- projects:write
- takeoffs:deep
- takeoffs:delete
- takeoffs:read
- takeoffs:review
- takeoffs:run
- webhooks:manage
scopes:
- description: View credits and usage
  flows:
  - authorizationCode
  - clientCredentials
  scope: billing:read
- description: Purchase credits
  flows:
  - authorizationCode
  - clientCredentials
  scope: billing:write
- description: Generate BIM models + embed URLs (uses credits)
  flows:
  - authorizationCode
  - clientCredentials
  scope: bim:generate
- description: View BIM coordination models
  flows:
  - authorizationCode
  - clientCredentials
  scope: bim:read
- description: Convert PDF drawings to CAD (free to view; downloading the CAD file is a one-time purchase — paid from your credits only when you say so, otherwise via your own checkout)
  flows:
  - authorizationCode
  - clientCredentials
  scope: cad:convert
- description: Run clash detection + embed URLs (uses credits)
  flows:
  - authorizationCode
  - clientCredentials
  scope: clash:run
- description: Delete documents
  flows:
  - authorizationCode
  - clientCredentials
  scope: documents:delete
- description: View and download documents
  flows:
  - authorizationCode
  - clientCredentials
  scope: documents:read
- description: Upload drawings
  flows:
  - authorizationCode
  - clientCredentials
  scope: documents:write
- description: Generate estimates (uses credits)
  flows:
  - authorizationCode
  - clientCredentials
  scope: estimates:generate
- description: View estimates
  flows:
  - authorizationCode
  - clientCredentials
  scope: estimates:read
- description: Read the event log
  flows:
  - authorizationCode
  - clientCredentials
  scope: events:read
- description: Create exports
  flows:
  - authorizationCode
  - clientCredentials
  scope: exports:create
- description: Download exports
  flows:
  - authorizationCode
  - clientCredentials
  scope: exports:read
- description: Render floor plans and start purchases on your account (uses credits; paid add-ons need your checkout)
  flows:
  - authorizationCode
  - clientCredentials
  scope: interior:generate
- description: View floor-plan renders (dollhouse, room images, film)
  flows:
  - authorizationCode
  - clientCredentials
  scope: interior:read
- description: Delete projects
  flows:
  - authorizationCode
  - clientCredentials
  scope: projects:delete
- description: View projects
  flows:
  - authorizationCode
  - clientCredentials
  scope: projects:read
- description: Create and update projects
  flows:
  - authorizationCode
  - clientCredentials
  scope: projects:write
- description: Run deep (UI-parity) takeoffs
  flows:
  - authorizationCode
  - clientCredentials
  scope: takeoffs:deep
- description: Delete takeoffs
  flows:
  - authorizationCode
  - clientCredentials
  scope: takeoffs:delete
- description: View takeoffs, items, routes and schedules
  flows:
  - authorizationCode
  - clientCredentials
  scope: takeoffs:read
- description: Accept, reject or adjust takeoff items
  flows:
  - authorizationCode
  - clientCredentials
  scope: takeoffs:review
- description: Run takeoffs (uses credits)
  flows:
  - authorizationCode
  - clientCredentials
  scope: takeoffs:run
- description: Manage webhook endpoints
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhooks:manage
slug: aginera-ai-scopes
source_filename: aginera-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/aginera-ai-openapi.json, openapi/aginera-openapi.json, openapi/aginera-openapi.yaml\nschemes:\n- name: oauth2\n  source: openapi/aginera-ai-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/65f567a9-6e6a-4f81-863c-aea4ece1f8eb/oauth2/v2.0/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.aginera.ai/oauth/authorize\n    tokenUrl: https://auth.aginera.ai/oauth/token\n  description: Client credentials (service mode, Microsoft Entra ID tenant of Aginera; request\n    scope=api://<aginera-api-app-id>/.default; granular scopes are attached to the credential)\n    or authorization code + PKCE (delegated mode via the Aginera authorization server; scopes\n    are consented by the user).\n- name: oauth2\n  source: openapi/aginera-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/65f567a9-6e6a-4f81-863c-aea4ece1f8eb/oauth2/v2.0/token\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://auth.aginera.ai/oauth/authorize\n    tokenUrl: https://auth.aginera.ai/oauth/token\n  description: Client credentials (service mode, Microsoft Entra ID tenant of Aginera; request\n    scope=api://<aginera-api-app-id>/.default; granular scopes are attached to the credential)\n    or authorization code + PKCE (delegated mode via the Aginera authorization server; scopes\n    are consented by the user).\n- name: oauth2\n  source: openapi/aginera-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/65f567a9-6e6a-4f81-863c-aea4ece1f8eb/oauth2/v2.0/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.aginera.ai/oauth/authorize\n    tokenUrl: https://auth.aginera.ai/oauth/token\n  description: Client credentials (service mode, Microsoft Entra ID tenant of Aginera; request\n    scope=api://<aginera-api-app-id>/.default; granular scopes are attached to the credential)\n \
  \   or authorization code + PKCE (delegated mode via the Aginera authorization server; scopes\n    are consented by the user).\nscopes:\n- scope: billing:read\n  description: View credits and usage\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: billing:write\n  description: Purchase credits\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: bim:generate\n  description: Generate BIM models + embed URLs (uses credits)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: bim:read\n  description: View BIM coordination models\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n\
  \  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: cad:convert\n  description: Convert PDF drawings to CAD (free to view; downloading the CAD file is a one-time\n    purchase — paid from your credits only when you say so, otherwise via your own checkout)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: clash:run\n  description: Run clash detection + embed URLs (uses credits)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: documents:delete\n  description: Delete documents\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: documents:read\n  description: View and download\
  \ documents\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: documents:write\n  description: Upload drawings\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: estimates:generate\n  description: Generate estimates (uses credits)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: estimates:read\n  description: View estimates\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: events:read\n  description: Read the event log\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: exports:create\n  description: Create exports\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: exports:read\n  description: Download exports\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: interior:generate\n  description: Render floor plans and start purchases on your account (uses credits; paid add-ons\n    need your checkout)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: interior:read\n  description: View floor-plan renders (dollhouse, room images, film)\n  flows:\n\
  \  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: projects:delete\n  description: Delete projects\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: projects:read\n  description: View projects\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: projects:write\n  description: Create and update projects\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: takeoffs:deep\n  description: Run deep (UI-parity) takeoffs\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n\
  \  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: takeoffs:delete\n  description: Delete takeoffs\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: takeoffs:read\n  description: View takeoffs, items, routes and schedules\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: takeoffs:review\n  description: Accept, reject or adjust takeoff items\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: takeoffs:run\n  description: Run takeoffs (uses credits)\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n\
  \  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n- scope: webhooks:manage\n  description: Manage webhook endpoints\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/aginera-ai-openapi.json\n  - openapi/aginera-openapi.json\n  - openapi/aginera-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/aginera-ai/scopes/aginera-ai-scopes.yml
summary_line: 25 scopes · clientCredentials/authorizationCode
tags:
- Artificial Intelligence
- Construction
- Estimating
- MEP
- Software
token_bound: false
token_urls:
- https://login.microsoftonline.com/65f567a9-6e6a-4f81-863c-aea4ece1f8eb/oauth2/v2.0/token
- https://auth.aginera.ai/oauth/token
---
