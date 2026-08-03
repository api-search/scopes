---
api_specs:
- filename: 401go-openapi-original.json
  format: json
  label: 401GO API
  slug: 401go-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/openapi/401go-openapi-original.json
authorization_urls:
- https://app.401go.com/api/o/authorize
description: ''
docs: https://developer.401go.com/docs/authentication
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: 401Go Scopes
name_suffix: OAuth Scopes
note: 'The published OpenAPI declares its OAuth surface as an http/bearer scheme rather than an oauth2 scheme, so the mechanical derive pass finds no scopes. The real authorization server metadata is published at app.401go.com/api/o/.well-known/openid-configuration, and the scopes below are its verbatim scopes_supported list. 401GO layers a second, non-OAuth authorization control on top: a per-client endpoint + HTTP-method allow list negotiated at onboarding, documented at https://developer.401go.com/docs/api-endpoint-and-method-access. Holding a scope is therefore necessary but not sufficient — an unlisted endpoint/method returns 403.'
overview: '401GO publishes 12 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the 401GO API on a user''s behalf.


  Tokens are issued from https://app.401go.com/api/o/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 401GO
provider_slug: 401go
schemes:
- access_token_lifetime: 3600
  flows:
  - authorizationUrl: https://app.401go.com/api/o/authorize
    code_challenge_methods:
    - plain
    - S256
    flow: authorizationCode
    pkce: true
    tokenUrl: https://app.401go.com/api/o/token
  - docs: https://developer.401go.com/docs/client-credentials-flow
    flow: clientCredentials
    note: restricted to approved partners; credentials distributed by secure email
    tokenUrl: https://app.401go.com/api/o/token
  name: oauth2
  refresh_token_lifetime: 2592000
  source: https://app.401go.com/api/o/.well-known/openid-configuration
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
scope_count: 12
scope_names:
- openid
- participant:read
- participant:write
- participant:billing
- company:read
- company:write
- plan:read
- plan:write
- affiliate_firm:read
- affiliate_firm:write
- affiliate:read
- affiliate:write
scopes:
- description: OpenID Connect SSO. By default grants access to employee (participant) identity only; pair with company:read to use SSO for a company admin.
  flows:
  - authorizationCode
  scope: openid
- description: Read participant (employee) data — census record, deferrals, totals, portfolio, beneficiaries, loans, disbursements, rollovers, notifications, documents.
  flows:
  - authorizationCode
  - clientCredentials
  scope: participant:read
- description: Create and update participant data — participant records, deferral elections, beneficiaries, portfolio allocations, loan and disbursement and rollover requests.
  flows:
  - authorizationCode
  - clientCredentials
  scope: participant:write
- description: Access participant billing-related data.
  flows:
  - authorizationCode
  - clientCredentials
  scope: participant:billing
- description: Read company data — company list, plan provisions, employer match formulas, investment options, company affiliates, participant census.
  flows:
  - authorizationCode
  - clientCredentials
  scope: company:read
- description: Write company-scoped data, including payroll submission.
  flows:
  - authorizationCode
  - clientCredentials
  scope: company:write
- description: Read 401(k) plan configuration.
  flows:
  - authorizationCode
  - clientCredentials
  scope: plan:read
- description: Create and update 401(k) plans via the plan-setup endpoints.
  flows:
  - authorizationCode
  - clientCredentials
  scope: plan:write
- description: Read affiliate firm data — affiliates, fund lineups, pooled plans, pricing tiers.
  flows:
  - authorizationCode
  - clientCredentials
  scope: affiliate_firm:read
- description: Write affiliate firm data.
  flows:
  - authorizationCode
  - clientCredentials
  scope: affiliate_firm:write
- description: Read individual affiliate (advisor) data, including pricing tiers.
  flows:
  - authorizationCode
  - clientCredentials
  scope: affiliate:read
- description: Write individual affiliate (advisor) data.
  flows:
  - authorizationCode
  - clientCredentials
  scope: affiliate:write
slug: 401go-scopes
source_filename: 401go-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://app.401go.com/api/o/.well-known/openid-configuration\ndocs: https://developer.401go.com/docs/authentication\nnote: >-\n  The published OpenAPI declares its OAuth surface as an http/bearer scheme rather than an\n  oauth2 scheme, so the mechanical derive pass finds no scopes. The real authorization server\n  metadata is published at app.401go.com/api/o/.well-known/openid-configuration, and the\n  scopes below are its verbatim scopes_supported list. 401GO layers a second, non-OAuth\n  authorization control on top: a per-client endpoint + HTTP-method allow list negotiated at\n  onboarding, documented at\n  https://developer.401go.com/docs/api-endpoint-and-method-access. Holding a scope is\n  therefore necessary but not sufficient — an unlisted endpoint/method returns 403.\nissuer: https://app.401go.com/api/o\nschemes:\n- name: oauth2\n  source: https://app.401go.com/api/o/.well-known/openid-configuration\n  flows:\n  -\
  \ flow: authorizationCode\n    authorizationUrl: https://app.401go.com/api/o/authorize\n    tokenUrl: https://app.401go.com/api/o/token\n    pkce: true\n    code_challenge_methods: [plain, S256]\n  - flow: clientCredentials\n    tokenUrl: https://app.401go.com/api/o/token\n    docs: https://developer.401go.com/docs/client-credentials-flow\n    note: restricted to approved partners; credentials distributed by secure email\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n  access_token_lifetime: 3600\n  refresh_token_lifetime: 2592000\nscopes:\n- scope: openid\n  description: OpenID Connect SSO. By default grants access to employee (participant)\n    identity only; pair with company:read to use SSO for a company admin.\n  flows: [authorizationCode]\n  sources: [openid-configuration, docs]\n- scope: participant:read\n  description: Read participant (employee) data — census record, deferrals, totals,\n    portfolio, beneficiaries, loans, disbursements, rollovers,\
  \ notifications, documents.\n  flows: [authorizationCode, clientCredentials]\n  sources: [openid-configuration, docs]\n- scope: participant:write\n  description: Create and update participant data — participant records, deferral elections,\n    beneficiaries, portfolio allocations, loan and disbursement and rollover requests.\n  flows: [authorizationCode, clientCredentials]\n  sources: [openid-configuration, docs]\n- scope: participant:billing\n  description: Access participant billing-related data.\n  flows: [authorizationCode, clientCredentials]\n  sources: [openid-configuration]\n- scope: company:read\n  description: Read company data — company list, plan provisions, employer match formulas,\n    investment options, company affiliates, participant census.\n  flows: [authorizationCode, clientCredentials]\n  sources: [openid-configuration, docs]\n- scope: company:write\n  description: Write company-scoped data, including payroll submission.\n  flows: [authorizationCode, clientCredentials]\n\
  \  sources: [openid-configuration]\n- scope: plan:read\n  description: Read 401(k) plan configuration.\n  flows: [authorizationCode, clientCredentials]\n  sources: [openid-configuration]\n- scope: plan:write\n  description: Create and update 401(k) plans via the plan-setup endpoints.\n  flows: [authorizationCode, clientCredentials]\n  sources: [openid-configuration]\n- scope: affiliate_firm:read\n  description: Read affiliate firm data — affiliates, fund lineups, pooled plans, pricing tiers.\n  flows: [authorizationCode, clientCredentials]\n  sources: [openid-configuration]\n- scope: affiliate_firm:write\n  description: Write affiliate firm data.\n  flows: [authorizationCode, clientCredentials]\n  sources: [openid-configuration]\n- scope: affiliate:read\n  description: Read individual affiliate (advisor) data, including pricing tiers.\n  flows: [authorizationCode, clientCredentials]\n  sources: [openid-configuration]\n- scope: affiliate:write\n  description: Write individual affiliate\
  \ (advisor) data.\n  flows: [authorizationCode, clientCredentials]\n  sources: [openid-configuration]\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://app.401go.com/api/o/.well-known/openid-configuration\n  http_status: 200\n  scopes_found: 12\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/401go/refs/heads/main/scopes/401go-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials
tags:
- Company
- Retirement
- 401k
- Financial Services
- Fintech
- Payroll
- Human Resources
- Benefits
- Investments
- Wealth Management
token_urls:
- https://app.401go.com/api/o/token
---
