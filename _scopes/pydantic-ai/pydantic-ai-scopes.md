---
api_specs:
- filename: pydantic-ai-discovery-openapi.yml
  format: yaml
  label: PydanticAI Agent Framework
  slug: pydantic-ai-agent-framework
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-discovery-openapi.yml
- filename: pydantic-ai-logfire-openapi.yml
  format: yaml
  label: Pydantic Logfire
  slug: pydantic-logfire
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-logfire-openapi.yml
authorization_urls:
- api/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Pydantic Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PydanticAI publishes 38 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PydanticAI API on a user''s behalf.


  Tokens are issued from /api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PydanticAI
provider_slug: pydantic-ai
schemes:
- flows:
  - authorizationUrl: api/oauth/authorize
    flow: authorizationCode
    tokenUrl: /api/oauth/token
  name: OAuth2AuthorizationCodeBearer
  source: openapi/pydantic-ai-logfire-openapi.yml
scope_count: 38
scope_names:
- instance:admin
- instance:billing
- organization:admin
- organization:auditlog
- organization:create_api_key
- organization:create_project
- organization:payment
- organization:read
- organization:read_api_key
- organization:read_channel
- organization:read_invitation
- organization:read_member
- organization:read_trust_policy
- organization:scim
- organization:write
- organization:write_api_key
- organization:write_channel
- organization:write_invitation
- organization:write_member
- organization:write_trust_policy
- project:gateway_proxy
- project:read
- project:read_alert
- project:read_api_key
- project:read_dashboard
- project:read_datasets
- project:read_external_variables
- project:read_otlp
- project:read_token
- project:read_variables
- project:write
- project:write_alert
- project:write_api_key
- project:write_dashboard
- project:write_datasets
- project:write_otlp
- project:write_token
- project:write_variables
scopes:
- description: Platform admin access to manage the whole self-hosted instance
  flows:
  - authorizationCode
  scope: instance:admin
- description: Read billing and usage data across the whole self-hosted instance
  flows:
  - authorizationCode
  scope: instance:billing
- description: Platform admin access to manage organizations across the instance (self-hosted only)
  flows:
  - authorizationCode
  scope: organization:admin
- description: Read audit logs for the organization
  flows:
  - authorizationCode
  scope: organization:auditlog
- description: Create new API keys for the organization
  flows:
  - authorizationCode
  scope: organization:create_api_key
- description: Ability to create projects within the organization
  flows:
  - authorizationCode
  scope: organization:create_project
- description: Read billing usage data for the organization
  flows:
  - authorizationCode
  scope: organization:payment
- description: Read access to organizations
  flows:
  - authorizationCode
  scope: organization:read
- description: Read API keys across the organization
  flows:
  - authorizationCode
  scope: organization:read_api_key
- description: Read notification channels across the organization
  flows:
  - authorizationCode
  scope: organization:read_channel
- description: Read organization invitations
  flows:
  - authorizationCode
  scope: organization:read_invitation
- description: Read organization members and roles
  flows:
  - authorizationCode
  scope: organization:read_member
- description: Read OIDC trust policies and their token exchange history
  flows:
  - authorizationCode
  scope: organization:read_trust_policy
- description: SCIM access to organizations
  flows:
  - authorizationCode
  scope: organization:scim
- description: Write access to organizations
  flows:
  - authorizationCode
  scope: organization:write
- description: Edit or revoke existing API keys across the organization
  flows:
  - authorizationCode
  scope: organization:write_api_key
- description: Create or modify notification channels across the organization
  flows:
  - authorizationCode
  scope: organization:write_channel
- description: Create organization invitations
  flows:
  - authorizationCode
  scope: organization:write_invitation
- description: Modify organization member roles and membership
  flows:
  - authorizationCode
  scope: organization:write_member
- description: Create, modify, or delete OIDC trust policies and revoke issued workload tokens
  flows:
  - authorizationCode
  scope: organization:write_trust_policy
- description: Proxy AI model requests through the project AI Gateway
  flows:
  - authorizationCode
  scope: project:gateway_proxy
- description: Read access to projects
  flows:
  - authorizationCode
  scope: project:read
- description: Read alerts within a project
  flows:
  - authorizationCode
  scope: project:read_alert
- description: Read API keys within a project
  flows:
  - authorizationCode
  scope: project:read_api_key
- description: Read dashboards within a project
  flows:
  - authorizationCode
  scope: project:read_dashboard
- description: Read datasets within a project
  flows:
  - authorizationCode
  scope: project:read_datasets
- description: Read external managed variables within a project via OFREP
  flows:
  - authorizationCode
  scope: project:read_external_variables
- description: Query trace data submitted to the project via OTLP
  flows:
  - authorizationCode
  scope: project:read_otlp
- description: Create read tokens
  flows:
  - authorizationCode
  scope: project:read_token
- description: Read managed variables and prompts within a project
  flows:
  - authorizationCode
  scope: project:read_variables
- description: Write access to projects
  flows:
  - authorizationCode
  scope: project:write
- description: Create or modify alerts within a project
  flows:
  - authorizationCode
  scope: project:write_alert
- description: Create, edit, or revoke API keys within a project
  flows:
  - authorizationCode
  scope: project:write_api_key
- description: Create or modify dashboards within a project
  flows:
  - authorizationCode
  scope: project:write_dashboard
- description: Create or modify datasets within a project
  flows:
  - authorizationCode
  scope: project:write_datasets
- description: Send OTLP traces, logs, and metrics to the project
  flows:
  - authorizationCode
  scope: project:write_otlp
- description: Create write tokens
  flows:
  - authorizationCode
  scope: project:write_token
- description: Create or modify managed variables and prompts within a project
  flows:
  - authorizationCode
  scope: project:write_variables
slug: pydantic-ai-scopes
source_filename: pydantic-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pydantic-ai-logfire-openapi.yml\nschemes:\n- name: OAuth2AuthorizationCodeBearer\n  source: openapi/pydantic-ai-logfire-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: api/oauth/authorize\n    tokenUrl: /api/oauth/token\nscopes:\n- scope: instance:admin\n  description: Platform admin access to manage the whole self-hosted instance\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: instance:billing\n  description: Read billing and usage data across the whole self-hosted instance\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:admin\n  description: Platform admin access to manage organizations across the instance (self-hosted\n    only)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:auditlog\n  description: Read audit\
  \ logs for the organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:create_api_key\n  description: Create new API keys for the organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:create_project\n  description: Ability to create projects within the organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:payment\n  description: Read billing usage data for the organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:read\n  description: Read access to organizations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:read_api_key\n  description: Read API keys across the organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n\
  - scope: organization:read_channel\n  description: Read notification channels across the organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:read_invitation\n  description: Read organization invitations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:read_member\n  description: Read organization members and roles\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:read_trust_policy\n  description: Read OIDC trust policies and their token exchange history\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:scim\n  description: SCIM access to organizations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:write\n  description: Write access to organizations\n  flows:\n \
  \ - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:write_api_key\n  description: Edit or revoke existing API keys across the organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:write_channel\n  description: Create or modify notification channels across the organization\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:write_invitation\n  description: Create organization invitations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:write_member\n  description: Modify organization member roles and membership\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: organization:write_trust_policy\n  description: Create, modify, or delete OIDC trust policies and revoke issued workload tokens\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:gateway_proxy\n  description: Proxy AI model requests through the project AI Gateway\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:read\n  description: Read access to projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:read_alert\n  description: Read alerts within a project\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:read_api_key\n  description: Read API keys within a project\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:read_dashboard\n  description: Read dashboards within a project\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:read_datasets\n  description: Read datasets within a\
  \ project\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:read_external_variables\n  description: Read external managed variables within a project via OFREP\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:read_otlp\n  description: Query trace data submitted to the project via OTLP\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:read_token\n  description: Create read tokens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:read_variables\n  description: Read managed variables and prompts within a project\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:write\n  description: Write access to projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope:\
  \ project:write_alert\n  description: Create or modify alerts within a project\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:write_api_key\n  description: Create, edit, or revoke API keys within a project\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:write_dashboard\n  description: Create or modify dashboards within a project\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:write_datasets\n  description: Create or modify datasets within a project\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:write_otlp\n  description: Send OTLP traces, logs, and metrics to the project\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:write_token\n  description: Create write tokens\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n- scope: project:write_variables\n  description: Create or modify managed variables and prompts within a project\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pydantic-ai-logfire-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/scopes/pydantic-ai-scopes.yml
summary_line: 38 scopes · authorizationCode
tags:
- AI
- Agents
- Python
- LLM
- Type Safety
- Structured Outputs
- Dependency Injection
- OpenAI
- Anthropic
- Gemini
- Observability
- Framework
token_urls:
- /api/oauth/token
---
