---
authorization_urls:
- https://docsend.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Docsend Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'DocSend publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the DocSend API on a user''s behalf.


  Tokens are issued from https://docsend.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DocSend
provider_slug: docsend
schemes:
- flows:
  - authorizationUrl: https://docsend.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://docsend.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://docsend.com/oauth/token
  name: OAuth2
  source: well-known/docsend-oauth-authorization-server.json
scope_count: 5
scope_names:
- documents:read
- spaces:read
- spaces:write
- analytics:read
- contacts:read
scopes:
- description: Read access to DocSend documents and the links that share them.
  flows:
  - authorizationCode
  - clientCredentials
  scope: documents:read
- description: Read access to DocSend Spaces (virtual data rooms) and their contents.
  flows:
  - authorizationCode
  - clientCredentials
  scope: spaces:read
- description: Write access to DocSend Spaces (virtual data rooms) — the only write scope DocSend advertises on this resource.
  flows:
  - authorizationCode
  - clientCredentials
  scope: spaces:write
- description: Read access to DocSend viewer analytics (visits, page-by-page engagement).
  flows:
  - authorizationCode
  - clientCredentials
  scope: analytics:read
- description: Read access to DocSend contacts / visitors captured against shared links.
  flows:
  - authorizationCode
  - clientCredentials
  scope: contacts:read
slug: docsend-scopes
source_filename: docsend-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  scopes_supported in https://docsend.com/.well-known/oauth-authorization-server and\n  https://mcp.docsend.com/.well-known/oauth-authorization-server, plus scopes_supported in\n  https://docsend.com/.well-known/oauth-protected-resource/mcp and the scope=\"...\" value in\n  the WWW-Authenticate challenge returned by https://docsend.com/mcp\ndocs: null\ndocs_note: >-\n  DocSend publishes no readable scope/permission reference page. www.docsend.com and\n  help.docsend.com return HTTP 403 (Cloudflare bot challenge) to non-browser clients, so\n  the scope descriptions below are honest readings of the scope names themselves against\n  DocSend's product vocabulary, not copy from a provider scopes page.\nschemes:\n- name: OAuth2\n  source: well-known/docsend-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://docsend.com/oauth/authorize\n    tokenUrl: https://docsend.com/oauth/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://docsend.com/oauth/token\nscopes:\n- scope: documents:read\n  description: Read access to DocSend documents and the links that share them.\n  access: read\n  domain: documents\n  flows: [authorizationCode, clientCredentials]\n  sources:\n  - well-known/docsend-oauth-authorization-server.json\n  - well-known/docsend-oauth-protected-resource-mcp.json\n- scope: spaces:read\n  description: Read access to DocSend Spaces (virtual data rooms) and their contents.\n  access: read\n  domain: spaces\n  flows: [authorizationCode, clientCredentials]\n  sources:\n  - well-known/docsend-oauth-authorization-server.json\n  - well-known/docsend-oauth-protected-resource-mcp.json\n- scope: spaces:write\n  description: >-\n    Write access to DocSend Spaces (virtual data rooms) — the only write scope DocSend\n    advertises on this resource.\n  access: write\n  domain: spaces\n  flows: [authorizationCode, clientCredentials]\n  sources:\n  - well-known/docsend-oauth-authorization-server.json\n\
  \  - well-known/docsend-oauth-protected-resource-mcp.json\n- scope: analytics:read\n  description: Read access to DocSend viewer analytics (visits, page-by-page engagement).\n  access: read\n  domain: analytics\n  flows: [authorizationCode, clientCredentials]\n  sources:\n  - well-known/docsend-oauth-authorization-server.json\n  - well-known/docsend-oauth-protected-resource-mcp.json\n- scope: contacts:read\n  description: Read access to DocSend contacts / visitors captured against shared links.\n  access: read\n  domain: contacts\n  flows: [authorizationCode, clientCredentials]\n  sources:\n  - well-known/docsend-oauth-authorization-server.json\n  - well-known/docsend-oauth-protected-resource-mcp.json\nresource:\n  identifier: https://docsend.com/mcp\n  authorization_servers: [https://docsend.com]\n  bearer_methods_supported: [header]\nchanges_since_last_round:\n  checked: '2026-08-14'\n  previous: '2026-07-18'\n  removed: [mcp:read, mcp:write]\n  added: [documents:read, spaces:read, spaces:write,\
  \ analytics:read, contacts:read]\n  notes: >-\n    The coarse mcp:read / mcp:write pair recorded on 2026-07-18 no longer appears in any\n    DocSend discovery document or in the live WWW-Authenticate challenge. It has been\n    replaced by five resource-scoped scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docsend/refs/heads/main/scopes/docsend-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Company
- Enterprise
- Document Sharing
- Sales Enablement
- Analytics
- Data Room
- E-Signature
- MCP
- Dropbox
token_urls:
- https://docsend.com/oauth/token
---
