---
authorization_urls: []
description: 'Two custom scopes on the MCP resource server plus standard OIDC scopes. Interactive connector tokens always carry both custom scopes; writes are actually gated by an org switch, admin role and confirm: true.'
docs: https://docs.cloudquell.com/mcp/connect-auth/authentication/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: CloudQuell Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CloudQuell publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CloudQuell API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CloudQuell
provider_slug: cloudquell-com
schemes: []
scope_count: 5
scope_names:
- https://mcp.cloudquell.com/mcp/read
- https://mcp.cloudquell.com/mcp/admin:write
- openid
- email
- profile
scopes:
- description: All 41 read tools, plus switch_organization. The only scope a cak_ service key can hold.
  flows: []
  scope: https://mcp.cloudquell.com/mcp/read
- description: Lets the other 23 write tools be attempted, in addition to read. It is not on its own permission to write.
  flows: []
  scope: https://mcp.cloudquell.com/mcp/admin:write
- description: Standard OIDC scope used to identify the user.
  flows: []
  scope: openid
- description: Standard OIDC scope used to identify the user.
  flows: []
  scope: email
- description: Standard OIDC scope used to identify the user.
  flows: []
  scope: profile
slug: cloudquell-com-scopes
source_filename: cloudquell-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.cloudquell.com/mcp/connect-auth/authentication/\ndocs: https://docs.cloudquell.com/mcp/connect-auth/authentication/\ndescription: 'Two custom scopes on the MCP resource server plus standard OIDC scopes. Interactive connector tokens always\n  carry both custom scopes; writes are actually gated by an org switch, admin role and confirm: true.'\nscopes:\n- scope: https://mcp.cloudquell.com/mcp/read\n  short: read\n  description: All 41 read tools, plus switch_organization. The only scope a cak_ service key can hold.\n- scope: https://mcp.cloudquell.com/mcp/admin:write\n  short: admin:write\n  description: Lets the other 23 write tools be attempted, in addition to read. It is not on its own permission to write.\n- scope: openid\n  description: Standard OIDC scope used to identify the user.\n- scope: email\n  description: Standard OIDC scope used to identify the user.\n- scope: profile\n  description: Standard OIDC scope\
  \ used to identify the user.\n"
source_yaml_url: https://artifacts.apis.io/cloudquell-com/scopes/cloudquell-com-scopes.yml
summary_line: 5 scopes
tags:
- Company
- FinOps
- Cloud Cost Management
- AI Cost Management
- Cost Allocation
- Anomaly Detection
- Multi-Cloud
- MCP
token_bound: false
token_urls: []
---
