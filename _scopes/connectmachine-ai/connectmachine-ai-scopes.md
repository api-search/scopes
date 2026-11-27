---
authorization_urls: []
description: OAuth scopes the docs list for the native Zapier integration (approved on the ConnectMachine consent page). The MCP server's OAuth scopes are not documented.
docs: https://www.connectmachine.ai/docs/#zapier-native
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: ConnectMachine Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ConnectMachine publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the ConnectMachine API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ConnectMachine
provider_slug: connectmachine-ai
schemes:
- docs: https://www.connectmachine.ai/docs/#zapier-native
  grant_types:
  - authorization_code
  - refresh_token
  name: zapierOAuth
  notes: authorization code with S256 PKCE and automatic refresh
  type: oauth2
scope_count: 4
scope_names:
- user:read
- contacts:read
- contacts:write
- webhooks:write
scopes:
- description: labels the connection
  flows: []
  scope: user:read
- description: powers triggers, samples, and dropdowns
  flows: []
  scope: contacts:read
- description: permits Create Contact and Update Contact
  flows: []
  scope: contacts:write
- description: lets Zapier manage only its own trigger subscriptions
  flows: []
  scope: webhooks:write
slug: connectmachine-ai-scopes
source_filename: connectmachine-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.connectmachine.ai/docs/#zapier-native\ndocs: https://www.connectmachine.ai/docs/#zapier-native\ndescription: OAuth scopes the docs list for the native Zapier integration (approved on the ConnectMachine consent page). The MCP server's OAuth scopes are not documented.\nschemes:\n- name: zapierOAuth\n  type: oauth2\n  grant_types: [authorization_code, refresh_token]\n  docs: https://www.connectmachine.ai/docs/#zapier-native\n  notes: authorization code with S256 PKCE and automatic refresh\nscopes:\n- scope: user:read\n  description: labels the connection\n  schemes: [zapierOAuth]\n- scope: contacts:read\n  description: powers triggers, samples, and dropdowns\n  schemes: [zapierOAuth]\n- scope: contacts:write\n  description: permits Create Contact and Update Contact\n  schemes: [zapierOAuth]\n- scope: webhooks:write\n  description: lets Zapier manage only its own trigger subscriptions\n  schemes: [zapierOAuth]\n"
source_yaml_url: https://artifacts.apis.io/connectmachine-ai/scopes/connectmachine-ai-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Digital Business Cards
- Contact Management
- Business Card Scanner
- Networking
- Artificial Intelligence
- MCP
- CRM
token_bound: false
token_urls: []
---
