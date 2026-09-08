---
api_specs:
- filename: 7signalsolutions-openapi.json
  format: json
  label: 7SIGNAL Platform API (Gateway v2)
  slug: 7signal-platform-api-gateway-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7signalsolutions/refs/heads/main/openapi/7signalsolutions-openapi.json
authorization_urls:
- https://mcp-v2.7signal.com/authorize
description: ''
docs: https://github.com/7Signal/API-Examples/blob/develop/docs/01-authentication.md
flows:
- clientCredentials
- authorization_code
kind: oauth-scopes
layout: scope
method: searched
name: 7Signalsolutions Scopes
name_suffix: OAuth Scopes
note: 'The REST gateway''s OpenAPI declares an oauth2 clientCredentials scheme whose scopes map is empty; only three of the 215 operations carry an explicit `read` scope requirement, and the remaining 211 declare `oauth2: []`. The published scope vocabulary lives on the MCP surface instead, in the RFC 9728 protected-resource document. 7SIGNAL''s auth docs show a token response carrying `"scope": "read:resources write:resources"` as an illustrative example, not an enumerated reference, so those two strings are NOT recorded here as real scopes.'
overview: '7SIGNAL publishes 10 OAuth 2.0 scopes via the clientCredentials and authorization_code flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the 7SIGNAL API on a user''s behalf.


  Tokens are issued from https://api-v2.7signal.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 7SIGNAL
provider_slug: 7signalsolutions
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api-v2.7signal.com/oauth2/token
  name: oauth2
  source: openapi/7signalsolutions-openapi.json
  surface: 7SIGNAL Platform API (Gateway v2)
- flows:
  - authorizationUrl: https://mcp-v2.7signal.com/authorize
    flow: authorization_code
    tokenUrl: https://mcp-v2.7signal.com/token
  name: mcp_oauth
  source: https://mcp-v2.7signal.com/.well-known/oauth-authorization-server
  surface: 7SIGNAL MCP Server
scope_count: 10
scope_names:
- read
- openid
- profile
- email
- offline_access
- https://login.7signal.com/scopes/user.read
- https://login.7signal.com/scopes/organization.admin
- sap:user.read
- sap:user.config
- mds:organizations.read
scopes:
- description: 'The only scope named in the OpenAPI security requirements. Applied to exactly three operations: sensor-clients (GET /clients/sensors), sensor-kpis-by-organization (GET /kpis/sensors/organizations) and sensor-kpis-by-access-point (GET /kpis/sensors/access-points/{accessPointId}). The other 212 operations declare `oauth2: []` with no scope named.'
  flows: []
  scope: read
- description: OpenID Connect authentication of the agent's human operator.
  flows: []
  scope: openid
- description: Basic profile claims for the authenticated user.
  flows: []
  scope: profile
- description: Email claim for the authenticated user.
  flows: []
  scope: email
- description: Issue a refresh token so the agent session survives access-token expiry.
  flows: []
  scope: offline_access
- description: Read the authenticated 7SIGNAL user record.
  flows: []
  scope: https://login.7signal.com/scopes/user.read
- description: Administrative access to the user's 7SIGNAL organization.
  flows: []
  scope: https://login.7signal.com/scopes/organization.admin
- description: Read access to Sapphire (sensor platform) user data.
  flows: []
  scope: sap:user.read
- description: Sapphire user configuration access.
  flows: []
  scope: sap:user.config
- description: Read organizations from the MDS (managed data services) layer.
  flows: []
  scope: mds:organizations.read
slug: 7signalsolutions-scopes
source_filename: 7signalsolutions-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://mcp-v2.7signal.com/.well-known/oauth-protected-resource\ndocs: https://github.com/7Signal/API-Examples/blob/develop/docs/01-authentication.md\nnote: >-\n  The REST gateway's OpenAPI declares an oauth2 clientCredentials scheme whose scopes map is empty; only\n  three of the 215 operations carry an explicit `read` scope requirement, and the remaining 211 declare\n  `oauth2: []`. The published scope vocabulary lives on the MCP surface instead, in the RFC 9728\n  protected-resource document. 7SIGNAL's auth docs show a token response carrying\n  `\"scope\": \"read:resources write:resources\"` as an illustrative example, not an enumerated reference,\n  so those two strings are NOT recorded here as real scopes.\nschemes:\n- name: oauth2\n  surface: 7SIGNAL Platform API (Gateway v2)\n  source: openapi/7signalsolutions-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-v2.7signal.com/oauth2/token\n\
  - name: mcp_oauth\n  surface: 7SIGNAL MCP Server\n  source: https://mcp-v2.7signal.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorization_code\n    authorizationUrl: https://mcp-v2.7signal.com/authorize\n    tokenUrl: https://mcp-v2.7signal.com/token\nscopes:\n- scope: read\n  surface: 7SIGNAL Platform API (Gateway v2)\n  description: >-\n    The only scope named in the OpenAPI security requirements. Applied to exactly three operations:\n    sensor-clients (GET /clients/sensors), sensor-kpis-by-organization (GET /kpis/sensors/organizations)\n    and sensor-kpis-by-access-point (GET /kpis/sensors/access-points/{accessPointId}). The other 212\n    operations declare `oauth2: []` with no scope named.\n  sources:\n  - openapi/7signalsolutions-openapi.json\n- scope: openid\n  surface: 7SIGNAL MCP Server\n  description: OpenID Connect authentication of the agent's human operator.\n  sources:\n  - https://mcp-v2.7signal.com/.well-known/oauth-protected-resource\n- scope:\
  \ profile\n  surface: 7SIGNAL MCP Server\n  description: Basic profile claims for the authenticated user.\n  sources:\n  - https://mcp-v2.7signal.com/.well-known/oauth-protected-resource\n- scope: email\n  surface: 7SIGNAL MCP Server\n  description: Email claim for the authenticated user.\n  sources:\n  - https://mcp-v2.7signal.com/.well-known/oauth-protected-resource\n- scope: offline_access\n  surface: 7SIGNAL MCP Server\n  description: Issue a refresh token so the agent session survives access-token expiry.\n  sources:\n  - https://mcp-v2.7signal.com/.well-known/oauth-protected-resource\n- scope: https://login.7signal.com/scopes/user.read\n  surface: 7SIGNAL MCP Server\n  description: Read the authenticated 7SIGNAL user record.\n  sources:\n  - https://mcp-v2.7signal.com/.well-known/oauth-protected-resource\n- scope: https://login.7signal.com/scopes/organization.admin\n  surface: 7SIGNAL MCP Server\n  description: Administrative access to the user's 7SIGNAL organization.\n  sources:\n\
  \  - https://mcp-v2.7signal.com/.well-known/oauth-protected-resource\n- scope: sap:user.read\n  surface: 7SIGNAL MCP Server\n  description: Read access to Sapphire (sensor platform) user data.\n  sources:\n  - https://mcp-v2.7signal.com/.well-known/oauth-protected-resource\n- scope: sap:user.config\n  surface: 7SIGNAL MCP Server\n  description: Sapphire user configuration access.\n  sources:\n  - https://mcp-v2.7signal.com/.well-known/oauth-protected-resource\n- scope: mds:organizations.read\n  surface: 7SIGNAL MCP Server\n  description: Read organizations from the MDS (managed data services) layer.\n  sources:\n  - https://mcp-v2.7signal.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7signalsolutions/refs/heads/main/scopes/7signalsolutions-scopes.yml
summary_line: 10 scopes · clientCredentials/authorization_code
tags:
- Wireless Network Monitoring
- Wi-Fi Experience Monitoring
- Digital Experience Monitoring
- Network Performance Monitoring
- Network Observability
- AIOps
- IT Operations
- Endpoint Monitoring
- Time Series
- MCP
- agent-native
- Company
token_urls:
- https://api-v2.7signal.com/oauth2/token
- https://mcp-v2.7signal.com/token
---
