---
authorization_urls: []
description: ''
docs: https://cooperpetcare.app/llms-full.txt
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cooper Pet Care Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cooper Pet Care publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cooper Pet Care API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cooper Pet Care
provider_slug: cooperpetcare-app
schemes: []
scope_count: 2
scope_names:
- mcp.read
- mcp.write
scopes:
- description: Read the authenticated user's data (consulta de datos del usuario).
  flows: []
  scope: mcp.read
- description: Actions on the user's behalf; the assistant must ask for explicit user confirmation before invoking.
  flows: []
  scope: mcp.write
slug: cooperpetcare-app-scopes
source_filename: cooperpetcare-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cooperpetcare.app/llms-full.txt\ndocs: https://cooperpetcare.app/llms-full.txt\napplies_to: Cooper MCP server (OAuth 2.1 + PKCE against Amazon Cognito)\nscopes:\n- name: mcp.read\n  description: Read the authenticated user's data (consulta de datos del usuario).\n  tools: [getMyOrders, getMyOrderDetail, getMyPets, getMyChats, getChatMessages]\n- name: mcp.write\n  description: Actions on the user's behalf; the assistant must ask for explicit user confirmation before invoking.\n  tools: [createOrder, sendChatMessage]\n"
source_yaml_url: https://artifacts.apis.io/cooperpetcare-app/scopes/cooperpetcare-app-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Pet Care
- Dog Walking
- Dog Boarding
- Dog Training
- Marketplace
- Mobile App
- Argentina
- Latin America
- MCP
token_bound: false
token_urls: []
---
