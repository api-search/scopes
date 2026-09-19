---
authorization_urls:
- https://auth.{global.domain}/realms/boltmcp/protocol/openid-connect/auth
description: ''
docs: https://install.boltmcp.io/docs/configuration-reference
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Boltmcp Scopes
name_suffix: OAuth Scopes
note: BoltMCP publishes no OpenAPI, so derive-oauth-scopes.py had nothing to read. These are the platform-owned OAuth realm resources the chart's `keycloak-reconcile` hook creates and re-applies on every install and upgrade, named verbatim in the configuration reference. They are the only authorization primitives BoltMCP publishes; everything else is defined by the customer in their own identity provider.
overview: 'BoltMCP publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BoltMCP API on a user''s behalf.


  Tokens are issued from https://auth.{global.domain}/realms/boltmcp/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BoltMCP
provider_slug: boltmcp
schemes:
- flows:
  - authorizationUrl: https://auth.{global.domain}/realms/boltmcp/protocol/openid-connect/auth
    flow: authorizationCode
    note: Standard Keycloak realm endpoints implied by the published issuer. Recorded as templates; not probed, because no BoltMCP-operated realm is publicly reachable.
    tokenUrl: https://auth.{global.domain}/realms/boltmcp/protocol/openid-connect/token
  issuer_template: https://auth.{global.domain}/realms/boltmcp
  name: oidc
  provider: keycloak
  realm: boltmcp
scope_count: 1
scope_names:
- boltmcp:rest-api:access
scopes:
- description: Platform-owned client scope granting access to the BoltMCP internal REST API. Created and reconciled by the chart's keycloak-reconcile hook Job.
  flows:
  - authorizationCode
  scope: boltmcp:rest-api:access
slug: boltmcp-scopes
source_filename: boltmcp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://install.boltmcp.io/docs/configuration-reference\ndocs: https://install.boltmcp.io/docs/configuration-reference\nnote: >-\n  BoltMCP publishes no OpenAPI, so derive-oauth-scopes.py had nothing to read. These are the\n  platform-owned OAuth realm resources the chart's `keycloak-reconcile` hook creates and re-applies\n  on every install and upgrade, named verbatim in the configuration reference. They are the only\n  authorization primitives BoltMCP publishes; everything else is defined by the customer in their own\n  identity provider.\nschemes:\n- name: oidc\n  provider: keycloak\n  realm: boltmcp\n  issuer_template: https://auth.{global.domain}/realms/boltmcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.{global.domain}/realms/boltmcp/protocol/openid-connect/auth\n    tokenUrl: https://auth.{global.domain}/realms/boltmcp/protocol/openid-connect/token\n    note: >-\n      Standard Keycloak\
  \ realm endpoints implied by the published issuer. Recorded as templates; not\n      probed, because no BoltMCP-operated realm is publicly reachable.\nscopes:\n- scope: boltmcp:rest-api:access\n  description: >-\n    Platform-owned client scope granting access to the BoltMCP internal REST API. Created and\n    reconciled by the chart's keycloak-reconcile hook Job.\n  flows: [authorizationCode]\n  sources: [https://install.boltmcp.io/docs/configuration-reference]\nroles:\n- role: mcp:manage\n  description: >-\n    Platform-owned realm role for managing MCP servers. Created and reconciled by the chart's\n    keycloak-reconcile hook Job alongside the OIDC clients and the rest-api access scope.\n  sources: [https://install.boltmcp.io/docs/configuration-reference]\ngaps:\n- No published scope/permission reference page exists. The dashboard documentation that covers\n  managing authorization ships inside the deployment, behind SSO, and is not on the public web.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltmcp/refs/heads/main/scopes/boltmcp-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- MCP
- Agents
- Artificial Intelligence
- Kubernetes
- Self-Hosted
- Enterprise
- Identity
- Developer Tools
token_urls:
- https://auth.{global.domain}/realms/boltmcp/protocol/openid-connect/token
---
