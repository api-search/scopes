---
api_specs:
- filename: hedgespecialty-com-account-api-openapi.yml
  format: yaml
  label: Hedge Account API
  slug: hedgespecialty-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-account-api-openapi.yml
- filename: hedgespecialty-com-appetite-api-openapi.yml
  format: yaml
  label: Hedge Appetite API
  slug: hedgespecialty-com-appetite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-appetite-api-openapi.yml
- filename: hedgespecialty-com-auth-api-openapi.yml
  format: yaml
  label: Hedge Auth API
  slug: hedgespecialty-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-auth-api-openapi.yml
- filename: hedgespecialty-com-binding-api-openapi.yml
  format: yaml
  label: Hedge Binding API
  slug: hedgespecialty-com-binding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-binding-api-openapi.yml
- filename: hedgespecialty-com-carrier-quotes-api-openapi.yml
  format: yaml
  label: Hedge Carrier quotes API
  slug: hedgespecialty-com-carrier-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-carrier-quotes-api-openapi.yml
- filename: hedgespecialty-com-documents-api-openapi.yml
  format: yaml
  label: Hedge Documents API
  slug: hedgespecialty-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-documents-api-openapi.yml
- filename: hedgespecialty-com-market-access-api-openapi.yml
  format: yaml
  label: Hedge Market access API
  slug: hedgespecialty-com-market-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-market-access-api-openapi.yml
- filename: hedgespecialty-com-payments-api-openapi.yml
  format: yaml
  label: Hedge Payments API
  slug: hedgespecialty-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-payments-api-openapi.yml
- filename: hedgespecialty-com-policies-api-openapi.yml
  format: yaml
  label: Hedge Policies API
  slug: hedgespecialty-com-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-policies-api-openapi.yml
- filename: hedgespecialty-com-programs-api-openapi.yml
  format: yaml
  label: Hedge Programs API
  slug: hedgespecialty-com-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-programs-api-openapi.yml
- filename: hedgespecialty-com-requirements-api-openapi.yml
  format: yaml
  label: Hedge Requirements API
  slug: hedgespecialty-com-requirements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-requirements-api-openapi.yml
- filename: hedgespecialty-com-submissions-api-openapi.yml
  format: yaml
  label: Hedge Submissions API
  slug: hedgespecialty-com-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-submissions-api-openapi.yml
- filename: hedgespecialty-com-webhooks-api-openapi.yml
  format: yaml
  label: Hedge Webhooks API
  slug: hedgespecialty-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-webhooks-api-openapi.yml
authorization_urls:
- https://api.hedgespecialty.com/api/v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Hedgespecialty Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hedge publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hedge API on a user''s behalf.


  Tokens are issued from https://api.hedgespecialty.com/api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hedge
provider_slug: hedgespecialty-com
schemes:
- description: 'Broker access token. Scopes: `broker_mcp` (read), `broker_submit`

    (write). Per-user tokens come from the OAuth authorization-code +

    PKCE flow (`/oauth/authorize` → `/oauth/token`); machine tokens

    from `client_credentials`, using an API key created self-serve in

    the broker portal (Settings → API keys) or issued by Hedge ops.

    Access tokens live 60 minutes.'
  flows:
  - authorizationUrl: https://api.hedgespecialty.com/api/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hedgespecialty.com/api/v1/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.hedgespecialty.com/api/v1/oauth/token
  name: brokerOAuth
  source: openapi/hedgespecialty-com-openapi.yml
scope_count: 2
scope_names:
- broker_mcp
- broker_submit
scopes:
- description: Read brokerage-scoped submissions, policies, payments, appetite, and requirements.
  flows:
  - authorizationCode
  - clientCredentials
  scope: broker_mcp
- description: Create submissions, answer Hedge's asks, and act on quotes for your brokerage.
  flows:
  - authorizationCode
  - clientCredentials
  scope: broker_submit
slug: hedgespecialty-com-scopes
source_filename: hedgespecialty-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/hedgespecialty-com-openapi.yml\nschemes:\n- name: brokerOAuth\n  source: openapi/hedgespecialty-com-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.hedgespecialty.com/api/v1/oauth/authorize\n    tokenUrl: https://api.hedgespecialty.com/api/v1/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.hedgespecialty.com/api/v1/oauth/token\n  description: |-\n    Broker access token. Scopes: `broker_mcp` (read), `broker_submit`\n    (write). Per-user tokens come from the OAuth authorization-code +\n    PKCE flow (`/oauth/authorize` → `/oauth/token`); machine tokens\n    from `client_credentials`, using an API key created self-serve in\n    the broker portal (Settings → API keys) or issued by Hedge ops.\n    Access tokens live 60 minutes.\nscopes:\n- scope: broker_mcp\n  description: Read brokerage-scoped submissions, policies, payments, appetite, and requirements.\n  flows:\n\
  \  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/hedgespecialty-com-openapi.yml\n- scope: broker_submit\n  description: Create submissions, answer Hedge's asks, and act on quotes for your brokerage.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/hedgespecialty-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/hedgespecialty-com/scopes/hedgespecialty-com-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Company
- Insurance
- Wholesale
- Brokers
- Specialty
token_bound: false
token_urls:
- https://api.hedgespecialty.com/api/v1/oauth/token
---
