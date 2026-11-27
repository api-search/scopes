---
authorization_urls: []
description: ''
docs: https://cmein.com/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CMeIn Scopes
name_suffix: OAuth Scopes
note: Scope list from the authorization-server and protected-resource metadata (GET, HTTP 200, 2026-11-04). Tool-to-scope mapping is from each tool's own description in the anonymous tools/list (examples/cmein-com-mcp-tools-list.json). photos:write is advertised by the authorization server but not by the MCP resource and no documented tool requires it.
overview: 'CMeIn publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CMeIn API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CMeIn
provider_slug: cmein-com
schemes: []
scope_count: 5
scope_names:
- credits:read
- photos:read
- scenes:read
- support:write
- photos:write
scopes:
- description: Read the credit balance on the connected account.
  flows: []
  scope: credits:read
- description: Read recent generations (scene, completion status, date; images are not returned).
  flows: []
  scope: photos:read
- description: Search the scene catalogue filtered to the account.
  flows: []
  scope: scenes:read
- description: Open a credits-back request answered by a person by email.
  flows: []
  scope: support:write
- description: Advertised in authorization-server metadata only; no documented tool uses it and it is not in the MCP resource's scopes_supported.
  flows: []
  scope: photos:write
slug: cmein-com-scopes
source_filename: cmein-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: CMeIn OAuth scopes\ngenerated: '2026-11-04'\nmethod: probed\nsource:\n- https://cmein.com/.well-known/oauth-authorization-server\n- https://mcp.cmein.com/.well-known/oauth-protected-resource\ndocs: https://cmein.com/mcp\nnote: Scope list from the authorization-server and protected-resource metadata (GET, HTTP 200, 2026-11-04). Tool-to-scope mapping is from each tool's own description in the anonymous tools/list (examples/cmein-com-mcp-tools-list.json). photos:write is advertised by the authorization server but not by the MCP resource and no documented tool requires it.\nscopes:\n- name: credits:read\n  description: Read the credit balance on the connected account.\n  tools: [my_credits]\n- name: photos:read\n  description: Read recent generations (scene, completion status, date; images are not returned).\n  tools: [my_generations]\n- name: scenes:read\n  description: Search the scene catalogue filtered to the account.\n  tools: [find_scene]\n- name: support:write\n  description:\
  \ Open a credits-back request answered by a person by email.\n  tools: [request_credits_back]\n- name: photos:write\n  description: Advertised in authorization-server metadata only; no documented tool uses it and it is not in the MCP resource's scopes_supported.\n  tools: []\n"
source_yaml_url: https://artifacts.apis.io/cmein-com/scopes/cmein-com-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Artificial Intelligence
- AI Image Generation
- Photos
- Dating
- Headshots
- Consumer App
- MCP
token_bound: false
token_urls: []
---
