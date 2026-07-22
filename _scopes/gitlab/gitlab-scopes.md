---
api_specs:
- filename: gitlab-api-v4-groups-openapi-original.yml
  format: yaml
  label: GitLab Groups API
  slug: apiv4groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-groups-openapi-original.yml
- filename: gitlab-api-v4-projects-openapi-original.yml
  format: yaml
  label: GitLab Projects API
  slug: apiv4projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-projects-openapi-original.yml
- filename: gitlab-api-v4-admin-openapi-original.yml
  format: yaml
  label: GitLab Admin API
  slug: apiv4admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-admin-openapi-original.yml
- filename: gitlab-api-v4-applications-openapi-original.yml
  format: yaml
  label: GitLab Applications API
  slug: apiv4applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-applications-openapi-original.yml
- filename: gitlab-api-v4-avatar-openapi-original.yml
  format: yaml
  label: GitLab Avatar API
  slug: apiv4avatar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-avatar-openapi-original.yml
- filename: gitlab-api-v4-broadcast-messages-openapi-original.yml
  format: yaml
  label: GitLab Broadcast Messages API
  slug: apiv4broadcast-messages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-broadcast-messages-openapi-original.yml
- filename: gitlab-api-v4-bulk-imports-openapi-original.yml
  format: yaml
  label: GitLab Bulk Imports API
  slug: apiv4bulk-imports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-bulk-imports-openapi-original.yml
- filename: gitlab-api-v4-application-openapi-original.yml
  format: yaml
  label: GitLab Application Settings API
  slug: apiv4application
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-application-openapi-original.yml
- filename: gitlab-api-v4-metadata-openapi-original.yml
  format: yaml
  label: GitLab Metadata API
  slug: apiv4metadata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-metadata-openapi-original.yml
- filename: gitlab-api-v4-version-openapi-original.yml
  format: yaml
  label: GitLab Version API
  slug: apiv4version
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-version-openapi-original.yml
- filename: gitlab-openapi-original.yml
  format: yaml
  label: GitLab REST API
  slug: gitlab-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-openapi-original.yml
- filename: gitlab-oauth2-openapi.yml
  format: yaml
  label: GitLab OAuth 2.0 API
  slug: gitlab-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-oauth2-openapi.yml
- filename: gitlab-webhooks-openapi.yml
  format: yaml
  label: GitLab Webhooks
  slug: gitlab-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-webhooks-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.gitlab.com/integration/oauth_provider/
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Gitlab Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GitLab publishes 25 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the GitLab API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GitLab
provider_slug: gitlab
schemes:
- authorizationUrl: https://gitlab.com/oauth/authorize
  code_challenge_methods:
  - plain
  - S256
  device_authorization_endpoint: https://gitlab.com/oauth/authorize_device
  flows:
  - authorizationCode
  - clientCredentials
  - deviceCode
  grant_types:
  - authorization_code
  - client_credentials
  - device_code
  - refresh_token
  issuer: https://gitlab.com
  name: OAuth2
  registration_endpoint: https://gitlab.com/oauth/register
  tokenUrl: https://gitlab.com/oauth/token
scope_count: 25
scope_names:
- api
- read_api
- read_user
- create_runner
- manage_runner
- k8s_proxy
- self_rotate
- mcp
- mcp_orbit
- read_repository
- write_repository
- read_registry
- write_registry
- read_virtual_registry
- write_virtual_registry
- read_observability
- write_observability
- ai_features
- ai_workflows
- sudo
- admin_mode
- read_service_ping
- openid
- profile
- email
scopes:
- description: Complete read/write access to the API, including all groups and projects, the container registry, the dependency proxy, and the package registry.
  flows: []
  scope: api
- description: Read access to the API, including all groups and projects, the container registry, and the package registry.
  flows: []
  scope: read_api
- description: Read-only access to the authenticated user's profile through the /user API, including username, public email, and full name.
  flows: []
  scope: read_user
- description: Grants create access to the runners.
  flows: []
  scope: create_runner
- description: Grants access to manage the runners.
  flows: []
  scope: manage_runner
- description: Perform Kubernetes API calls using the agent for Kubernetes.
  flows: []
  scope: k8s_proxy
- description: Rotate the access token used to make the request. Documented via the live discovery metadata; not enumerated on the OAuth provider scopes page.
  flows: []
  scope: self_rotate
- description: Access to the GitLab Model Context Protocol (MCP) server at /api/v4/mcp for AI agents.
  flows: []
  scope: mcp
- description: Scope for the GitLab Orbit agent context surface (from live discovery metadata).
  flows: []
  scope: mcp_orbit
- description: Read-only access to repositories on private projects using Git-over-HTTP or the Repository Files API.
  flows: []
  scope: read_repository
- description: Read-write access to repositories on private projects using Git-over-HTTP.
  flows: []
  scope: write_repository
- description: Read-only access to container registry images on private projects.
  flows: []
  scope: read_registry
- description: Write access to container registry images on private projects.
  flows: []
  scope: write_registry
- description: Read-only access to container images through the dependency proxy.
  flows: []
  scope: read_virtual_registry
- description: Read, write, and delete access to container images through the dependency proxy.
  flows: []
  scope: write_virtual_registry
- description: Read-only access to GitLab Observability.
  flows: []
  scope: read_observability
- description: Write access to GitLab Observability.
  flows: []
  scope: write_observability
- description: Access to GitLab Duo related API endpoints.
  flows: []
  scope: ai_features
- description: Access to AI workflow endpoints (from live discovery metadata).
  flows: []
  scope: ai_workflows
- description: Perform API actions as any user in the system (available only for administrators).
  flows: []
  scope: sudo
- description: Perform API actions as an administrator when Admin Mode is enabled.
  flows: []
  scope: admin_mode
- description: Download Service Ping payloads through the API when authenticated as an administrator.
  flows: []
  scope: read_service_ping
- description: Authenticate with GitLab using OpenID Connect; also grants read-only access to the user's profile and group memberships.
  flows: []
  scope: openid
- description: Read-only access to the user's profile data using OpenID Connect.
  flows: []
  scope: profile
- description: Read-only access to the user's primary email address using OpenID Connect.
  flows: []
  scope: email
slug: gitlab-scopes
source_filename: gitlab-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://gitlab.com/.well-known/oauth-authorization-server\ndocs: https://docs.gitlab.com/integration/oauth_provider/\nschemes:\n- name: OAuth2\n  issuer: https://gitlab.com\n  authorizationUrl: https://gitlab.com/oauth/authorize\n  tokenUrl: https://gitlab.com/oauth/token\n  device_authorization_endpoint: https://gitlab.com/oauth/authorize_device\n  registration_endpoint: https://gitlab.com/oauth/register\n  grant_types: [authorization_code, client_credentials, device_code, refresh_token]\n  code_challenge_methods: [plain, S256]\n  flows: [authorizationCode, clientCredentials, deviceCode]\nscopes:\n- scope: api\n  description: Complete read/write access to the API, including all groups and projects, the container registry, the dependency proxy, and the package registry.\n- scope: read_api\n  description: Read access to the API, including all groups and projects, the container registry, and the package registry.\n- scope: read_user\n\
  \  description: Read-only access to the authenticated user's profile through the /user API, including username, public email, and full name.\n- scope: create_runner\n  description: Grants create access to the runners.\n- scope: manage_runner\n  description: Grants access to manage the runners.\n- scope: k8s_proxy\n  description: Perform Kubernetes API calls using the agent for Kubernetes.\n- scope: self_rotate\n  description: Rotate the access token used to make the request. Documented via the live discovery metadata; not enumerated on the OAuth provider scopes page.\n- scope: mcp\n  description: Access to the GitLab Model Context Protocol (MCP) server at /api/v4/mcp for AI agents.\n- scope: mcp_orbit\n  description: Scope for the GitLab Orbit agent context surface (from live discovery metadata).\n- scope: read_repository\n  description: Read-only access to repositories on private projects using Git-over-HTTP or the Repository Files API.\n- scope: write_repository\n  description: Read-write\
  \ access to repositories on private projects using Git-over-HTTP.\n- scope: read_registry\n  description: Read-only access to container registry images on private projects.\n- scope: write_registry\n  description: Write access to container registry images on private projects.\n- scope: read_virtual_registry\n  description: Read-only access to container images through the dependency proxy.\n- scope: write_virtual_registry\n  description: Read, write, and delete access to container images through the dependency proxy.\n- scope: read_observability\n  description: Read-only access to GitLab Observability.\n- scope: write_observability\n  description: Write access to GitLab Observability.\n- scope: ai_features\n  description: Access to GitLab Duo related API endpoints.\n- scope: ai_workflows\n  description: Access to AI workflow endpoints (from live discovery metadata).\n- scope: sudo\n  description: Perform API actions as any user in the system (available only for administrators).\n- scope:\
  \ admin_mode\n  description: Perform API actions as an administrator when Admin Mode is enabled.\n- scope: read_service_ping\n  description: Download Service Ping payloads through the API when authenticated as an administrator.\n- scope: openid\n  description: Authenticate with GitLab using OpenID Connect; also grants read-only access to the user's profile and group memberships.\n- scope: profile\n  description: Read-only access to the user's profile data using OpenID Connect.\n- scope: email\n  description: Read-only access to the user's primary email address using OpenID Connect.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/scopes/gitlab-scopes.yml
summary_line: 25 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Code
- Platform
- Software Development
- Source Control
token_urls: []
---
