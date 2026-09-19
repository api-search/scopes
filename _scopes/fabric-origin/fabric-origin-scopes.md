---
api_specs:
- filename: fabric-origin-entertainment-api-openapi.yml
  format: yaml
  label: Fabric Origin Entertainment API
  slug: entertainment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-entertainment-api-openapi.yml
- filename: fabric-origin-celebrity-api-openapi.yml
  format: yaml
  label: Fabric Origin Celebrity API
  slug: celebrity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-celebrity-api-openapi.yml
- filename: fabric-origin-videos-api-openapi.yml
  format: yaml
  label: Fabric Origin Video API
  slug: video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-videos-api-openapi.yml
- filename: fabric-origin-images-api-openapi.yml
  format: yaml
  label: Fabric Origin Image API
  slug: image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-images-api-openapi.yml
- filename: fabric-origin-entertainment-api-openapi.yml
  format: yaml
  label: Fabric Origin Entertainment API
  slug: fabric-origin-entertainment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-entertainment-api-openapi.yml
- filename: fabric-origin-images-api-openapi.yml
  format: yaml
  label: Fabric Origin Images API
  slug: fabric-origin-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-images-api-openapi.yml
- filename: fabric-origin-videos-api-openapi.yml
  format: yaml
  label: Fabric Origin Videos API
  slug: fabric-origin-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-videos-api-openapi.yml
- filename: fabric-origin-fandango-api-openapi.yml
  format: yaml
  label: Fabric Origin Fandango API
  slug: fandango-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-fandango-api-openapi.yml
- filename: fabric-origin-metacritic-api-openapi.yml
  format: yaml
  label: Fabric Origin Metacritic API
  slug: metacritic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-metacritic-api-openapi.yml
- filename: fabric-origin-analytics-api-openapi.yml
  format: yaml
  label: Fabric Origin Analytics API
  slug: fabric-origin-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-analytics-api-openapi.yml
- filename: fabric-origin-common-api-openapi.yml
  format: yaml
  label: Fabric Origin Common API
  slug: fabric-origin-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-common-api-openapi.yml
- filename: fabric-origin-commonsense-api-openapi.yml
  format: yaml
  label: Fabric Origin Commonsense API
  slug: fabric-origin-commonsense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-commonsense-api-openapi.yml
- filename: fabric-origin-katchmedia-api-openapi.yml
  format: yaml
  label: Fabric Origin Katchmedia API
  slug: fabric-origin-katchmedia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-katchmedia-api-openapi.yml
- filename: fabric-origin-rabbitrecommendations-api-openapi.yml
  format: yaml
  label: Fabric Origin Rabbitrecommendations API
  slug: fabric-origin-rabbitrecommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-rabbitrecommendations-api-openapi.yml
- filename: fabric-origin-rev-api-openapi.yml
  format: yaml
  label: Fabric Origin Rev API
  slug: fabric-origin-rev-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-rev-api-openapi.yml
- filename: fabric-origin-rottentomatoes-api-openapi.yml
  format: yaml
  label: Fabric Origin Rottentomatoes API
  slug: fabric-origin-rottentomatoes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-rottentomatoes-api-openapi.yml
- filename: fabric-origin-tvgrid-api-openapi.yml
  format: yaml
  label: Fabric Origin Tvgrid API
  slug: fabric-origin-tvgrid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-tvgrid-api-openapi.yml
authorization_urls: []
description: 'OAuth scopes advertised by Fabric Origin''s two MCP authorization servers, read from their live RFC 8414 discovery documents. Both servers publish only OIDC identity scopes — there is no resource-permission scope vocabulary. Authorization is not scope-based: Origin Studio derives tenant and permissions from the identity in the token against the same RBAC model that governs human users, and Origin Insights is read-only and catalog-scoped.'
docs:
- https://knowledgebase.fabricdata.com/studio/origin-studio-mcp-server/origin-studio-mcp-server
- https://knowledgebase.fabricdata.com/insights/origin-insights-mcp/mcp-access
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Fabric Origin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fabric Origin uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fabric Origin
provider_slug: fabric-origin
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: fabric-origin-scopes
source_filename: fabric-origin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://mcp-api.studio.fabricdata.com/.well-known/oauth-authorization-server\ndocs:\n- https://knowledgebase.fabricdata.com/studio/origin-studio-mcp-server/origin-studio-mcp-server\n- https://knowledgebase.fabricdata.com/insights/origin-insights-mcp/mcp-access\nprovider: Fabric Origin\nproviderId: fabric-origin\ndescription: >-\n  OAuth scopes advertised by Fabric Origin's two MCP authorization servers, read from their live\n  RFC 8414 discovery documents. Both servers publish only OIDC identity scopes — there is no\n  resource-permission scope vocabulary. Authorization is not scope-based: Origin Studio derives\n  tenant and permissions from the identity in the token against the same RBAC model that governs\n  human users, and Origin Insights is read-only and catalog-scoped.\nauthorization_servers:\n- id: origin-studio-mcp\n  issuer: https://mcp-api.studio.fabricdata.com\n  discovery: https://mcp-api.studio.fabricdata.com/.well-known/oauth-authorization-server\n\
  \  probed_status: 200\n  scopes:\n  - name: openid\n    description: OIDC — issue an ID token for the signed-in Studio user.\n  - name: profile\n    description: OIDC — basic profile claims for the signed-in user.\n  - name: email\n    description: OIDC — email claim for the signed-in user.\n  - name: offline_access\n    description: >-\n      Issue a refresh token. Provider warns these are long-lived and NON-ROTATING; store encrypted\n      and revoke on user offboarding.\n  pkce_methods: [S256]\n  token_endpoint_auth_methods: [none]\n- id: origin-insights-mcp\n  issuer: https://insights.fabric-mcp.link/\n  discovery: https://insights.fabric-mcp.link/.well-known/oauth-authorization-server\n  probed_status: 200\n  scopes:\n  - name: openid\n    description: OIDC — issue an ID token.\n  - name: email\n    description: OIDC — email claim.\n  - name: profile\n    description: OIDC — basic profile claims.\n  bearer_methods_supported: [header]\npermission_model:\n  scope_based: false\n  note:\
  \ >-\n    Tool-level access on Origin Studio maps to the identity's Studio role and permission groups,\n    enforced server-side on every call. Tenant is inferred from the token and client-supplied tenant\n    hints are ignored. Origin Insights is read-only. The Xytech X2 MCP server (a different Fabric\n    product family) is documented as scoping OAuth grants to the individual tool level.\n  source: https://www.fabricdata.com/agent-governance\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/scopes/fabric-origin-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Entertainment
- Metadata
- Movies
- Television
- Games
- Celebrities
- Trailers
- Image
- TV Listings
- Market Intelligence
- Media
- MCP
token_urls: []
---
