---
api_specs:
- filename: kernel-api-keys-api-openapi.yml
  format: yaml
  label: Kernel API Keys API
  slug: kernel-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-api-keys-api-openapi.yml
- filename: kernel-apps-api-openapi.yml
  format: yaml
  label: Kernel Apps API
  slug: kernel-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-apps-api-openapi.yml
- filename: kernel-audit-logs-api-openapi.yml
  format: yaml
  label: Kernel Audit Logs API
  slug: kernel-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-audit-logs-api-openapi.yml
- filename: kernel-browser-computer-controls-api-openapi.yml
  format: yaml
  label: Kernel Browser Computer Controls API
  slug: kernel-browser-computer-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-browser-computer-controls-api-openapi.yml
- filename: kernel-browser-filesystem-api-openapi.yml
  format: yaml
  label: Kernel Browser Filesystem API
  slug: kernel-browser-filesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-browser-filesystem-api-openapi.yml
- filename: kernel-browser-logs-api-openapi.yml
  format: yaml
  label: Kernel Browser Logs API
  slug: kernel-browser-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-browser-logs-api-openapi.yml
- filename: kernel-browser-playwright-api-openapi.yml
  format: yaml
  label: Kernel Browser Playwright API
  slug: kernel-browser-playwright-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-browser-playwright-api-openapi.yml
- filename: kernel-browser-pools-api-openapi.yml
  format: yaml
  label: Kernel Browser Pools API
  slug: kernel-browser-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-browser-pools-api-openapi.yml
- filename: kernel-browser-processes-api-openapi.yml
  format: yaml
  label: Kernel Browser Processes API
  slug: kernel-browser-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-browser-processes-api-openapi.yml
- filename: kernel-browser-replays-api-openapi.yml
  format: yaml
  label: Kernel Browser Replays API
  slug: kernel-browser-replays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-browser-replays-api-openapi.yml
- filename: kernel-browser-telemetry-api-openapi.yml
  format: yaml
  label: Kernel Browser Telemetry API
  slug: kernel-browser-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-browser-telemetry-api-openapi.yml
- filename: kernel-browsers-api-openapi.yml
  format: yaml
  label: Kernel Browsers API
  slug: kernel-browsers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-browsers-api-openapi.yml
- filename: kernel-credential-providers-api-openapi.yml
  format: yaml
  label: Kernel Credential Providers API
  slug: kernel-credential-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-credential-providers-api-openapi.yml
- filename: kernel-credentials-api-openapi.yml
  format: yaml
  label: Kernel Credentials API
  slug: kernel-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-credentials-api-openapi.yml
- filename: kernel-deployments-api-openapi.yml
  format: yaml
  label: Kernel Deployments API
  slug: kernel-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-deployments-api-openapi.yml
- filename: kernel-extensions-api-openapi.yml
  format: yaml
  label: Kernel Extensions API
  slug: kernel-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-extensions-api-openapi.yml
- filename: kernel-invocations-api-openapi.yml
  format: yaml
  label: Kernel Invocations API
  slug: kernel-invocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-invocations-api-openapi.yml
- filename: kernel-managed-auth-api-openapi.yml
  format: yaml
  label: Kernel Managed Auth API
  slug: kernel-managed-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-managed-auth-api-openapi.yml
- filename: kernel-organization-api-openapi.yml
  format: yaml
  label: Kernel Organization API
  slug: kernel-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-organization-api-openapi.yml
- filename: kernel-profiles-api-openapi.yml
  format: yaml
  label: Kernel Profiles API
  slug: kernel-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-profiles-api-openapi.yml
- filename: kernel-projects-api-openapi.yml
  format: yaml
  label: Kernel Projects API
  slug: kernel-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-projects-api-openapi.yml
- filename: kernel-proxies-api-openapi.yml
  format: yaml
  label: Kernel Proxies API
  slug: kernel-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-proxies-api-openapi.yml
authorization_urls: []
description: ''
docs: https://kernel.sh/docs/reference/mcp-server/authentication.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Kernel Scopes
name_suffix: OAuth Scopes
note: The Kernel REST API OpenAPI declares a single bearer (API key) scheme without oauth2 flows, but the RFC 8414 authorization-server metadata advertises OAuth 2.1 (used by the hosted MCP server, with dynamic client registration) and two coarse scopes. Scopes are captured from the well-known document verbatim.
overview: 'Kernel publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kernel API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kernel
provider_slug: kernel
schemes:
- bearer_methods_supported:
  - header
  dynamic_client_registration: true
  flows:
  - flow: authorizationCode
    note: OAuth 2.1 with dynamic client registration; used by the hosted MCP server.
  issuer: https://api.onkernel.com/
  name: OAuth2.1
  source: https://api.onkernel.com/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- api.read
- api.write
scopes:
- description: Read access to Kernel API resources.
  flows: []
  scope: api.read
- description: Write access to Kernel API resources.
  flows: []
  scope: api.write
slug: kernel-scopes
source_filename: kernel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.onkernel.com/.well-known/oauth-authorization-server\ndocs: https://kernel.sh/docs/reference/mcp-server/authentication.md\nnote: >-\n  The Kernel REST API OpenAPI declares a single bearer (API key) scheme without\n  oauth2 flows, but the RFC 8414 authorization-server metadata advertises OAuth 2.1\n  (used by the hosted MCP server, with dynamic client registration) and two coarse\n  scopes. Scopes are captured from the well-known document verbatim.\nschemes:\n  - name: OAuth2.1\n    source: https://api.onkernel.com/.well-known/oauth-authorization-server\n    issuer: https://api.onkernel.com/\n    bearer_methods_supported: [header]\n    dynamic_client_registration: true\n    flows:\n      - flow: authorizationCode\n        note: OAuth 2.1 with dynamic client registration; used by the hosted MCP server.\nscopes:\n  - scope: api.read\n    description: Read access to Kernel API resources.\n    sources: [https://api.onkernel.com/.well-known/oauth-authorization-server]\n\
  \  - scope: api.write\n    description: Write access to Kernel API resources.\n    sources: [https://api.onkernel.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/scopes/kernel-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Browser Automation
- Web Agents
- Browser Infrastructure
- AI Agents
- Playwright
- Cloud Browsers
- Computer Use
- MCP
- Managed Auth
token_urls: []
---
