---
authorization_urls: []
description: OAuth scopes advertised by Laurence's authorization-server discovery document. Laurence does not publish a dedicated scopes/permissions reference page; the scope set below is taken verbatim from scopes_supported in the discovery metadata. Three are the standard OpenID Connect scopes; one vendor scope, laurence:mcp, gates the MCP server and is the only scope echoed by the MCP protected-resource metadata. Scopes are coarse-grained — authorization is enforced per Amazon Ads profile at call time rather than by finer-grained scopes.
docs: https://www.laurence.com/blog/laurence-mcp-launch
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Laurence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Laurence uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Laurence
provider_slug: laurence
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: laurence-scopes
source_filename: laurence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://www.laurence.com/.well-known/openid-configuration,\n  https://laurence-ai-68564--ask-laurence-agent-mcp-server.modal.run/.well-known/oauth-protected-resource\ndocs: https://www.laurence.com/blog/laurence-mcp-launch\ndescription: >-\n  OAuth scopes advertised by Laurence's authorization-server discovery document. Laurence does not\n  publish a dedicated scopes/permissions reference page; the scope set below is taken verbatim from\n  scopes_supported in the discovery metadata. Three are the standard OpenID Connect scopes; one\n  vendor scope, laurence:mcp, gates the MCP server and is the only scope echoed by the MCP\n  protected-resource metadata. Scopes are coarse-grained — authorization is enforced per Amazon Ads\n  profile at call time rather than by finer-grained scopes.\nissuer: https://www.laurence.com\nresource: https://laurence-ai-68564--ask-laurence-agent-mcp-server.modal.run/mcp\nscopes:\n  - name: openid\n\
  \    standard: oidc\n    description: Standard OpenID Connect scope requesting an ID token for the signed-in Laurence user.\n  - name: profile\n    standard: oidc\n    description: Standard OpenID Connect scope granting access to basic profile claims.\n  - name: email\n    standard: oidc\n    description: Standard OpenID Connect scope granting access to the user's email address claim.\n  - name: laurence:mcp\n    standard: vendor\n    description: >-\n      Grants a registered client read-only access to the Laurence MCP server's nine tools over the\n      Amazon Advertising and Amazon Marketing Stream data for the Ads profiles the signed-in user\n      belongs to. This is the only scope listed in scopes_supported on the MCP protected-resource\n      metadata.\n    resource: https://laurence-ai-68564--ask-laurence-agent-mcp-server.modal.run/mcp\nnotes:\n  - No scope-to-tool mapping is published; laurence:mcp appears to gate the whole tool surface.\n  - >-\n    Per-record authorization is\
  \ enforced by Amazon Ads profile membership, discoverable at runtime\n    via the list_allowed_ads_profiles tool, not through scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laurence/refs/heads/main/scopes/laurence-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Advertising
- Amazon
- E-Commerce
- Marketing
- Machine Learning
- Retail Media
- MCP
token_urls: []
---
