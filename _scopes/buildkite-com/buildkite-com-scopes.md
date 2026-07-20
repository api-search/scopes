---
api_specs:
- filename: buildkite-rest-api-openapi.yml
  format: yaml
  label: Buildkite REST API
  slug: buildkite-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-rest-api-openapi.yml
- filename: buildkite-agent-api-openapi.yml
  format: yaml
  label: Buildkite Agent API
  slug: buildkite-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-agent-api-openapi.yml
authorization_urls: []
description: Buildkite REST API access tokens are Bearer tokens (not OAuth2 authorization-code flows), but they carry a rich, granular scope surface configured per token. This artifact captures the full documented scope list verbatim from the managing-api-tokens reference. GraphQL access is a separate boolean toggle ("Enable GraphQL API access") rather than a scope — it is full-access with no further granular restriction.
docs: https://buildkite.com/docs/apis/managing-api-tokens
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Buildkite Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Buildkite publishes 42 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Buildkite API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Buildkite
provider_slug: buildkite-com
schemes: []
scope_count: 42
scope_names:
- read_agents
- write_agents
- read_clusters
- write_clusters
- read_pipelines
- write_pipelines
- read_pipeline_templates
- write_pipeline_templates
- read_builds
- write_builds
- read_build_logs
- write_build_logs
- read_job_env
- read_artifacts
- write_artifacts
- read_rules
- write_rules
- read_teams
- write_teams
- read_organizations
- write_organizations
- read_organization_settings
- write_organization_settings
- read_organization_repository_connections
- read_notification_services
- write_notification_services
- read_user
- read_audit_events
- read_secrets_details
- write_secrets
- read_suites
- write_suites
- read_test_plan
- write_test_plan
- read_registries
- write_registries
- delete_registries
- read_packages
- write_packages
- delete_packages
- read_portals
- write_portals
scopes:
- description: List and retrieve details of agents.
  flows: []
  scope: read_agents
- description: Stop agents.
  flows: []
  scope: write_agents
- description: List and retrieve details of clusters.
  flows: []
  scope: read_clusters
- description: Create
  flows: []
  scope: write_clusters
- description: List and retrieve details of pipelines.
  flows: []
  scope: read_pipelines
- description: Create
  flows: []
  scope: write_pipelines
- description: List and retrieve details of pipeline templates.
  flows: []
  scope: read_pipeline_templates
- description: Create
  flows: []
  scope: write_pipeline_templates
- description: List and retrieve details of builds.
  flows: []
  scope: read_builds
- description: Create new builds.
  flows: []
  scope: write_builds
- description: Retrieve build logs.
  flows: []
  scope: read_build_logs
- description: Delete build logs.
  flows: []
  scope: write_build_logs
- description: Retrieve job environment variables.
  flows: []
  scope: read_job_env
- description: Retrieve build artifacts.
  flows: []
  scope: read_artifacts
- description: Delete build artifacts.
  flows: []
  scope: write_artifacts
- description: List and retrieve details of rules.
  flows: []
  scope: read_rules
- description: Create or delete rules.
  flows: []
  scope: write_rules
- description: List teams.
  flows: []
  scope: read_teams
- description: Create
  flows: []
  scope: write_teams
- description: List and retrieve details of organizations.
  flows: []
  scope: read_organizations
- description: Update organization settings.
  flows: []
  scope: write_organizations
- description: Read organization's API security and pipeline settings.
  flows: []
  scope: read_organization_settings
- description: Update organization's API security and pipeline settings.
  flows: []
  scope: write_organization_settings
- description: List and retrieve details of connected source control integrations.
  flows: []
  scope: read_organization_repository_connections
- description: List and retrieve notification services.
  flows: []
  scope: read_notification_services
- description: Create
  flows: []
  scope: write_notification_services
- description: Retrieve basic details of the user.
  flows: []
  scope: read_user
- description: List and retrieve details of audit log events (Enterprise plan only).
  flows: []
  scope: read_audit_events
- description: List and retrieve details about secrets.
  flows: []
  scope: read_secrets_details
- description: Create
  flows: []
  scope: write_secrets
- description: Retrieve suite information (Test Engine).
  flows: []
  scope: read_suites
- description: Create suites (Test Engine).
  flows: []
  scope: write_suites
- description: Retrieve test plan information (Test Engine).
  flows: []
  scope: read_test_plan
- description: Create test plan (Test Engine).
  flows: []
  scope: write_test_plan
- description: List and retrieve details of package registries.
  flows: []
  scope: read_registries
- description: Create and update package registries.
  flows: []
  scope: write_registries
- description: Delete package registries.
  flows: []
  scope: delete_registries
- description: List and retrieve details of packages.
  flows: []
  scope: read_packages
- description: Create packages.
  flows: []
  scope: write_packages
- description: Delete packages.
  flows: []
  scope: delete_packages
- description: List and retrieve details of GraphQL Portals.
  flows: []
  scope: read_portals
- description: Create
  flows: []
  scope: write_portals
slug: buildkite-com-scopes
source_filename: buildkite-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/buildkite-rest-api-openapi.yml\ndocs: https://buildkite.com/docs/apis/managing-api-tokens\ndescription: >-\n  Buildkite REST API access tokens are Bearer tokens (not OAuth2 authorization-code\n  flows), but they carry a rich, granular scope surface configured per token. This\n  artifact captures the full documented scope list verbatim from the managing-api-tokens\n  reference. GraphQL access is a separate boolean toggle (\"Enable GraphQL API access\")\n  rather than a scope — it is full-access with no further granular restriction.\nmodel: bearer-token-scoped\ngraphql_access:\n  type: boolean-toggle\n  name: Enable GraphQL API access\n  note: Full-access; does not provide further granular scopes/permission restrictions.\nscopes:\n  - {scope: read_agents, description: List and retrieve details of agents.}\n  - {scope: write_agents, description: Stop agents.}\n  - {scope: read_clusters, description: List and retrieve details\
  \ of clusters.}\n  - {scope: write_clusters, description: Create, update, and delete clusters.}\n  - {scope: read_pipelines, description: List and retrieve details of pipelines.}\n  - {scope: write_pipelines, description: Create, update, and delete pipelines.}\n  - {scope: read_pipeline_templates, description: List and retrieve details of pipeline templates.}\n  - {scope: write_pipeline_templates, description: Create, update, and delete pipeline templates.}\n  - {scope: read_builds, description: List and retrieve details of builds.}\n  - {scope: write_builds, description: Create new builds.}\n  - {scope: read_build_logs, description: Retrieve build logs.}\n  - {scope: write_build_logs, description: Delete build logs.}\n  - {scope: read_job_env, description: Retrieve job environment variables.}\n  - {scope: read_artifacts, description: Retrieve build artifacts.}\n  - {scope: write_artifacts, description: Delete build artifacts.}\n  - {scope: read_rules, description: List and retrieve details\
  \ of rules.}\n  - {scope: write_rules, description: Create or delete rules.}\n  - {scope: read_teams, description: List teams.}\n  - {scope: write_teams, description: Create, update, and delete teams.}\n  - {scope: read_organizations, description: List and retrieve details of organizations.}\n  - {scope: write_organizations, description: Update organization settings.}\n  - {scope: read_organization_settings, description: Read organization's API security and pipeline settings.}\n  - {scope: write_organization_settings, description: Update organization's API security and pipeline settings.}\n  - {scope: read_organization_repository_connections, description: List and retrieve details of connected source control integrations.}\n  - {scope: read_notification_services, description: List and retrieve notification services.}\n  - {scope: write_notification_services, description: Create, update, delete, enable, and disable notification services.}\n  - {scope: read_user, description: Retrieve basic\
  \ details of the user.}\n  - {scope: read_audit_events, description: List and retrieve details of audit log events (Enterprise plan only).}\n  - {scope: read_secrets_details, description: List and retrieve details about secrets.}\n  - {scope: write_secrets, description: Create, update, and delete secrets.}\n  - {scope: read_suites, description: Retrieve suite information (Test Engine).}\n  - {scope: write_suites, description: Create suites (Test Engine).}\n  - {scope: read_test_plan, description: Retrieve test plan information (Test Engine).}\n  - {scope: write_test_plan, description: Create test plan (Test Engine).}\n  - {scope: read_registries, description: List and retrieve details of package registries.}\n  - {scope: write_registries, description: Create and update package registries.}\n  - {scope: delete_registries, description: Delete package registries.}\n  - {scope: read_packages, description: List and retrieve details of packages.}\n  - {scope: write_packages, description: Create\
  \ packages.}\n  - {scope: delete_packages, description: Delete packages.}\n  - {scope: read_portals, description: List and retrieve details of GraphQL Portals.}\n  - {scope: write_portals, description: Create, update, and delete GraphQL Portals.}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/scopes/buildkite-com-scopes.yml
summary_line: 42 scopes
tags:
- CI/CD
- Continuous Integration
- Continuous Delivery
- DevOps
- Pipelines
- Hybrid CI
- Build Automation
- Test Engine
- Package Registries
- Agents
- GraphQL
- REST
- MCP
- Webhooks
token_urls: []
---
