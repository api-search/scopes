---
api_specs:
- filename: capxule-ai-account-api-openapi.yml
  format: yaml
  label: Capxule Account API
  slug: capxule-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capxule-ai/openapi/capxule-ai-account-api-openapi.yml
- filename: capxule-ai-catalog-api-openapi.yml
  format: yaml
  label: Capxule Catalog API
  slug: capxule-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capxule-ai/openapi/capxule-ai-catalog-api-openapi.yml
- filename: capxule-ai-plan-api-openapi.yml
  format: yaml
  label: Capxule Plan API
  slug: capxule-ai-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capxule-ai/openapi/capxule-ai-plan-api-openapi.yml
authorization_urls: []
description: ''
docs: https://capxule.ai/identity
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Capxule Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares only an http bearer scheme; the scope family is documented on /identity ("Scopes, in product words (per delegation, coarse)") and enforced per tool per the changelog.
overview: 'Capxule publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Capxule API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Capxule
provider_slug: capxule-ai
schemes: []
scope_count: 4
scope_names:
- journey
- account:bind
- grant:revoke
- account:upgrade
scopes:
- description: Run guided journeys for you, one step at a time
  flows: []
  scope: journey
- description: Set up or connect your account for you, with a code you read back
  flows: []
  scope: account:bind
- description: Disconnect itself from your account when you ask
  flows: []
  scope: grant:revoke
- description: Send you a secure payment page when you ask to upgrade
  flows: []
  scope: account:upgrade
slug: capxule-ai-scopes
source_filename: capxule-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://capxule.ai/identity\ndocs: https://capxule.ai/identity\nnote: The OpenAPI declares only an http bearer scheme; the scope family is documented on /identity (\"Scopes, in product words (per delegation, coarse)\") and enforced per tool per the changelog.\nscopes:\n- name: journey\n  description: Run guided journeys for you, one step at a time\n  granted: every delegation\n- name: account:bind\n  description: Set up or connect your account for you, with a code you read back\n  granted: every delegation\n- name: grant:revoke\n  description: Disconnect itself from your account when you ask\n  granted: every delegation\n- name: account:upgrade\n  description: Send you a secure payment page when you ask to upgrade\n  granted: only where the host's policy permits brokering; absent from the consent screen elsewhere\nnot_scopes:\n- billing:read\n- account:admin\n"
source_yaml_url: https://artifacts.apis.io/capxule-ai/scopes/capxule-ai-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Context Marketplace
- Artificial Intelligence
- AI Agents
- MCP
- Education
- Test Preparation
- Knowledge
token_bound: false
token_urls: []
---
