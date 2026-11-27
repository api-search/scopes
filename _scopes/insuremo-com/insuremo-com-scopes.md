---
api_specs:
- filename: insuremo-com-openapi-generated.yml
  format: yaml
  label: insureMO API Platform
  slug: insuremo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insuremo-com/openapi/_ae-authored/insuremo-com-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: insureMO Scopes
name_suffix: OAuth Scopes
note: Only OIDC identity scopes are advertised; no API-level permission scopes are published.
overview: 'insureMO publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the insureMO API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: insureMO
provider_slug: insuremo-com
schemes: []
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OpenID Connect sign-in
  flows: []
  scope: openid
- description: Profile claims (name, nickname, preferred_username)
  flows: []
  scope: profile
- description: Email claim
  flows: []
  scope: email
slug: insuremo-com-scopes
source_filename: insuremo-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: https://portal-gw.insuremo.com/.well-known/oauth-authorization-server\nscopes:\n- name: openid\n  description: OpenID Connect sign-in\n- name: profile\n  description: Profile claims (name, nickname, preferred_username)\n- name: email\n  description: Email claim\nnote: Only OIDC identity scopes are advertised; no API-level permission scopes are\n  published.\n"
source_yaml_url: https://artifacts.apis.io/insuremo-com/scopes/insuremo-com-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Insurance
- Artificial Intelligence
- Platform
token_bound: false
token_urls: []
---
