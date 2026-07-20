---
api_specs:
- filename: insforge-auth-openapi.yaml
  format: yaml
  label: Insforge Authentication API
  slug: insforge-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-auth-openapi.yaml
- filename: insforge-payments-openapi.yaml
  format: yaml
  label: Insforge Payments API
  slug: insforge-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-payments-openapi.yaml
- filename: insforge-storage-openapi.yaml
  format: yaml
  label: Insforge Storage API
  slug: insforge-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-storage-openapi.yaml
- filename: insforge-deployments-openapi.yaml
  format: yaml
  label: Insforge Deployments API
  slug: insforge-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-deployments-openapi.yaml
- filename: insforge-realtime-openapi.yaml
  format: yaml
  label: Insforge Realtime API
  slug: insforge-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-realtime-openapi.yaml
- filename: insforge-functions-openapi.yaml
  format: yaml
  label: Insforge Functions API
  slug: insforge-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-functions-openapi.yaml
- filename: insforge-ai-openapi.yaml
  format: yaml
  label: Insforge AI API
  slug: insforge-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-ai-openapi.yaml
- filename: insforge-tables-openapi.yaml
  format: yaml
  label: Insforge Tables API
  slug: insforge-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-tables-openapi.yaml
- filename: insforge-records-openapi.yaml
  format: yaml
  label: Insforge Records API
  slug: insforge-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-records-openapi.yaml
- filename: insforge-metadata-openapi.yaml
  format: yaml
  label: Insforge Metadata API
  slug: insforge-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-metadata-openapi.yaml
- filename: insforge-secrets-openapi.yaml
  format: yaml
  label: Insforge Secrets API
  slug: insforge-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-secrets-openapi.yaml
- filename: insforge-email-openapi.yaml
  format: yaml
  label: Insforge Email API
  slug: insforge-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-email-openapi.yaml
- filename: insforge-logs-openapi.yaml
  format: yaml
  label: Insforge Logs API
  slug: insforge-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-logs-openapi.yaml
- filename: insforge-health-openapi.yaml
  format: yaml
  label: Insforge Health API
  slug: insforge-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/openapi/insforge-health-openapi.yaml
authorization_urls:
- https://api.insforge.dev/api/oauth/v1/authorize
description: ''
docs: https://api.insforge.dev/.well-known/oauth-authorization-server
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Insforge Scopes
name_suffix: OAuth Scopes
note: OAuth 2.0 scopes are published by the InsForge authorization server metadata (RFC 8414), not by the per-service OpenAPI specs (which declare bearer/api-key auth). The authorization server also advertises an agent_auth block supporting WorkOS ID-JAG identity_assertion for autonomous agent registration.
overview: 'Insforge publishes 11 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Insforge API on a user''s behalf.


  Tokens are issued from https://api.insforge.dev/api/oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Insforge
provider_slug: insforge
schemes:
- codeChallengeMethods:
  - S256
  - plain
  flows:
  - authorizationUrl: https://api.insforge.dev/api/oauth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.insforge.dev/api/oauth/v1/token
  - deviceAuthorizationUrl: https://api.insforge.dev/api/oauth/v1/device_authorization
    flow: deviceCode
    tokenUrl: https://api.insforge.dev/api/oauth/v1/token
  introspectionEndpoint: https://api.insforge.dev/api/oauth/v1/introspect
  issuer: https://api.insforge.dev
  name: OAuth2
  registrationEndpoint: https://api.insforge.dev/api/oauth/v1/clients/register
  revocationEndpoint: https://api.insforge.dev/api/oauth/v1/revoke
  source: https://api.insforge.dev/.well-known/oauth-authorization-server
scope_count: 11
scope_names:
- user:read
- organizations:read
- organizations:write
- organizations:delete
- projects:read
- projects:write
- projects:delete
- projects.database:read
- projects.database:write
- projects.storage:read
- projects.storage:write
scopes:
- description: Read the authenticated user's profile.
  flows:
  - authorizationCode
  - deviceCode
  scope: user:read
- description: Read organizations the user belongs to.
  flows:
  - authorizationCode
  - deviceCode
  scope: organizations:read
- description: Create and update organizations.
  flows:
  - authorizationCode
  - deviceCode
  scope: organizations:write
- description: Delete organizations.
  flows:
  - authorizationCode
  - deviceCode
  scope: organizations:delete
- description: Read projects within an organization.
  flows:
  - authorizationCode
  - deviceCode
  scope: projects:read
- description: Create and update projects.
  flows:
  - authorizationCode
  - deviceCode
  scope: projects:write
- description: Delete projects.
  flows:
  - authorizationCode
  - deviceCode
  scope: projects:delete
- description: Read a project's database schema and records.
  flows:
  - authorizationCode
  - deviceCode
  scope: projects.database:read
- description: Write to a project's database schema and records.
  flows:
  - authorizationCode
  - deviceCode
  scope: projects.database:write
- description: Read a project's storage buckets and objects.
  flows:
  - authorizationCode
  - deviceCode
  scope: projects.storage:read
- description: Write to a project's storage buckets and objects.
  flows:
  - authorizationCode
  - deviceCode
  scope: projects.storage:write
slug: insforge-scopes
source_filename: insforge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.insforge.dev/.well-known/oauth-authorization-server\ndocs: https://api.insforge.dev/.well-known/oauth-authorization-server\nnote: >-\n  OAuth 2.0 scopes are published by the InsForge authorization server metadata\n  (RFC 8414), not by the per-service OpenAPI specs (which declare bearer/api-key\n  auth). The authorization server also advertises an agent_auth block supporting\n  WorkOS ID-JAG identity_assertion for autonomous agent registration.\nschemes:\n- name: OAuth2\n  source: https://api.insforge.dev/.well-known/oauth-authorization-server\n  issuer: https://api.insforge.dev\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.insforge.dev/api/oauth/v1/authorize\n    tokenUrl: https://api.insforge.dev/api/oauth/v1/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://api.insforge.dev/api/oauth/v1/device_authorization\n    tokenUrl: https://api.insforge.dev/api/oauth/v1/token\n\
  \  registrationEndpoint: https://api.insforge.dev/api/oauth/v1/clients/register\n  revocationEndpoint: https://api.insforge.dev/api/oauth/v1/revoke\n  introspectionEndpoint: https://api.insforge.dev/api/oauth/v1/introspect\n  codeChallengeMethods: [S256, plain]\nscopes:\n- scope: user:read\n  description: Read the authenticated user's profile.\n  flows: [authorizationCode, deviceCode]\n- scope: organizations:read\n  description: Read organizations the user belongs to.\n  flows: [authorizationCode, deviceCode]\n- scope: organizations:write\n  description: Create and update organizations.\n  flows: [authorizationCode, deviceCode]\n- scope: organizations:delete\n  description: Delete organizations.\n  flows: [authorizationCode, deviceCode]\n- scope: projects:read\n  description: Read projects within an organization.\n  flows: [authorizationCode, deviceCode]\n- scope: projects:write\n  description: Create and update projects.\n  flows: [authorizationCode, deviceCode]\n- scope: projects:delete\n\
  \  description: Delete projects.\n  flows: [authorizationCode, deviceCode]\n- scope: projects.database:read\n  description: Read a project's database schema and records.\n  flows: [authorizationCode, deviceCode]\n- scope: projects.database:write\n  description: Write to a project's database schema and records.\n  flows: [authorizationCode, deviceCode]\n- scope: projects.storage:read\n  description: Read a project's storage buckets and objects.\n  flows: [authorizationCode, deviceCode]\n- scope: projects.storage:write\n  description: Write to a project's storage buckets and objects.\n  flows: [authorizationCode, deviceCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insforge/refs/heads/main/scopes/insforge-scopes.yml
summary_line: 11 scopes · authorizationCode/deviceCode
tags:
- Company
- Backend as a Service
- Agent Native
- Cloud Infrastructure
- Database
- Authentication
- Storage
- Serverless
- Edge Functions
- AI Gateway
- Payments
- Realtime
- Open Source
- Y Combinator
token_urls:
- https://api.insforge.dev/api/oauth/v1/token
---
