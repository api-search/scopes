---
authorization_urls:
- https://scs.sifive.com/o/authorize/
description: The complete scope set SiFive Cloud Services advertises in its RFC 8414 metadata. SiFive publishes no scopes/permissions reference page, so these three values are the only authoritative statement of the SCS OAuth permission surface that exists publicly. The two mcp:* scopes are the provider's own evidence of a Model Context Protocol resource server behind the portal — see mcp/sifive-mcp.yml.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Sifive Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SiFive publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SiFive API on a user''s behalf.


  Tokens are issued from https://scs.sifive.com/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SiFive
provider_slug: sifive
schemes:
- flows:
  - authorizationUrl: https://scs.sifive.com/o/authorize/
    flow: authorizationCode
    tokenUrl: https://scs.sifive.com/o/token/
  name: SiFiveCloudServicesOAuth2
  source: https://scs.sifive.com/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- openid
- mcp:read
- mcp:write
scopes:
- description: Standard OpenID Connect scope requesting an ID token about the authenticated SiFive Cloud Services user. Signed RS256 per the metadata, though the advertised JWKS is currently empty.
  flows:
  - authorizationCode
  scope: openid
- description: Read access to the Model Context Protocol resource server behind SiFive Cloud Services. Description is inferred from the scope name and MCP convention — SiFive publishes no scope reference page. The resource endpoint itself was not publicly discoverable.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access to the Model Context Protocol resource server behind SiFive Cloud Services. Description is inferred from the scope name and MCP convention — SiFive publishes no scope reference page.
  flows:
  - authorizationCode
  scope: mcp:write
slug: sifive-scopes
source_filename: sifive-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://scs.sifive.com/.well-known/oauth-authorization-server\ndescription: >-\n  The complete scope set SiFive Cloud Services advertises in its RFC 8414 metadata. SiFive\n  publishes no scopes/permissions reference page, so these three values are the only\n  authoritative statement of the SCS OAuth permission surface that exists publicly. The\n  two mcp:* scopes are the provider's own evidence of a Model Context Protocol resource\n  server behind the portal — see mcp/sifive-mcp.yml.\nschemes:\n- name: SiFiveCloudServicesOAuth2\n  source: https://scs.sifive.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://scs.sifive.com/o/authorize/\n    tokenUrl: https://scs.sifive.com/o/token/\nscopes:\n- scope: openid\n  description: >-\n    Standard OpenID Connect scope requesting an ID token about the authenticated SiFive\n    Cloud Services user. Signed RS256 per the metadata,\
  \ though the advertised JWKS is\n    currently empty.\n  flows: [authorizationCode]\n  sources: ['https://scs.sifive.com/.well-known/oauth-authorization-server']\n- scope: 'mcp:read'\n  description: >-\n    Read access to the Model Context Protocol resource server behind SiFive Cloud\n    Services. Description is inferred from the scope name and MCP convention — SiFive\n    publishes no scope reference page. The resource endpoint itself was not publicly\n    discoverable.\n  flows: [authorizationCode]\n  sources: ['https://scs.sifive.com/.well-known/oauth-authorization-server']\n  x-description-inferred: true\n- scope: 'mcp:write'\n  description: >-\n    Write access to the Model Context Protocol resource server behind SiFive Cloud\n    Services. Description is inferred from the scope name and MCP convention — SiFive\n    publishes no scope reference page.\n  flows: [authorizationCode]\n  sources: ['https://scs.sifive.com/.well-known/oauth-authorization-server']\n  x-description-inferred:\
  \ true\ngaps:\n- >-\n  No published scopes/permissions reference. The names above are the entire public record;\n  the two mcp:* descriptions are inferred from the scope name, not quoted from SiFive.\n- >-\n  No RFC 9728 protected-resource metadata is served, so the resource server(s) these\n  scopes protect cannot be discovered from the authorization server.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://scs.sifive.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sifive/refs/heads/main/scopes/sifive-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Semiconductors
- RISC-V
- Processor IP
- Chip Design
- Embedded
- Hardware
- Developer Tools
- Electronic Design Automation
- OAuth
token_urls:
- https://scs.sifive.com/o/token/
---
