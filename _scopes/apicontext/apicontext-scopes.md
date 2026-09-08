---
api_specs:
- filename: apicontext-platform-openapi.yml
  format: yaml
  label: APIContext Platform API
  slug: apicontext-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-platform-openapi.yml
- filename: apicontext-api-calls-api-openapi.yml
  format: yaml
  label: APIContext Calls API
  slug: apicontext-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-api-calls-api-openapi.yml
- filename: apicontext-schedules-api-openapi.yml
  format: yaml
  label: APIContext Schedules API
  slug: apicontext-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-schedules-api-openapi.yml
- filename: apicontext-webhooks-openapi.yml
  format: yaml
  label: APIContext Webhooks API
  slug: apicontext-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-webhooks-openapi.yml
- filename: apicontext-workflows-api-openapi.yml
  format: yaml
  label: APIContext Workflows API
  slug: apicontext-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-workflows-api-openapi.yml
- filename: apicontext-governance-openapi.yml
  format: yaml
  label: APIContext Governance API
  slug: apicontext-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-governance-openapi.yml
- filename: apicontext-statistics-api-openapi.yml
  format: yaml
  label: APIContext Stats API
  slug: apicontext-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-statistics-api-openapi.yml
- filename: apicontext-results-api-openapi.yml
  format: yaml
  label: APIContext Results API
  slug: apicontext-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-results-api-openapi.yml
- filename: apicontext-agents-api-openapi.yml
  format: yaml
  label: APIContext Agents API
  slug: apicontext-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-agents-api-openapi.yml
- filename: apicontext-projects-api-openapi.yml
  format: yaml
  label: APIContext Projects API
  slug: apicontext-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-projects-api-openapi.yml
- filename: apicontext-insights-api-openapi.yml
  format: yaml
  label: APIContext Insights API
  slug: apicontext-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-insights-api-openapi.yml
- filename: apicontext-tokens-api-openapi.yml
  format: yaml
  label: APIContext Auth Tokens API
  slug: apicontext-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-tokens-api-openapi.yml
- filename: apicontext-mcp-monitors-openapi.yml
  format: yaml
  label: APIContext MCP Monitors API
  slug: apicontext-mcp-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-mcp-monitors-openapi.yml
- filename: apicontext-reports-api-openapi.yml
  format: yaml
  label: APIContext Reports API
  slug: apicontext-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-reports-api-openapi.yml
- filename: apicontext-alerts-api-openapi.yml
  format: yaml
  label: APIContext Notifications API
  slug: apicontext-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-alerts-api-openapi.yml
- filename: apicontext-directory-api-openapi.yml
  format: yaml
  label: APIContext Suppliers API
  slug: apicontext-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-directory-api-openapi.yml
authorization_urls:
- https://auth.apimetrics.io/authorize?audience=https://client.apimetrics.io
description: ''
docs: https://docs.apimetrics.io/docs/device-code-authorization-flow
flows:
- authorizationCode
- deviceCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Apicontext Scopes
name_suffix: OAuth Scopes
note: 'APIContext''s OAuth2 is an Auth0 tenant at auth.apimetrics.io fronting the platform API as the audience https://client.apimetrics.io. The platform contract declares only the three OIDC identity scopes on its authorizationCode flow, and NO operation in the 325-operation surface declares a per-operation scope requirement — every operation carries the bare `security: [{OAuth2: []}, {ApiKey: []}]`. Authorization is therefore enforced by project and organization role (Project Roles, Organization Roles, Project Access operations exist in the contract), not by OAuth scope. The wider scopes_supported list below is what the Auth0 discovery document advertises; it is the standard OIDC claim set, not an APIContext permission model.'
overview: 'APIContext publishes 3 OAuth 2.0 scopes via the authorizationCode, deviceCode, and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the APIContext API on a user''s behalf.


  Tokens are issued from https://auth.apimetrics.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: APIContext
provider_slug: apicontext
schemes:
- audience: https://client.apimetrics.io
  flows:
  - authorizationUrl: https://auth.apimetrics.io/authorize?audience=https://client.apimetrics.io
    flow: authorizationCode
    tokenUrl: https://auth.apimetrics.io/oauth/token
  - deviceAuthorizationUrl: https://auth.apimetrics.io/oauth/device/code
    flow: deviceCode
    source: https://docs.apimetrics.io/docs/device-code-authorization-flow
    tokenUrl: https://auth.apimetrics.io/oauth/token
  - flow: clientCredentials
    source: https://github.com/APImetrics/APImetrics-cli (service accounts)
    tokenUrl: https://auth.apimetrics.io/oauth/token
  name: OAuth2
  source: openapi/_original/apicontext-apimetrics-openapi.json
  type: oauth2
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OpenID Connect identity
  flows:
  - authorizationCode
  scope: openid
- description: User profile
  flows:
  - authorizationCode
  scope: profile
- description: User email address
  flows:
  - authorizationCode
  scope: email
slug: apicontext-scopes
source_filename: apicontext-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: openapi/_original/apicontext-apimetrics-openapi.json\ndocs: https://docs.apimetrics.io/docs/device-code-authorization-flow\ndiscovery: https://auth.apimetrics.io/.well-known/openid-configuration\nnote: >-\n  APIContext's OAuth2 is an Auth0 tenant at auth.apimetrics.io fronting the platform API as the\n  audience https://client.apimetrics.io. The platform contract declares only the three OIDC identity\n  scopes on its authorizationCode flow, and NO operation in the 325-operation surface declares a\n  per-operation scope requirement — every operation carries the bare `security: [{OAuth2: []},\n  {ApiKey: []}]`. Authorization is therefore enforced by project and organization role\n  (Project Roles, Organization Roles, Project Access operations exist in the contract), not by OAuth\n  scope. The wider scopes_supported list below is what the Auth0 discovery document advertises; it is\n  the standard OIDC claim set, not an APIContext\
  \ permission model.\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: openapi/_original/apicontext-apimetrics-openapi.json\n  audience: https://client.apimetrics.io\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.apimetrics.io/authorize?audience=https://client.apimetrics.io\n    tokenUrl: https://auth.apimetrics.io/oauth/token\n  - flow: deviceCode\n    tokenUrl: https://auth.apimetrics.io/oauth/token\n    deviceAuthorizationUrl: https://auth.apimetrics.io/oauth/device/code\n    source: https://docs.apimetrics.io/docs/device-code-authorization-flow\n  - flow: clientCredentials\n    tokenUrl: https://auth.apimetrics.io/oauth/token\n    source: https://github.com/APImetrics/APImetrics-cli (service accounts)\nscopes:\n- {scope: openid, description: OpenID Connect identity, flows: [authorizationCode], sources: [openapi/_original/apicontext-apimetrics-openapi.json]}\n- {scope: profile, description: User profile, flows: [authorizationCode], sources: [openapi/_original/apicontext-apimetrics-openapi.json]}\n\
  - {scope: email, description: User email address, flows: [authorizationCode], sources: [openapi/_original/apicontext-apimetrics-openapi.json]}\nidentity_provider_scopes_supported:\n- openid\n- profile\n- offline_access\n- name\n- given_name\n- family_name\n- nickname\n- email\n- email_verified\n- picture\n- created_at\n- identities\n- phone\n- address\noperation_scope_requirements: none\nauthorization_model:\n  style: role-based\n  surfaces:\n  - {tag: Project Roles, operations: 5}\n  - {tag: Organization Roles, operations: 4}\n  - {tag: Project Access, operations: 6}\n  - {tag: Service Accounts, operations: 8}\n  - {tag: API Keys, operations: 3}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/scopes/apicontext-scopes.yml
summary_line: 3 scopes · authorizationCode/deviceCode/clientCredentials
tags:
- API Directory
- API Monitoring
- Agent Skills
- Conformance
- MCP Monitoring
- Observability
- OpenTelemetry
- Performance
- Platform
- SLO
- Synthetic Testing
- Testing
token_urls:
- https://auth.apimetrics.io/oauth/token
---
