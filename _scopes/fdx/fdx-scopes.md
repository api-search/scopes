---
authorization_urls:
- https://www.your-organization.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Fdx Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Financial Data Exchange (FDX) publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Financial Data Exchange (FDX) API on a user''s behalf.


  Tokens are issued from https://www.your-organization.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Financial Data Exchange (FDX)
provider_slug: fdx
schemes:
- description: 'This API uses an [OAuth2.0 authorization code flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow) and accepts the resulting access token as a bearer token. For example,  `curl -H ''Authorization: Bearer <ACCESS&#95;TOKEN|''`.'
  flows:
  - authorizationUrl: https://www.your-organization.com/authorize
    flow: authorizationCode
    tokenUrl: https://www.your-organization.com/token
  name: oauth2
  source: openapi/fdx-corex-6.0.0.yaml
- description: 'This API uses an [OAuth2.0 authorization code flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow) and accepts the resulting access token as a bearer token. For example,  `curl -H ''Authorization: Bearer <ACCESS&#95;TOKEN|''`.'
  flows:
  - authorizationUrl: https://www.your-organization.com/authorize
    flow: authorizationCode
    tokenUrl: https://www.your-organization.com/token
  name: oauth2
  source: openapi/fdx-corex-6.2.0.yaml
- description: 'This API uses an [OAuth2.0 authorization code flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow) and accepts the resulting access token as a bearer token. For example,  `curl -H ''Authorization: Bearer <ACCESS&#95;TOKEN|''`.'
  flows:
  - authorizationUrl: https://www.your-organization.com/authorize
    flow: authorizationCode
    tokenUrl: https://www.your-organization.com/token
  name: oauth2
  source: openapi/fdx-corex-6.3.1.yaml
scope_count: 3
scope_names:
- Account
- Customer
- Transactions
scopes:
- description: (optional) Read account data
  flows:
  - authorizationCode
  scope: Account
- description: (optional) Read customer data
  flows:
  - authorizationCode
  scope: Customer
- description: (optional) Read transaction data
  flows:
  - authorizationCode
  scope: Transactions
slug: fdx-scopes
source_filename: fdx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fdx-corex-6.0.0.yaml, openapi/fdx-corex-6.2.0.yaml, openapi/fdx-corex-6.3.1.yaml\nschemes:\n- name: oauth2\n  source: openapi/fdx-corex-6.0.0.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.your-organization.com/authorize\n    tokenUrl: https://www.your-organization.com/token\n  description: 'This API uses an [OAuth2.0 authorization code flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow)\n    and accepts the resulting access token as a bearer token. For example,  `curl -H ''Authorization:\n    Bearer <ACCESS&#95;TOKEN|''`.'\n- name: oauth2\n  source: openapi/fdx-corex-6.2.0.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.your-organization.com/authorize\n    tokenUrl: https://www.your-organization.com/token\n  description: 'This API uses an [OAuth2.0 authorization code flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow)\n\
  \    and accepts the resulting access token as a bearer token. For example,  `curl -H ''Authorization:\n    Bearer <ACCESS&#95;TOKEN|''`.'\n- name: oauth2\n  source: openapi/fdx-corex-6.3.1.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.your-organization.com/authorize\n    tokenUrl: https://www.your-organization.com/token\n  description: 'This API uses an [OAuth2.0 authorization code flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/authorization-code-flow)\n    and accepts the resulting access token as a bearer token. For example,  `curl -H ''Authorization:\n    Bearer <ACCESS&#95;TOKEN|''`.'\nscopes:\n- scope: Account\n  description: (optional) Read account data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fdx-corex-6.0.0.yaml\n  - openapi/fdx-corex-6.2.0.yaml\n  - openapi/fdx-corex-6.3.1.yaml\n- scope: Customer\n  description: (optional) Read customer data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fdx-corex-6.0.0.yaml\n\
  \  - openapi/fdx-corex-6.2.0.yaml\n  - openapi/fdx-corex-6.3.1.yaml\n- scope: Transactions\n  description: (optional) Read transaction data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fdx-corex-6.0.0.yaml\n  - openapi/fdx-corex-6.2.0.yaml\n  - openapi/fdx-corex-6.3.1.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fdx/refs/heads/main/scopes/fdx-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Financial Data
- Open Banking
- Open Finance
- Financial Data Exchange
- Consumer Permissioned
- Account Data
- Transactions
- Investments
- Insurance
- Tax Data
- Payroll
- REST
- OAuth2
- FAPI
- CFPB 1033
token_urls:
- https://www.your-organization.com/token
---
