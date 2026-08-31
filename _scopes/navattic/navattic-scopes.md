---
api_specs:
- filename: navattic-health-api-openapi.yml
  format: yaml
  label: Navattic Health API
  slug: navattic-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navattic/refs/heads/main/openapi/navattic-health-api-openapi.yml
authorization_urls:
- https://app.navattic.com/api/mcp/oauth/authorize
description: 'Navattic publishes its OAuth scope list twice — machine-readably in the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata, and in prose as a scope/permission table on the MCP docs page, which adds the required workspace role for each. The two lists agree on the seven scopes the docs describe; the metadata advertises four more that the docs do not yet document. Both facts are recorded below.

  '
docs: https://docs.navattic.com/workspace/mcp-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Navattic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Navattic publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Navattic API on a user''s behalf.


  Tokens are issued from https://app.navattic.com/api/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Navattic
provider_slug: navattic
schemes:
- flows:
  - authorizationUrl: https://app.navattic.com/api/mcp/oauth/authorize
    flow: authorizationCode
    pkce: true
    tokenUrl: https://app.navattic.com/api/mcp/oauth/token
  name: NavatticMCPOAuth
  resource: https://app.navattic.com/api/mcp
  resource_name: Navattic MCP Server
  source: https://app.navattic.com/.well-known/oauth-authorization-server
scope_count: 11
scope_names:
- ANALYTICS
- DEMO_BROWSING
- DEMO_BUILDING
- DEMO_MANAGEMENT
- DEMO_PUBLISHING
- PERSONALIZATION
- LAUNCHPAD
- AGENT_DEMOS
- AGENT_ENVIRONMENTS
- WORKSPACE_MANAGEMENT
- NOTIFICATIONS
scopes:
- description: View demo performance, visitor data and account engagement.
  flows:
  - authorizationCode
  scope: ANALYTICS
- description: Browse projects, flows and share links.
  flows:
  - authorizationCode
  scope: DEMO_BROWSING
- description: Create flows; edit steps, buttons, navigation, beacons, media, voiceover and presenter settings.
  flows:
  - authorizationCode
  scope: DEMO_BUILDING
- description: Rename and organize projects; create share links.
  flows:
  - authorizationCode
  scope: DEMO_MANAGEMENT
- description: Publish and archive demos.
  flows:
  - authorizationCode
  scope: DEMO_PUBLISHING
- description: View custom properties and visitor activity.
  flows:
  - authorizationCode
  scope: PERSONALIZATION
- description: Browse and manage Launchpad share links, interest flows and recipient visitor data. Only offered in workspaces with Launchpad enabled, and only shown to users holding the Launchpad app role.
  flows:
  - authorizationCode
  scope: LAUNCHPAD
- description: ''
  flows:
  - authorizationCode
  scope: AGENT_DEMOS
- description: ''
  flows:
  - authorizationCode
  scope: AGENT_ENVIRONMENTS
- description: ''
  flows:
  - authorizationCode
  scope: WORKSPACE_MANAGEMENT
- description: ''
  flows:
  - authorizationCode
  scope: NOTIFICATIONS
slug: navattic-scopes
source_filename: navattic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://app.navattic.com/.well-known/oauth-authorization-server\ndocs: https://docs.navattic.com/workspace/mcp-server\ndescription: >\n  Navattic publishes its OAuth scope list twice — machine-readably in the RFC\n  8414 authorization-server metadata and the RFC 9728 protected-resource\n  metadata, and in prose as a scope/permission table on the MCP docs page, which\n  adds the required workspace role for each. The two lists agree on the seven\n  scopes the docs describe; the metadata advertises four more that the docs do\n  not yet document. Both facts are recorded below.\nschemes:\n  - name: NavatticMCPOAuth\n    source: https://app.navattic.com/.well-known/oauth-authorization-server\n    resource: https://app.navattic.com/api/mcp\n    resource_name: Navattic MCP Server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.navattic.com/api/mcp/oauth/authorize\n        tokenUrl: https://app.navattic.com/api/mcp/oauth/token\n\
  \        pkce: true\nscopes:\n  - scope: ANALYTICS\n    description: View demo performance, visitor data and account engagement.\n    required_role: Viewer or above\n    flows: [authorizationCode]\n    documented: true\n    sources: [oauth-authorization-server, oauth-protected-resource, docs]\n  - scope: DEMO_BROWSING\n    description: Browse projects, flows and share links.\n    required_role: Viewer or above\n    flows: [authorizationCode]\n    documented: true\n    sources: [oauth-authorization-server, oauth-protected-resource, docs]\n  - scope: DEMO_BUILDING\n    description: >\n      Create flows; edit steps, buttons, navigation, beacons, media, voiceover\n      and presenter settings.\n    required_role: Builder or above\n    flows: [authorizationCode]\n    documented: true\n    sources: [oauth-authorization-server, oauth-protected-resource, docs]\n  - scope: DEMO_MANAGEMENT\n    description: Rename and organize projects; create share links.\n    required_role: Builder or above\n\
  \    flows: [authorizationCode]\n    documented: true\n    sources: [oauth-authorization-server, oauth-protected-resource, docs]\n  - scope: DEMO_PUBLISHING\n    description: Publish and archive demos.\n    required_role: Builder or above\n    flows: [authorizationCode]\n    documented: true\n    sources: [oauth-authorization-server, oauth-protected-resource, docs]\n  - scope: PERSONALIZATION\n    description: View custom properties and visitor activity.\n    required_role: Viewer or above\n    flows: [authorizationCode]\n    documented: true\n    sources: [oauth-authorization-server, oauth-protected-resource, docs]\n  - scope: LAUNCHPAD\n    description: >\n      Browse and manage Launchpad share links, interest flows and recipient\n      visitor data. Only offered in workspaces with Launchpad enabled, and only\n      shown to users holding the Launchpad app role.\n    required_role: Viewer or above (Launchpad workspaces only)\n    flows: [authorizationCode]\n    documented: true\n  \
  \  sources: [oauth-authorization-server, oauth-protected-resource, docs]\n  - scope: AGENT_DEMOS\n    description: null\n    required_role: null\n    flows: [authorizationCode]\n    documented: false\n    note: >\n      Advertised in scopes_supported but absent from the docs scope table. Left\n      undescribed rather than guessed; likely relates to the AGENT_DEMO session\n      type that appears in the webhook payload reference.\n    sources: [oauth-authorization-server, oauth-protected-resource]\n  - scope: AGENT_ENVIRONMENTS\n    description: null\n    required_role: null\n    flows: [authorizationCode]\n    documented: false\n    note: Advertised in scopes_supported but absent from the docs scope table.\n    sources: [oauth-authorization-server, oauth-protected-resource]\n  - scope: WORKSPACE_MANAGEMENT\n    description: null\n    required_role: null\n    flows: [authorizationCode]\n    documented: false\n    note: Advertised in scopes_supported but absent from the docs scope table.\n\
  \    sources: [oauth-authorization-server, oauth-protected-resource]\n  - scope: NOTIFICATIONS\n    description: null\n    required_role: null\n    flows: [authorizationCode]\n    documented: false\n    note: Advertised in scopes_supported but absent from the docs scope table.\n    sources: [oauth-authorization-server, oauth-protected-resource]\ncoverage:\n  scopes_advertised: 11\n  scopes_documented: 7\n  scopes_undocumented: 4\nx-evidence:\n  - {url: 'https://app.navattic.com/.well-known/oauth-authorization-server', status: 200}\n  - {url: 'https://app.navattic.com/.well-known/oauth-protected-resource', status: 200}\n  - {url: 'https://docs.navattic.com/workspace/mcp-server.md', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navattic/refs/heads/main/scopes/navattic-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Interactive Demos
- Product Demo
- Sales Enablement
- Marketing
- No-Code
- Webhook
- CRM Integration
- Sales Automation
- MCP
- Agents
- Product Analytics
token_urls:
- https://app.navattic.com/api/mcp/oauth/token
---
