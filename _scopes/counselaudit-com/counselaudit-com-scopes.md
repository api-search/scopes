---
authorization_urls: []
description: ''
docs: https://www.counselaudit.com/mcp.html
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CounselAudit Scopes
name_suffix: OAuth Scopes
note: scopes_supported as advertised by the authorization server (Clerk). These are identity scopes; CounselAudit documents no product-level permission scopes — the MCP page says every request runs under the user's own account, scoped to their organization.
overview: 'CounselAudit publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CounselAudit API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CounselAudit
provider_slug: counselaudit-com
schemes: []
scope_count: 6
scope_names:
- openid
- profile
- email
- public_metadata
- private_metadata
- offline_access
scopes:
- description: OpenID Connect sign-in (identity provider scope, Clerk).
  flows: []
  scope: openid
- description: Basic profile claims.
  flows: []
  scope: profile
- description: Email claim.
  flows: []
  scope: email
- description: Clerk user public metadata.
  flows: []
  scope: public_metadata
- description: Clerk user private metadata.
  flows: []
  scope: private_metadata
- description: Refresh tokens.
  flows: []
  scope: offline_access
slug: counselaudit-com-scopes
source_filename: counselaudit-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://clerk.counselaudit.com/.well-known/oauth-authorization-server\ndocs: https://www.counselaudit.com/mcp.html\nscopes:\n- name: openid\n  description: OpenID Connect sign-in (identity provider scope, Clerk).\n- name: profile\n  description: Basic profile claims.\n- name: email\n  description: Email claim.\n- name: public_metadata\n  description: Clerk user public metadata.\n- name: private_metadata\n  description: Clerk user private metadata.\n- name: offline_access\n  description: Refresh tokens.\nnote: scopes_supported as advertised by the authorization server (Clerk). These are identity scopes; CounselAudit documents no product-level permission scopes — the MCP page says every request runs under the user's own account, scoped to their organization.\n"
source_yaml_url: https://artifacts.apis.io/counselaudit-com/scopes/counselaudit-com-scopes.yml
summary_line: 6 scopes
tags:
- Company
- Legal Tech
- Legal Billing
- Invoice Review
- E-Billing
- Outside Counsel Guidelines
- Artificial Intelligence
- MCP
token_bound: false
token_urls: []
---
