---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CreditPolicy.ai Scopes
name_suffix: OAuth Scopes
note: scopes_supported as advertised by the authorization server named in https://creditpolicy.ai/.well-known/oauth-protected-resource. These are generic Supabase Auth / OIDC scopes; no CreditPolicy-specific permission scopes are published, and the PRM lists no scopes_supported.
overview: 'CreditPolicy.ai publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CreditPolicy.ai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CreditPolicy.ai
provider_slug: creditpolicy-ai
schemes: []
scope_count: 5
scope_names:
- openid
- profile
- email
- phone
- offline_access
scopes:
- description: OpenID Connect sign-in
  flows: []
  scope: openid
- description: User profile claims
  flows: []
  scope: profile
- description: Email claim
  flows: []
  scope: email
- description: Phone claim
  flows: []
  scope: phone
- description: Refresh token issuance
  flows: []
  scope: offline_access
slug: creditpolicy-ai-scopes
source_filename: creditpolicy-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://txmbawsgucegjjaxcvae.supabase.co/auth/v1/.well-known/oauth-authorization-server\nnote: scopes_supported as advertised by the authorization server named in https://creditpolicy.ai/.well-known/oauth-protected-resource. These are generic Supabase Auth / OIDC scopes; no CreditPolicy-specific permission scopes are published, and the PRM lists no scopes_supported.\nscopes:\n- name: openid\n  description: OpenID Connect sign-in\n- name: profile\n  description: User profile claims\n- name: email\n  description: Email claim\n- name: phone\n  description: Phone claim\n- name: offline_access\n  description: Refresh token issuance\n"
source_yaml_url: https://artifacts.apis.io/creditpolicy-ai/scopes/creditpolicy-ai-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Artificial Intelligence
- Credit Policy
- Lending
- Mortgage Brokers
- MCP
- Financial Services
- Australia
token_bound: false
token_urls: []
---
