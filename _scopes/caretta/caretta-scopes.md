---
authorization_urls: []
description: ''
docs: https://www.caretta.so/docs/caretta-mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Caretta Scopes
name_suffix: OAuth Scopes
note: 'Caretta issues no API keys. The only authorization surface is the OAuth flow in front of the MCP server. Two distinct scope layers exist and they do not match, which is recorded here rather than reconciled: the RFC 9728 protected-resource document advertises only the OIDC scope "openid", while the three product scopes a user actually consents to are documented in the developer docs and surfaced in the consent screen.'
overview: 'Caretta publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Caretta API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Caretta
provider_slug: caretta
schemes:
- authorization_servers:
  - authorization_endpoint: https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1/oauth/authorize
    code_challenge_methods_supported:
    - S256
    - plain
    grant_types_supported:
    - authorization_code
    - refresh_token
    issuer: https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1
    jwks_uri: https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1/.well-known/jwks.json
    note: Third-party Supabase Auth tenant, named as the authorization server by Caretta's own protected-resource document. Its metadata is generic Supabase Auth and is recorded as evidence, not as a Caretta-authored document.
    registration_endpoint: https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1/oauth/clients/register
    response_types_supported:
    - code
    scopes_supported:
    - openid
    - profile
    - email
    - phone
    - offline_access
    token_endpoint: https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1/oauth/token
  bearer_methods_supported:
  - header
  name: MCP OAuth
  protected_resource_metadata: https://gateway.caretta.app/.well-known/oauth-protected-resource
  resource: https://gateway.caretta.app/mcp
  type: oauth2
scope_count: 4
scope_names:
- calls:read
- todos:read
- todos:write
- openid
scopes:
- description: View call metadata, summaries, and transcripts you can access.
  flows: []
  scope: calls:read
- description: View todos created from your calls.
  flows: []
  scope: todos:read
- description: Add new todos and modify existing todos on calls you can access.
  flows: []
  scope: todos:write
- description: OIDC subject identity. The only scope advertised in the RFC 9728 metadata.
  flows: []
  scope: openid
slug: caretta-scopes
source_filename: caretta-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://gateway.caretta.app/.well-known/oauth-protected-resource\ndocs: https://www.caretta.so/docs/caretta-mcp\n\nnote: >-\n  Caretta issues no API keys. The only authorization surface is the OAuth flow\n  in front of the MCP server. Two distinct scope layers exist and they do not\n  match, which is recorded here rather than reconciled: the RFC 9728\n  protected-resource document advertises only the OIDC scope \"openid\", while the\n  three product scopes a user actually consents to are documented in the\n  developer docs and surfaced in the consent screen.\n\nschemes:\n- name: MCP OAuth\n  type: oauth2\n  resource: https://gateway.caretta.app/mcp\n  protected_resource_metadata: https://gateway.caretta.app/.well-known/oauth-protected-resource\n  bearer_methods_supported: [header]\n  authorization_servers:\n  - issuer: https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1\n    authorization_endpoint: https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1/oauth/authorize\n\
  \    token_endpoint: https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1/oauth/token\n    jwks_uri: https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1/.well-known/jwks.json\n    registration_endpoint: https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1/oauth/clients/register\n    grant_types_supported: [authorization_code, refresh_token]\n    response_types_supported: [code]\n    code_challenge_methods_supported: [S256, plain]\n    scopes_supported: [openid, profile, email, phone, offline_access]\n    note: >-\n      Third-party Supabase Auth tenant, named as the authorization server by\n      Caretta's own protected-resource document. Its metadata is generic Supabase\n      Auth and is recorded as evidence, not as a Caretta-authored document.\n\nscopes:\n- scope: calls:read\n  description: View call metadata, summaries, and transcripts you can access.\n  layer: product\n  sources: [https://www.caretta.so/docs/caretta-mcp]\n  grants_tools: [caretta_list_calls, caretta_list_my_calls, caretta_search_transcripts,\
  \ caretta_get_call]\n- scope: todos:read\n  description: View todos created from your calls.\n  layer: product\n  sources: [https://www.caretta.so/docs/caretta-mcp]\n  grants_tools: [caretta_list_todos, caretta_get_call]\n- scope: todos:write\n  description: Add new todos and modify existing todos on calls you can access.\n  layer: product\n  sources: [https://www.caretta.so/docs/caretta-mcp]\n  grants_tools: [caretta_create_todo, caretta_update_todo]\n- scope: openid\n  description: OIDC subject identity. The only scope advertised in the RFC 9728 metadata.\n  layer: transport\n  sources: [https://gateway.caretta.app/.well-known/oauth-protected-resource]\n\nconsent_model:\n  user_selects_scopes: true\n  least_privilege_guidance: >-\n    Provider guidance: grant calls:read for call and transcript questions, add\n    todos:read to retrieve todos, and add todos:write only if the client should\n    create or change them.\n  escalation: >-\n    Existing authorisations cannot silently expand\
  \ their own permissions. To add\n    a scope, unauthorise the client in Settings -> Caretta MCP and reconnect.\n  revocation: >-\n    Per-client Unauthorise in Settings -> Caretta MCP. Revoking one client does\n    not affect other authorised MCP clients.\n\nx-evidence:\n- url: https://gateway.caretta.app/.well-known/oauth-protected-resource\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://ztejbfpbhxgwecvxngtf.supabase.co/auth/v1/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://www.caretta.so/docs/caretta-mcp\n  http_status: 200\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caretta/refs/heads/main/scopes/caretta-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Artificial Intelligence
- Sales
- Sales Intelligence
- Real-Time
- Conversation Intelligence
- Revenue Operations
- Y Combinator
- Model Context Protocol
- Webhooks
- Agents
token_urls: []
---
