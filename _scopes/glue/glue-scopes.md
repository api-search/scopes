---
authorization_urls: []
description: ''
docs: https://docs.glue.ai/developers/authentication/scopes.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Glue Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Glue publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Glue API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Glue
provider_slug: glue
schemes:
- flow: clientCredentials
  name: GraphQLOAuth2ClientCredentials
  tokenUrl: https://api.gluegroups.com/oauth/token
- authorizationUrl: https://api.glue.ai/oauth/authorize
  flow: authorizationCode
  name: MCPOAuth2AuthorizationCode
  tokenUrl: https://api.glue.ai/oauth/token
scope_count: 6
scope_names:
- workspaces:read
- threads:read
- groups:read
- threads.messages:write
- mcp:read
- mcp:write
scopes:
- description: View workspace information
  flows:
  - clientCredentials
  scope: workspaces:read
- description: View thread information
  flows:
  - clientCredentials
  scope: threads:read
- description: View group information
  flows:
  - clientCredentials
  scope: groups:read
- description: Send messages in threads, group chats and DMs
  flows:
  - clientCredentials
  scope: threads.messages:write
- description: Read access via the hosted MCP server
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access via the hosted MCP server
  flows:
  - authorizationCode
  scope: mcp:write
slug: glue-scopes
source_filename: glue-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.glue.ai/developers/authentication/scopes.md\ndocs: https://docs.glue.ai/developers/authentication/scopes.md\nschemes:\n  - name: GraphQLOAuth2ClientCredentials\n    flow: clientCredentials\n    tokenUrl: https://api.gluegroups.com/oauth/token\n  - name: MCPOAuth2AuthorizationCode\n    flow: authorizationCode\n    authorizationUrl: https://api.glue.ai/oauth/authorize\n    tokenUrl: https://api.glue.ai/oauth/token\nscopes:\n  - scope: workspaces:read\n    description: View workspace information\n    flows: [clientCredentials]\n    sources: [https://docs.glue.ai/developers/authentication/scopes.md]\n  - scope: threads:read\n    description: View thread information\n    flows: [clientCredentials]\n    sources: [https://docs.glue.ai/developers/authentication/scopes.md]\n  - scope: groups:read\n    description: View group information\n    flows: [clientCredentials]\n    sources: [https://docs.glue.ai/developers/authentication/scopes.md]\n\
  \  - scope: threads.messages:write\n    description: Send messages in threads, group chats and DMs\n    flows: [clientCredentials]\n    sources: [https://docs.glue.ai/developers/authentication/scopes.md]\n  - scope: mcp:read\n    description: Read access via the hosted MCP server\n    flows: [authorizationCode]\n    sources: [https://api.glue.ai/.well-known/oauth-authorization-server]\n  - scope: mcp:write\n    description: Write access via the hosted MCP server\n    flows: [authorizationCode]\n    sources: [https://api.glue.ai/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glue/refs/heads/main/scopes/glue-scopes.yml
summary_line: 6 scopes
tags:
- Company
- SaaS
- Team Communication
- Messaging
- Collaboration
- GraphQL
- Webhooks
- MCP
- Productivity
- AI Agents
token_urls: []
---
