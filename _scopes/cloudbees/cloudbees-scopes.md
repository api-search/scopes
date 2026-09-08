---
api_specs:
- filename: cloudbees-unify-openapi.yml
  format: yaml
  label: CloudBees Unify Platform API
  slug: unify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-unify-openapi.yml
- filename: cloudbees-computer-api-openapi.yml
  format: yaml
  label: CloudBees Computer API
  slug: cloudbees-computer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-computer-api-openapi.yml
- filename: cloudbees-createitem-api-openapi.yml
  format: yaml
  label: CloudBees CreateItem API
  slug: cloudbees-createitem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-createitem-api-openapi.yml
- filename: cloudbees-job-api-openapi.yml
  format: yaml
  label: CloudBees Job API
  slug: cloudbees-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-job-api-openapi.yml
- filename: cloudbees-json-api-openapi.yml
  format: yaml
  label: CloudBees Json API
  slug: cloudbees-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-json-api-openapi.yml
- filename: cloudbees-python-api-openapi.yml
  format: yaml
  label: CloudBees Python API
  slug: cloudbees-python-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-python-api-openapi.yml
- filename: cloudbees-queue-api-openapi.yml
  format: yaml
  label: CloudBees Queue API
  slug: cloudbees-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-queue-api-openapi.yml
- filename: cloudbees-xml-api-openapi.yml
  format: yaml
  label: CloudBees Xml API
  slug: cloudbees-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-xml-api-openapi.yml
authorization_urls:
- https://id.cloudbees.io/realms/cloudbees/protocol/openid-connect/auth
description: ''
docs: https://docs.cloudbees.com/docs/cloudbees-unify/latest/unify-ai/how-to-guides/secure-your-mcp-connection
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cloudbees Scopes
name_suffix: OAuth Scopes
note: The CloudBees Unify REST API does not use OAuth — both published specifications declare a single http/bearer scheme carrying a personal access token, with no oauth2 securityScheme and therefore no scope surface. The OAuth scopes below belong to the CloudBees Unify MCP server, which IS an OAuth protected resource. This file exists for that surface only; do not read it as REST API scopes.
overview: 'CloudBees publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CloudBees API on a user''s behalf.


  Tokens are issued from https://id.cloudbees.io/realms/cloudbees/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CloudBees
provider_slug: cloudbees
schemes:
- authorization_servers:
  - https://id.cloudbees.io/realms/cloudbees
  bearer_methods_supported:
  - header
  flows:
  - authorizationUrl: https://id.cloudbees.io/realms/cloudbees/protocol/openid-connect/auth
    flow: authorizationCode
    source: well-known/cloudbees-id-openid-configuration.json
    tokenUrl: https://id.cloudbees.io/realms/cloudbees/protocol/openid-connect/token
  name: CloudBees Unify MCP Server
  resource: https://mcp.cloudbees.io/v1/mcp
  source: well-known/cloudbees-mcp-oauth-protected-resource.json
scope_count: 4
scope_names:
- openid
- profile
- email
- mcp:unify:connect
scopes:
- description: OIDC authentication of the connecting user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC profile claims for the connecting user.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC email claim for the connecting user.
  flows:
  - authorizationCode
  scope: email
- description: Authorises an MCP client to connect to the CloudBees Unify MCP server. Named in the WWW-Authenticate challenge returned by an unauthenticated POST to https://mcp.cloudbees.io/v1/mcp.
  flows:
  - authorizationCode
  scope: mcp:unify:connect
slug: cloudbees-scopes
source_filename: cloudbees-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://mcp.cloudbees.io/.well-known/oauth-protected-resource and\n  https://id.cloudbees.io/realms/cloudbees/.well-known/openid-configuration\ndocs: https://docs.cloudbees.com/docs/cloudbees-unify/latest/unify-ai/how-to-guides/secure-your-mcp-connection\nnote: >-\n  The CloudBees Unify REST API does not use OAuth — both published specifications declare a single\n  http/bearer scheme carrying a personal access token, with no oauth2 securityScheme and therefore no scope\n  surface. The OAuth scopes below belong to the CloudBees Unify MCP server, which IS an OAuth protected\n  resource. This file exists for that surface only; do not read it as REST API scopes.\nschemes:\n  - name: CloudBees Unify MCP Server\n    resource: https://mcp.cloudbees.io/v1/mcp\n    source: well-known/cloudbees-mcp-oauth-protected-resource.json\n    bearer_methods_supported: [header]\n    authorization_servers:\n      - https://id.cloudbees.io/realms/cloudbees\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://id.cloudbees.io/realms/cloudbees/protocol/openid-connect/auth\n        tokenUrl: https://id.cloudbees.io/realms/cloudbees/protocol/openid-connect/token\n        source: well-known/cloudbees-id-openid-configuration.json\nscopes:\n  - scope: openid\n    description: OIDC authentication of the connecting user.\n    flows: [authorizationCode]\n    sources: [well-known/cloudbees-mcp-oauth-protected-resource.json]\n  - scope: profile\n    description: Standard OIDC profile claims for the connecting user.\n    flows: [authorizationCode]\n    sources: [well-known/cloudbees-mcp-oauth-protected-resource.json]\n  - scope: email\n    description: Standard OIDC email claim for the connecting user.\n    flows: [authorizationCode]\n    sources: [well-known/cloudbees-mcp-oauth-protected-resource.json]\n  - scope: mcp:unify:connect\n    description: >-\n      Authorises an MCP client to connect to the CloudBees Unify MCP server.\
  \ Named in the WWW-Authenticate\n      challenge returned by an unauthenticated POST to https://mcp.cloudbees.io/v1/mcp.\n    flows: [authorizationCode]\n    sources: [well-known/cloudbees-mcp-oauth-protected-resource.json]\nauthorization_model:\n  note: >-\n    There is exactly one MCP scope and it is binary — connect or do not connect. Tool-level authority is not\n    expressed in scopes; the agent inherits the full permission set of the signed-in CloudBees Unify user and\n    is constrained by CloudBees Unify RBAC on the server side. An operator scoping an agent down therefore\n    has to do it with a dedicated Unify user and RBAC role, not with an OAuth scope. The X-MCP-Toolsets\n    header narrows which tools are SERVED, but it is a client-set header, not an authorisation boundary.\n  rbac_reference: >-\n    RBAC roles, permissions and authorizations are reachable through the MCP tools (rbac_roles_list,\n    rbac_permissions_list, rbac_authorization_create) but are not published in\
  \ the REST contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/scopes/cloudbees-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- CI/CD
- Continuous Delivery
- Continuous Integration
- DevOps
- Feature Flags
- Feature Management
- Jenkins
- Release Orchestration
- Software Delivery
token_urls:
- https://id.cloudbees.io/realms/cloudbees/protocol/openid-connect/token
---
