---
authorization_urls:
- https://www.adquick.com/mcp/oauth/authorize
description: ''
docs: https://www.adquick.com/mcp/usage-documentation
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Adquick Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AdQuick publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AdQuick API on a user''s behalf.


  Tokens are issued from https://www.adquick.com/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AdQuick
provider_slug: adquick
schemes:
- flows:
  - authorizationUrl: https://www.adquick.com/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.adquick.com/mcp/oauth/token
  name: MCPOAuth2
  source: https://www.adquick.com/.well-known/oauth-authorization-server
scope_count: 6
scope_names:
- inventory_read
- availability_read
- supplier_inventory
- campaign_read
- campaign_write
- programmatic_read
scopes:
- description: Search and browse advertising inventory
  flows: []
  scope: inventory_read
- description: Check unit availability
  flows: []
  scope: availability_read
- description: View supplier-specific inventory
  flows: []
  scope: supplier_inventory
- description: Search and view campaigns
  flows: []
  scope: campaign_read
- description: Create, update, and manage campaigns
  flows: []
  scope: campaign_write
- description: Read programmatic (DSP) plans and pacing
  flows: []
  scope: programmatic_read
slug: adquick-scopes
source_filename: adquick-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://www.adquick.com/.well-known/oauth-authorization-server\ndocs: https://www.adquick.com/mcp/usage-documentation\nnotes: >-\n  OAuth 2.0 scopes for the AdQuick MCP server. The authorization-server metadata advertises four\n  scopes (inventory_read, campaign_read, campaign_write, programmatic_read); the MCP usage\n  documentation additionally documents availability_read and supplier_inventory. All six are\n  captured. The partner REST API uses a static X-PARTNER-TOKEN header and has no OAuth scope surface.\nschemes:\n- name: MCPOAuth2\n  source: https://www.adquick.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.adquick.com/mcp/oauth/authorize\n    tokenUrl: https://www.adquick.com/mcp/oauth/token\nscopes:\n- scope: inventory_read\n  description: Search and browse advertising inventory\n  advertised_in_metadata: true\n- scope: availability_read\n  description:\
  \ Check unit availability\n  advertised_in_metadata: false\n- scope: supplier_inventory\n  description: View supplier-specific inventory\n  advertised_in_metadata: false\n- scope: campaign_read\n  description: Search and view campaigns\n  advertised_in_metadata: true\n- scope: campaign_write\n  description: Create, update, and manage campaigns\n  advertised_in_metadata: true\n- scope: programmatic_read\n  description: Read programmatic (DSP) plans and pacing\n  advertised_in_metadata: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adquick/refs/heads/main/scopes/adquick-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Enterprise Saas
- Advertising
- Out Of Home Advertising
- DOOH
- Programmatic Advertising
- Media Buying
- Marketing
- MCP
token_urls:
- https://www.adquick.com/mcp/oauth/token
---
