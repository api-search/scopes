---
api_specs:
- filename: azupay-api-keys-api-openapi.yml
  format: yaml
  label: Azupay API Keys API
  slug: azupay-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-api-keys-api-openapi.yml
- filename: azupay-billing-and-transaction-reports-api-openapi.yml
  format: yaml
  label: Azupay Billing and Transaction Reports API
  slug: azupay-billing-and-transaction-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-billing-and-transaction-reports-api-openapi.yml
- filename: azupay-check-accounts-api-openapi.yml
  format: yaml
  label: Azupay Check Accounts API
  slug: azupay-check-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-check-accounts-api-openapi.yml
- filename: azupay-clients-api-openapi.yml
  format: yaml
  label: Azupay Clients API
  slug: azupay-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-clients-api-openapi.yml
- filename: azupay-current-balances-api-openapi.yml
  format: yaml
  label: Azupay Current Balances API
  slug: azupay-current-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-current-balances-api-openapi.yml
- filename: azupay-payment-agreement-api-openapi.yml
  format: yaml
  label: Azupay Payment Agreement API
  slug: azupay-payment-agreement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-agreement-api-openapi.yml
- filename: azupay-payment-agreement-request-api-openapi.yml
  format: yaml
  label: Azupay Payment Agreement Request API
  slug: azupay-payment-agreement-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-agreement-request-api-openapi.yml
- filename: azupay-payment-api-openapi.yml
  format: yaml
  label: Azupay Payment API
  slug: azupay-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-api-openapi.yml
- filename: azupay-payment-initiation-api-openapi.yml
  format: yaml
  label: Azupay Payment Initiation API
  slug: azupay-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-initiation-api-openapi.yml
- filename: azupay-payment-request-api-openapi.yml
  format: yaml
  label: Azupay Payment Request API
  slug: azupay-payment-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-request-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.azupay.com.au/docs/oauth-20-api
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Azupay Scopes
name_suffix: OAuth Scopes
note: The REST OpenAPI declares only apiKey security. Docs document OAuth 2.0 client-credentials as an additional server-to-server option; the permitted scope set (oauth2AllowedScopes) is provisioned per client by Azupay and returned by the OAuth 2.0 connection-details endpoint (getClientOAuth2 / enableClientOAuth2) rather than published as a fixed public catalogue.
overview: 'Azupay publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azupay API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azupay
provider_slug: azupay
schemes:
- flow: clientCredentials
  grantType: client_credentials
  name: OAuth2ClientCredentials
  tokenType: JWT bearer
  tokenUrl: dynamic — returned as oauth2TokenUrl by POST /client/{clientId}/oauth2 (enableClientOAuth2)
  ttl: oauth2TtlInSecs (short-lived; token response carries expires_in)
scope_count: 1
scope_names:
- oauth2AllowedScopes
scopes:
- description: Per-client scope set enabling access to the specific Azupay REST endpoints agreed for the integration; exact scope names are provisioned and returned by Azupay, not published publicly.
  flows:
  - clientCredentials
  scope: oauth2AllowedScopes
slug: azupay-scopes
source_filename: azupay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/*.yml (no oauth2 in spec)\ndocs: https://developer.azupay.com.au/docs/oauth-20-api\nnote: The REST OpenAPI declares only apiKey security. Docs document OAuth 2.0 client-credentials as an\n  additional server-to-server option; the permitted scope set (oauth2AllowedScopes) is provisioned per\n  client by Azupay and returned by the OAuth 2.0 connection-details endpoint (getClientOAuth2 / enableClientOAuth2)\n  rather than published as a fixed public catalogue.\nschemes:\n- name: OAuth2ClientCredentials\n  flow: clientCredentials\n  tokenUrl: dynamic — returned as oauth2TokenUrl by POST /client/{clientId}/oauth2 (enableClientOAuth2)\n  grantType: client_credentials\n  tokenType: JWT bearer\n  ttl: oauth2TtlInSecs (short-lived; token response carries expires_in)\nscopes:\n- scope: oauth2AllowedScopes\n  description: Per-client scope set enabling access to the specific Azupay REST endpoints agreed for the\n    integration;\
  \ exact scope names are provisioned and returned by Azupay, not published publicly.\n  flows:\n  - clientCredentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/scopes/azupay-scopes.yml
summary_line: 1 scope
tags:
- Payments
- Australia
- Real-Time Payments
- Account-to-Account
- New Payments Platform
- PayID
- PayTo
- Money Transfer
- Confirmation of Payee
- Open Banking
token_urls: []
---
