---
authorization_urls: []
description: ''
docs: https://www.nextw.com/docs/mcpserver
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Nextworld Scopes
name_suffix: OAuth Scopes
note: These are not derived from an OpenAPI securityScheme — Nextworld publishes no OpenAPI. They are read verbatim from the RFC 9728 protected-resource metadata the MCP endpoint serves anonymously, captured at well-known/nextworld-oauth-protected-resource.json (HTTP 200, 2026-08-26). The authorization server is an AWS Cognito user pool, whose OIDC discovery document advertises only the four standard OIDC scopes; the resource-specific scope is declared by the resource server.
overview: 'Nextworld uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nextworld
provider_slug: nextworld
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: nextworld-scopes
source_filename: nextworld-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://apps.nextworld.net/ai/mcp/.well-known/oauth-protected-resource\ndocs: https://www.nextw.com/docs/mcpserver\nname: Nextworld OAuth scopes\nnote: >-\n  These are not derived from an OpenAPI securityScheme — Nextworld publishes no OpenAPI. They are\n  read verbatim from the RFC 9728 protected-resource metadata the MCP endpoint serves anonymously,\n  captured at well-known/nextworld-oauth-protected-resource.json (HTTP 200, 2026-08-26). The\n  authorization server is an AWS Cognito user pool, whose OIDC discovery document advertises only the\n  four standard OIDC scopes; the resource-specific scope is declared by the resource server.\nauthorization_servers:\n- issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_EJas25nD4\n  authorization_endpoint: https://464682c0-7c75-11f1-9d48-12d6f76c75f7.auth.us-east-1.amazoncognito.com/oauth2/authorize\n  token_endpoint: https://464682c0-7c75-11f1-9d48-12d6f76c75f7.auth.us-east-1.amazoncognito.com/oauth2/token\n\
  \  revocation_endpoint: https://464682c0-7c75-11f1-9d48-12d6f76c75f7.auth.us-east-1.amazoncognito.com/oauth2/revoke\n  userinfo_endpoint: https://464682c0-7c75-11f1-9d48-12d6f76c75f7.auth.us-east-1.amazoncognito.com/oauth2/userInfo\n  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_EJas25nD4/.well-known/jwks.json\nprotected_resources:\n- resource: https://apps.nextworld.net/ai/mcp\n  bearer_methods_supported:\n  - header\n  - body\nscope_count: 5\nscopes:\n- name: https://apps.nextworld.net/ai/mcp/access\n  type: resource\n  description: >-\n    Resource-server scope granting an MCP client access to the Nextworld MCP endpoint. Nextworld\n    publishes no separate per-operation scopes — actual authorization is enforced downstream by the\n    platform's own RUID permission model (security groups, permission definitions, roles, role\n    hierarchies, org unit security), scoped to the connecting user.\n- name: openid\n  type: oidc\n  description: Standard OpenID Connect scope;\
  \ requests an ID token.\n- name: email\n  type: oidc\n  description: Standard OIDC claim scope; email and email_verified.\n- name: phone\n  type: oidc\n  description: Standard OIDC claim scope; phone_number and phone_number_verified.\n- name: profile\n  type: oidc\n  description: Standard OIDC claim scope; basic profile claims.\ngaps:\n- >-\n  There is no published scope reference page. Nextworld does not document a granular scope surface\n  for its REST endpoints; inbound REST calls authenticate with Basic Auth and receive a short-lived\n  bearer token rather than a scoped OAuth grant.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextworld/refs/heads/main/scopes/nextworld-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Enterprise Resource Planning
- No-Code
- Enterprise Application Platform
- Workflow Automation
- Artificial Intelligence
- Model Context Protocol
- Integration
- Manufacturing
- Distribution
token_urls: []
---
