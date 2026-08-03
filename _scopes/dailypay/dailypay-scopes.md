---
api_specs:
- filename: dailypay-rest-openapi-original.yml
  format: yaml
  label: DailyPay Rest API
  slug: dailypay-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-rest-openapi-original.yml
authorization_urls:
- https://auth.dailypay.com/oauth2/auth
description: ''
docs: https://developer.dailypay.com/products/rest/guides/auth
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Dailypay Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'DailyPay publishes 5 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the DailyPay API on a user''s behalf.


  Tokens are issued from https://auth.dailypay.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DailyPay
provider_slug: dailypay
schemes:
- audience: server-to-server / partner application
  docs: https://developer.dailypay.com/products/rest/guides/auth/client-credentials-flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.dailypay.com/oauth2/token
  name: oauth_client_credentials_token
  source: openapi/dailypay-rest-openapi-original.yml
- audience: end user (employee) acting through the partner application
  docs: https://developer.dailypay.com/products/rest/guides/auth/authorization-code-flow
  flows:
  - authorizationUrl: https://auth.dailypay.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://auth.dailypay.com/oauth2/token
  name: oauth_user_token
  pkce: true
  refresh: https://developer.dailypay.com/products/rest/guides/auth/refresh-token
  source: openapi/dailypay-rest-openapi-original.yml
scope_count: 5
scope_names:
- client:admin
- client:lookup
- health:read
- user:read
- user:read_write
scopes:
- description: Application-level administrative access. Applied as the default client-credentials requirement at the document level and on the read operations reachable with an application token.
  flows:
  - clientCredentials
  scope: client:admin
- description: Read access to resources necessary to find a person by known identifiers.
  flows:
  - clientCredentials
  scope: client:lookup
- description: Read access to the API health endpoint (GET /rest/health). Declared on the operation's security requirement; not enumerated in either scheme's flow scopes map.
  flows: []
  scope: health:read
- description: Read access to all relevant objects for a non-application user, including accounts, jobs, people, transfers, and paychecks.
  flows:
  - authorizationCode
  scope: user:read
- description: Read and write access to all relevant objects for a non-application user, including accounts, jobs, people, transfers, and paychecks. Required for createTransfer, createAccount, deleteAccount, updateJob and updatePerson.
  flows:
  - authorizationCode
  scope: user:read_write
slug: dailypay-scopes
source_filename: dailypay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/dailypay-rest-openapi-original.yml\ndocs: https://developer.dailypay.com/products/rest/guides/auth\ndiscovery: https://auth.dailypay.com/.well-known/openid-configuration\nnotes: >-\n  DailyPay scopes are not self-serve. The auth guide states that DailyPay provides the application's\n  configuration values — including \"scope: a list of scopes your application can request, which may\n  include offline_access and openid\" — during partner registration, so the set of scopes a given\n  client may request is provisioned per application rather than published as a catalogue. The\n  API-resource scopes below are the ones declared in the OpenAPI security schemes and applied to\n  operations; the OIDC scopes below are advertised by the live authorization-server discovery\n  document. No standalone scopes/permissions reference page is published.\nschemes:\n- name: oauth_client_credentials_token\n  source: openapi/dailypay-rest-openapi-original.yml\n\
  \  audience: server-to-server / partner application\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.dailypay.com/oauth2/token\n  docs: https://developer.dailypay.com/products/rest/guides/auth/client-credentials-flow\n- name: oauth_user_token\n  source: openapi/dailypay-rest-openapi-original.yml\n  audience: end user (employee) acting through the partner application\n  pkce: true\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.dailypay.com/oauth2/auth\n    tokenUrl: https://auth.dailypay.com/oauth2/token\n  docs: https://developer.dailypay.com/products/rest/guides/auth/authorization-code-flow\n  refresh: https://developer.dailypay.com/products/rest/guides/auth/refresh-token\nscopes:\n- scope: client:admin\n  description: >-\n    Application-level administrative access. Applied as the default client-credentials requirement\n    at the document level and on the read operations reachable with an application token.\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/dailypay-rest-openapi-original.yml\n- scope: client:lookup\n  description: Read access to resources necessary to find a person by known identifiers.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dailypay-rest-openapi-original.yml\n- scope: health:read\n  description: >-\n    Read access to the API health endpoint (GET /rest/health). Declared on the operation's security\n    requirement; not enumerated in either scheme's flow scopes map.\n  sources:\n  - openapi/dailypay-rest-openapi-original.yml\n- scope: user:read\n  description: >-\n    Read access to all relevant objects for a non-application user, including accounts, jobs,\n    people, transfers, and paychecks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dailypay-rest-openapi-original.yml\n- scope: user:read_write\n  description: >-\n    Read and write access to all relevant objects for a non-application user, including accounts,\n    jobs, people, transfers, and paychecks. Required\
  \ for createTransfer, createAccount,\n    deleteAccount, updateJob and updatePerson.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/dailypay-rest-openapi-original.yml\noidc_scopes:\n  source: https://auth.dailypay.com/.well-known/openid-configuration\n  supported:\n  - scope: openid\n    description: Standard OIDC scope; requests an ID token.\n  - scope: offline_access\n    description: Requests a refresh token so the application can refresh the user access token.\n  - scope: offline\n    description: Legacy alias advertised alongside offline_access by the authorization server.\ngranularity:\n  note: >-\n    Scope granularity is coarse. There is no per-resource scope family — a single user:read_write\n    scope grants write access to accounts, jobs, people and transfers alike, which means a token\n    obtained to add a bank account also carries the authority to move money. This is reflected in\n    agentic-access/dailypay-agentic-access.yml, where createTransfer is classified\
  \ as\n    physical-consequence under the same scope as low-risk profile updates.\ncoverage:\n  api_scopes: 5\n  oidc_scopes: 3\n  schemes: 2\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/scopes/dailypay-scopes.yml
summary_line: 5 scopes · clientCredentials/authorizationCode
tags:
- Company
- Payments
- Payroll
- Human Resources
- Earned Wage Access
- On-Demand Pay
- Financial Services
- Fintech
- Money Transfer
- Benefits
token_urls:
- https://auth.dailypay.com/oauth2/token
---
