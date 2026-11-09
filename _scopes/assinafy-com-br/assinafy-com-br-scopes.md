---
api_specs:
- filename: assinafy-com-br-accounts-api-openapi.yml
  format: yaml
  label: Assinafy Accounts API
  slug: assinafy-com-br-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-accounts-api-openapi.yml
- filename: assinafy-com-br-assignments-api-openapi.yml
  format: yaml
  label: Assinafy Assignments API
  slug: assinafy-com-br-assignments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-assignments-api-openapi.yml
- filename: assinafy-com-br-authentication-api-openapi.yml
  format: yaml
  label: Assinafy Authentication API
  slug: assinafy-com-br-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-authentication-api-openapi.yml
- filename: assinafy-com-br-contracts-api-openapi.yml
  format: yaml
  label: Assinafy Contracts API
  slug: assinafy-com-br-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-contracts-api-openapi.yml
- filename: assinafy-com-br-documents-api-openapi.yml
  format: yaml
  label: Assinafy Documents API
  slug: assinafy-com-br-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-documents-api-openapi.yml
- filename: assinafy-com-br-fields-api-openapi.yml
  format: yaml
  label: Assinafy Fields API
  slug: assinafy-com-br-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-fields-api-openapi.yml
- filename: assinafy-com-br-oauth-api-openapi.yml
  format: yaml
  label: Assinafy OAuth API
  slug: assinafy-com-br-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-oauth-api-openapi.yml
- filename: assinafy-com-br-signers-api-openapi.yml
  format: yaml
  label: Assinafy Signers API
  slug: assinafy-com-br-signers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-signers-api-openapi.yml
- filename: assinafy-com-br-signing-api-openapi.yml
  format: yaml
  label: Assinafy Signing API
  slug: assinafy-com-br-signing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-signing-api-openapi.yml
- filename: assinafy-com-br-tags-api-openapi.yml
  format: yaml
  label: Assinafy Tags API
  slug: assinafy-com-br-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-tags-api-openapi.yml
- filename: assinafy-com-br-templates-api-openapi.yml
  format: yaml
  label: Assinafy Templates API
  slug: assinafy-com-br-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-templates-api-openapi.yml
- filename: assinafy-com-br-users-api-openapi.yml
  format: yaml
  label: Assinafy Users API
  slug: assinafy-com-br-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-users-api-openapi.yml
- filename: assinafy-com-br-webhook-payloads-api-openapi.yml
  format: yaml
  label: Assinafy Webhook Payloads API
  slug: assinafy-com-br-webhook-payloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-webhook-payloads-api-openapi.yml
- filename: assinafy-com-br-webhooks-api-openapi.yml
  format: yaml
  label: Assinafy Webhooks API
  slug: assinafy-com-br-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/assinafy-com-br/openapi/assinafy-com-br-webhooks-api-openapi.yml
authorization_urls:
- https://auth.assinafy.com.br/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Assinafy Com Br Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Assinafy publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Assinafy API on a user''s behalf.


  Tokens are issued from https://api.assinafy.com.br/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Assinafy
provider_slug: assinafy-com-br
schemes:
- description: 'OAuth 2.1 authorization code flow with mandatory PKCE (S256), for applications and AI assistants acting in a user''s workspace with that user''s permission — as opposed to `apiKeyAuth`/`bearerAuth`, which authenticate the workspace or user directly. A token carries only the scopes the user approved and works for one workspace. Endpoints are published by the authorization server at `https://auth.assinafy.com.br/.well-known/oauth-authorization-server`. An OAuth token cannot reach billing, account lifecycle, credential management or admin surfaces regardless of scope. A missing scope answers `403` with `WWW-Authenticate: Bearer error="insufficient_scope"` naming it. See **OAuth Integration Guide** for the full flow.'
  flows:
  - authorizationUrl: https://auth.assinafy.com.br/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.assinafy.com.br/v1/oauth/token
  name: oauth2
  source: openapi/assinafy-com-br-openapi.json
scope_count: 10
scope_names:
- account:read
- documents:read
- documents:write
- email
- offline_access
- openid
- profile
- templates:read
- templates:write
- webhooks:write
scopes:
- description: Read the workspace's profile, theme and logo.
  flows:
  - authorizationCode
  scope: account:read
- description: Read documents, their pages, tags, signers, assignments and activity, and the WhatsApp notifications sent for an assignment.
  flows:
  - authorizationCode
  scope: documents:read
- description: Create, update and delete documents, and manage their signers, assignments and activity.
  flows:
  - authorizationCode
  scope: documents:write
- description: Include the user's email and its verification status in the `id_token`/userinfo claims.
  flows:
  - authorizationCode
  scope: email
- description: Request a refresh token, so the app keeps working after the user's session expires without prompting them again. Only granted to a client that explicitly asks for it.
  flows:
  - authorizationCode
  scope: offline_access
- description: Identify the authenticated user (OpenID Connect `sub` claim) and enable the `/v1/oauth/userinfo` endpoint.
  flows:
  - authorizationCode
  scope: openid
- description: Include the user's name in the `id_token`/userinfo claims.
  flows:
  - authorizationCode
  scope: profile
- description: Read reusable document templates, their pages, roles, fields and tags.
  flows:
  - authorizationCode
  scope: templates:read
- description: Create, update and delete templates, their pages, roles, fields and tags.
  flows:
  - authorizationCode
  scope: templates:write
- description: Change the workspace's webhook subscription (delivery URL, events, contact email), deactivate it, manage webhook endpoints and re-send a delivery.
  flows:
  - authorizationCode
  scope: webhooks:write
slug: assinafy-com-br-scopes
source_filename: assinafy-com-br-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/assinafy-com-br-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/assinafy-com-br-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.assinafy.com.br/oauth/authorize\n    tokenUrl: https://api.assinafy.com.br/v1/oauth/token\n  description: 'OAuth 2.1 authorization code flow with mandatory PKCE (S256), for applications\n    and AI assistants acting in a user''s workspace with that user''s permission — as opposed\n    to `apiKeyAuth`/`bearerAuth`, which authenticate the workspace or user directly. A token\n    carries only the scopes the user approved and works for one workspace. Endpoints are published\n    by the authorization server at `https://auth.assinafy.com.br/.well-known/oauth-authorization-server`.\n    An OAuth token cannot reach billing, account lifecycle, credential management or admin surfaces\n    regardless of scope. A missing scope answers `403` with `WWW-Authenticate:\
  \ Bearer error=\"insufficient_scope\"`\n    naming it. See **OAuth Integration Guide** for the full flow.'\nscopes:\n- scope: account:read\n  description: Read the workspace's profile, theme and logo.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- scope: documents:read\n  description: Read documents, their pages, tags, signers, assignments and activity, and the\n    WhatsApp notifications sent for an assignment.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- scope: documents:write\n  description: Create, update and delete documents, and manage their signers, assignments and\n    activity.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- scope: email\n  description: Include the user's email and its verification status in the `id_token`/userinfo\n    claims.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- scope: offline_access\n\
  \  description: Request a refresh token, so the app keeps working after the user's session expires\n    without prompting them again. Only granted to a client that explicitly asks for it.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- scope: openid\n  description: Identify the authenticated user (OpenID Connect `sub` claim) and enable the `/v1/oauth/userinfo`\n    endpoint.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- scope: profile\n  description: Include the user's name in the `id_token`/userinfo claims.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- scope: templates:read\n  description: Read reusable document templates, their pages, roles, fields and tags.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- scope: templates:write\n  description: Create, update and delete templates, their pages, roles, fields and tags.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n- scope: webhooks:write\n  description: Change the workspace's webhook subscription (delivery URL, events, contact email),\n    deactivate it, manage webhook endpoints and re-send a delivery.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/assinafy-com-br-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/assinafy-com-br/scopes/assinafy-com-br-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- E-Signature
- Document Management
- Brazil
- Free
token_bound: false
token_urls:
- https://api.assinafy.com.br/v1/oauth/token
---
