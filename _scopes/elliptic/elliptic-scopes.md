---
api_specs:
- filename: elliptic-assets-api-openapi.yml
  format: yaml
  label: Elliptic Assets API
  slug: elliptic-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-assets-api-openapi.yml
- filename: elliptic-count-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Count Analyses API
  slug: elliptic-count-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-count-analyses-api-openapi.yml
- filename: elliptic-criteria-api-openapi.yml
  format: yaml
  label: Elliptic Criteria API
  slug: elliptic-criteria-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-criteria-api-openapi.yml
- filename: elliptic-customers-api-openapi.yml
  format: yaml
  label: Elliptic Customers API
  slug: elliptic-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-customers-api-openapi.yml
- filename: elliptic-health-api-openapi.yml
  format: yaml
  label: Elliptic Health API
  slug: elliptic-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-health-api-openapi.yml
- filename: elliptic-risk-rules-api-openapi.yml
  format: yaml
  label: Elliptic Risk Rules API
  slug: elliptic-risk-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-risk-rules-api-openapi.yml
- filename: elliptic-sanctions-api-openapi.yml
  format: yaml
  label: Elliptic Sanctions API
  slug: elliptic-sanctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-sanctions-api-openapi.yml
- filename: elliptic-screenings-api-openapi.yml
  format: yaml
  label: Elliptic Screenings API
  slug: elliptic-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-screenings-api-openapi.yml
- filename: elliptic-transaction-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Transaction Analyses API
  slug: elliptic-transaction-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-transaction-analyses-api-openapi.yml
- filename: elliptic-transaction-workflow-api-openapi.yml
  format: yaml
  label: Elliptic Transaction Workflow API
  slug: elliptic-transaction-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-transaction-workflow-api-openapi.yml
- filename: elliptic-tron-nodeintelligence-api-openapi.yml
  format: yaml
  label: Elliptic Tron NodeIntelligence API
  slug: elliptic-tron-nodeintelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-tron-nodeintelligence-api-openapi.yml
- filename: elliptic-users-api-openapi.yml
  format: yaml
  label: Elliptic Users API
  slug: elliptic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-users-api-openapi.yml
- filename: elliptic-wallet-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Analyses API
  slug: elliptic-wallet-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-analyses-api-openapi.yml
- filename: elliptic-wallet-analyses-count-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Analyses Count API
  slug: elliptic-wallet-analyses-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-analyses-count-api-openapi.yml
- filename: elliptic-wallet-api-openapi.yml
  format: yaml
  label: Elliptic Wallet API
  slug: elliptic-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-api-openapi.yml
- filename: elliptic-wallet-workflow-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Workflow API
  slug: elliptic-wallet-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-workflow-api-openapi.yml
authorization_urls:
- https://login.elliptic.co/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Elliptic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Elliptic publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Elliptic API on a user''s behalf.


  Tokens are issued from https://login.elliptic.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elliptic
provider_slug: elliptic
schemes:
- flows:
  - authorizationUrl: https://login.elliptic.co/authorize
    flow: authorizationCode
    tokenUrl: https://login.elliptic.co/oauth/token
  name: oauth2
  source: openapi/aml-api-oauth.json
scope_count: 2
scope_names:
- openid
- profile
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: openid
- description: ''
  flows:
  - authorizationCode
  scope: profile
slug: elliptic-scopes
source_filename: elliptic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aml-api-oauth.json\nschemes:\n- name: oauth2\n  source: openapi/aml-api-oauth.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.elliptic.co/authorize\n    tokenUrl: https://login.elliptic.co/oauth/token\nscopes:\n- scope: openid\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aml-api-oauth.json\n- scope: profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aml-api-oauth.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/scopes/elliptic-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Blockchain
- Crypto
- Compliance
- AML
- Transaction Screening
- Wallet Screening
- Risk Scoring
- Analytics
token_urls:
- https://login.elliptic.co/oauth/token
---
