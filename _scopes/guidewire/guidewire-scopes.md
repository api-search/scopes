---
api_specs:
- filename: guidewire-policycenter-openapi.yml
  format: yaml
  label: Guidewire PolicyCenter API
  slug: guidewire-policycenter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-policycenter-openapi.yml
- filename: guidewire-claimcenter-openapi.yml
  format: yaml
  label: Guidewire ClaimCenter API
  slug: guidewire-claimcenter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/openapi/guidewire-claimcenter-openapi.yml
- filename: guidewire-integration-gateway-asyncapi.yml
  format: yaml
  label: Guidewire Integration Gateway API
  slug: guidewire-integration-gateway-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/asyncapi/guidewire-integration-gateway-asyncapi.yml
authorization_urls:
- https://login.guidewire.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Guidewire Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Guidewire publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Guidewire API on a user''s behalf.


  Tokens are issued from https://login.guidewire.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Guidewire
provider_slug: guidewire
schemes:
- flows:
  - authorizationUrl: https://login.guidewire.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.guidewire.com/oauth/token
  name: OAuth2
  source: openapi/guidewire-claimcenter-openapi.yml
- flows:
  - authorizationUrl: https://login.guidewire.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://login.guidewire.com/oauth/token
  name: OAuth2
  source: openapi/guidewire-policycenter-openapi.yml
scope_count: 6
scope_names:
- cc.claims.read
- cc.claims.write
- cc.payments.write
- pc.accounts.read
- pc.policies.read
- pc.policies.write
scopes:
- description: Read claim data
  flows:
  - authorizationCode
  scope: cc.claims.read
- description: Create and update claims
  flows:
  - authorizationCode
  scope: cc.claims.write
- description: Create claim payments
  flows:
  - authorizationCode
  scope: cc.payments.write
- description: Read account data
  flows:
  - authorizationCode
  scope: pc.accounts.read
- description: Read policy data
  flows:
  - authorizationCode
  scope: pc.policies.read
- description: Write policy data
  flows:
  - authorizationCode
  scope: pc.policies.write
slug: guidewire-scopes
source_filename: guidewire-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/guidewire-claimcenter-openapi.yml, openapi/guidewire-policycenter-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/guidewire-claimcenter-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.guidewire.com/oauth/authorize\n    tokenUrl: https://login.guidewire.com/oauth/token\n- name: OAuth2\n  source: openapi/guidewire-policycenter-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.guidewire.com/oauth/authorize\n    tokenUrl: https://login.guidewire.com/oauth/token\nscopes:\n- scope: cc.claims.read\n  description: Read claim data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guidewire-claimcenter-openapi.yml\n- scope: cc.claims.write\n  description: Create and update claims\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guidewire-claimcenter-openapi.yml\n- scope: cc.payments.write\n  description: Create claim payments\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/guidewire-claimcenter-openapi.yml\n- scope: pc.accounts.read\n  description: Read account data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guidewire-policycenter-openapi.yml\n- scope: pc.policies.read\n  description: Read policy data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guidewire-policycenter-openapi.yml\n- scope: pc.policies.write\n  description: Write policy data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guidewire-policycenter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guidewire/refs/heads/main/scopes/guidewire-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Insurance
- Policy
- Claims
- Billing
- P&C
token_urls:
- https://login.guidewire.com/oauth/token
---
