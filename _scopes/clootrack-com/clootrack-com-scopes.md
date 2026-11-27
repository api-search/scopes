---
authorization_urls: []
description: ''
docs: https://www.clootrack.com/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Clootrack Scopes
name_suffix: OAuth Scopes
note: Scopes as advertised in the MCP server's OAuth metadata. The protected-resource document (https://mcp.clootrack.com/.well-known/oauth-protected-resource) lists openid and profile; the authorization-server document adds offline_access. Clootrack documents no product-level permission scopes; data access follows platform RBAC.
overview: 'Clootrack publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clootrack API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clootrack
provider_slug: clootrack-com
schemes: []
scope_count: 3
scope_names:
- openid
- profile
- offline_access
scopes:
- description: OpenID Connect sign-in (listed in both protected-resource and authorization-server metadata).
  flows: []
  scope: openid
- description: Basic profile claims (listed in both metadata documents).
  flows: []
  scope: profile
- description: Refresh-token issuance (authorization-server metadata only; refresh_token grant is supported).
  flows: []
  scope: offline_access
slug: clootrack-com-scopes
source_filename: clootrack-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://mcp.clootrack.com/.well-known/oauth-authorization-server\ndocs: https://www.clootrack.com/mcp\nnote: >-\n  Scopes as advertised in the MCP server's OAuth metadata. The protected-resource document\n  (https://mcp.clootrack.com/.well-known/oauth-protected-resource) lists openid and profile; the authorization-server\n  document adds offline_access. Clootrack documents no product-level permission scopes; data access follows platform RBAC.\nscopes:\n- name: openid\n  description: OpenID Connect sign-in (listed in both protected-resource and authorization-server metadata).\n- name: profile\n  description: Basic profile claims (listed in both metadata documents).\n- name: offline_access\n  description: Refresh-token issuance (authorization-server metadata only; refresh_token grant is supported).\n"
source_yaml_url: https://artifacts.apis.io/clootrack-com/scopes/clootrack-com-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Customer Experience
- Voice of the Customer
- Customer Feedback Analytics
- Artificial Intelligence
- Sentiment Analysis
- MCP
token_bound: false
token_urls: []
---
