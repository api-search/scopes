---
api_specs:
- filename: wefunder-openapi-original.yml
  format: yaml
  label: Wefunder API v2
  slug: wefunder-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-openapi-original.yml
authorization_urls:
- https://wefunder.com/oauth/authorize
description: ''
docs: https://docs.wefunder.com/api-reference
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Wefunder Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wefunder publishes 16 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wefunder API on a user''s behalf.


  Tokens are issued from https://wefunder.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wefunder
provider_slug: wefunder
schemes:
- description: OAuth 2.0 authorization with access tokens
  flows:
  - authorizationUrl: https://wefunder.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://wefunder.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://wefunder.com/oauth/token
  name: bearerAuth
  source: openapi/wefunder-openapi-original.yml
scope_count: 16
scope_names:
- admin:attribution
- read:attribution:aggregate
- read:attribution:anonymized
- read:attribution:full
- read:campaigns
- read:investments
- read:offerings
- read:profile
- read:public
- read:spvs
- read:syndicates
- read:webhooks
- write:profile
- write:spvs
- write:syndicates
- write:webhooks
scopes:
- description: Administrative access to attribution system (Tier 3 - Wefunder admins only)
  flows:
  - authorizationCode
  scope: admin:attribution
- description: Read aggregate attribution statistics (Tier 0)
  flows:
  - authorizationCode
  scope: read:attribution:aggregate
- description: Read anonymized attribution data (Tier 1 - requires approval)
  flows:
  - authorizationCode
  scope: read:attribution:anonymized
- description: Read full attribution data with investor PII (Tier 2 - founders only)
  flows:
  - authorizationCode
  scope: read:attribution:full
- description: Read campaign information for companies you founded
  flows:
  - authorizationCode
  scope: read:campaigns
- description: Read user investment data
  flows:
  - authorizationCode
  scope: read:investments
- description: ''
  flows: []
  scope: read:offerings
- description: Read user profile information
  flows:
  - authorizationCode
  scope: read:profile
- description: Read public deal data (explore offerings); requires no user context
  flows:
  - authorizationCode
  - clientCredentials
  scope: read:public
- description: View partner SPVs, their invites, sessions, and investments
  flows:
  - authorizationCode
  scope: read:spvs
- description: View syndicates, members, deals, and portfolio
  flows:
  - authorizationCode
  scope: read:syndicates
- description: View webhook subscriptions
  flows:
  - authorizationCode
  scope: read:webhooks
- description: ''
  flows: []
  scope: write:profile
- description: Create and manage partner SPVs, invites, and investment sessions
  flows:
  - authorizationCode
  scope: write:spvs
- description: Manage members, update settings, operate on deals
  flows:
  - authorizationCode
  scope: write:syndicates
- description: Create, update, and delete webhook subscriptions
  flows:
  - authorizationCode
  scope: write:webhooks
slug: wefunder-scopes
source_filename: wefunder-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/wefunder-openapi-original.yml + https://wefunder.com/.well-known/oauth-authorization-server\ndocs: https://docs.wefunder.com/api-reference\nnotes: >-\n  Scope catalog derived from the public-tier OpenAPI and confirmed against the live\n  RFC 8414 authorization-server metadata (saved at\n  well-known/wefunder-oauth-authorization-server.json), which advertises\n  scopes_supported [read:syndicates, read:profile], PKCE S256, authorization_code +\n  refresh_token grants, and a dynamic client registration endpoint\n  (https://wefunder.com/oauth/register). client_credentials tokens may only hold\n  read:public. Attribution scopes are tiered (0 aggregate, 1 anonymized - approval\n  required, 2 full PII - founders only, 3 admin).\nschemes:\n- name: bearerAuth\n  source: openapi/wefunder-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wefunder.com/oauth/authorize\n    tokenUrl: https://wefunder.com/oauth/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://wefunder.com/oauth/token\n  description: OAuth 2.0 authorization with access tokens\nscopes:\n- scope: admin:attribution\n  description: Administrative access to attribution system (Tier 3 - Wefunder admins only)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: read:attribution:aggregate\n  description: Read aggregate attribution statistics (Tier 0)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: read:attribution:anonymized\n  description: Read anonymized attribution data (Tier 1 - requires approval)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: read:attribution:full\n  description: Read full attribution data with investor PII (Tier 2 - founders only)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: read:campaigns\n  description: Read campaign\
  \ information for companies you founded\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: read:investments\n  description: Read user investment data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: read:offerings\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: read:profile\n  description: Read user profile information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: read:public\n  description: Read public deal data (explore offerings); requires no user context\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: read:spvs\n  description: View partner SPVs, their invites, sessions, and investments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: read:syndicates\n  description: View syndicates, members, deals, and\
  \ portfolio\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: read:webhooks\n  description: View webhook subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: write:profile\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: write:spvs\n  description: Create and manage partner SPVs, invites, and investment sessions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: write:syndicates\n  description: Manage members, update settings, operate on deals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n- scope: write:webhooks\n  description: Create, update, and delete webhook subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wefunder-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/scopes/wefunder-scopes.yml
summary_line: 16 scopes · authorizationCode/clientCredentials
tags:
- Company
- Crowdfunding
- Equity Crowdfunding
- Investing
- Fintech
- Startups
- Fundraising
- Syndicates
- Regulation Crowdfunding
token_urls:
- https://wefunder.com/oauth/token
---
