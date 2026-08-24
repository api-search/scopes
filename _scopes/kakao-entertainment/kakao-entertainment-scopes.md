---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Kakao Entertainment Scopes
name_suffix: OAuth Scopes
note: Scopes read verbatim from scopes_supported in the provider's RFC 8414 authorization server metadata document. Kakao Entertainment publishes no scope reference page, so no scope descriptions are published by the provider; the description field below is an API Evangelist reading of the scope name and is marked as such, not a provider statement. No scope-to-tool mapping is published for the Melon MCP server.
overview: 'Kakao Entertainment publishes 10 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kakao Entertainment API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kakao Entertainment
provider_slug: kakao-entertainment
schemes: []
scope_count: 10
scope_names:
- melonAuthentication
- melonAccessAuthority
- melonService
- memberKey
- memberName
- memberNickname
- ipinGender
- ipinBirthDate
- realNameYn
- ticketService
scopes:
- description: Authenticate the end user against their Melon account.
  flows: []
  scope: melonAuthentication
- description: Access authority / permission level held by the Melon member.
  flows: []
  scope: melonAccessAuthority
- description: Access to Melon service functionality on behalf of the member.
  flows: []
  scope: melonService
- description: The member key identifying the Melon account.
  flows: []
  scope: memberKey
- description: The member name on the Melon account.
  flows: []
  scope: memberName
- description: The member nickname on the Melon account.
  flows: []
  scope: memberNickname
- description: Gender as verified through the Korean i-PIN identity verification service.
  flows: []
  scope: ipinGender
- description: Birth date as verified through the Korean i-PIN identity verification service.
  flows: []
  scope: ipinBirthDate
- description: Whether the member has completed real-name verification.
  flows: []
  scope: realNameYn
- description: Access to the member's Melon ticket / subscription (voucher) service state.
  flows: []
  scope: ticketService
slug: kakao-entertainment-scopes
source_filename: kakao-entertainment-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://cola.melon.com/.well-known/oauth-authorization-server\nnote: Scopes read verbatim from scopes_supported in the provider's RFC 8414 authorization server metadata\n  document. Kakao Entertainment publishes no scope reference page, so no scope descriptions are published\n  by the provider; the description field below is an API Evangelist reading of the scope name and is marked\n  as such, not a provider statement. No scope-to-tool mapping is published for the Melon MCP server.\nauthorization_server: https://cola.melon.com\ndocumentation: null\ndescription_provenance: api-evangelist-reading (provider publishes names only)\nscope_count: 10\nscopes:\n- scope: melonAuthentication\n  description: Authenticate the end user against their Melon account.\n  source: scopes_supported\n- scope: melonAccessAuthority\n  description: Access authority / permission level held by the Melon member.\n  source: scopes_supported\n- scope: melonService\n\
  \  description: Access to Melon service functionality on behalf of the member.\n  source: scopes_supported\n- scope: memberKey\n  description: The member key identifying the Melon account.\n  source: scopes_supported\n- scope: memberName\n  description: The member name on the Melon account.\n  source: scopes_supported\n- scope: memberNickname\n  description: The member nickname on the Melon account.\n  source: scopes_supported\n- scope: ipinGender\n  description: Gender as verified through the Korean i-PIN identity verification service.\n  source: scopes_supported\n- scope: ipinBirthDate\n  description: Birth date as verified through the Korean i-PIN identity verification service.\n  source: scopes_supported\n- scope: realNameYn\n  description: Whether the member has completed real-name verification.\n  source: scopes_supported\n- scope: ticketService\n  description: Access to the member's Melon ticket / subscription (voucher) service state.\n  source: scopes_supported\nx-evidence:\n \
  \ fetched: '2026-08-23'\n  url: https://cola.melon.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kakao-entertainment/refs/heads/main/scopes/kakao-entertainment-scopes.yml
summary_line: 10 scopes
tags:
- Entertainment
- Music
- Streaming
- Webtoons
- Publishing
- Media
- Model Context Protocol
- Agents
- South Korea
- Company
token_urls: []
---
