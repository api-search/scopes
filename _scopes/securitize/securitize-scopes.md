---
api_specs:
- filename: securitize-apac-api-openapi.yml
  format: yaml
  label: Securitize APAC API
  slug: securitize-apac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-apac-api-openapi.yml
- filename: securitize-domains-api-openapi.yml
  format: yaml
  label: Securitize Domains API
  slug: securitize-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-domains-api-openapi.yml
- filename: securitize-health-check-api-openapi.yml
  format: yaml
  label: Securitize Health Check API
  slug: securitize-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-health-check-api-openapi.yml
- filename: securitize-travel-rule-api-openapi.yml
  format: yaml
  label: Securitize Travel Rule API
  slug: securitize-travel-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-travel-rule-api-openapi.yml
- filename: securitize-webhooks-api-openapi.yml
  format: yaml
  label: Securitize Webhooks API
  slug: securitize-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-webhooks-api-openapi.yml
authorization_urls: []
description: The Securitize Connect API is an OAuth provider for Securitize iD. Scopes are passed as a space-delimited `scope` query parameter on the authorize redirect and govern what investor data a partner may read once the investor signs the data-share agreement. The docs state only three scopes are currently supported. The Domains API is a separate surface and uses API-key auth with no scopes — see authentication/securitize-authentication.yml.
docs: https://sec-connect-api-docs.securitize.io/scope-of-access
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Securitize Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Securitize publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Securitize API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Securitize
provider_slug: securitize
schemes:
- authorization_code_ttl: 5 minutes
  authorization_url: https://id.securitize.io/#/authorize
  client_id_param: issuerId
  flow: authorization-code-like
  name: SecuritizeID OAuth
  redirect_allowlist_required: true
  redirect_param: redirecturl
  refresh_url: https://sec-id-api.securitize.io/v1/{clientId}/oauth2/refresh
  source: https://sec-connect-api-docs.securitize.io/authentication-1/authentication
  token_url: https://sec-id-api.securitize.io/v1/{clientId}/oauth2/authorize
  type: oauth2
scope_count: 3
scope_names:
- info
- details
- verification
scopes:
- description: Basic investor information — the identity fields the investor agreed to share with the partner application.
  flows: []
  scope: info
- description: Extended investor detail, including entity and legal-signer information where applicable.
  flows: []
  scope: details
- description: Investor verification state and verification details — KYC/KYB/AML status and the supporting verification records.
  flows: []
  scope: verification
slug: securitize-scopes
source_filename: securitize-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://sec-connect-api-docs.securitize.io/authentication-1/authentication\ndocs: https://sec-connect-api-docs.securitize.io/scope-of-access\napi: Securitize Connect API (Securitize iD)\ndescription: >-\n  The Securitize Connect API is an OAuth provider for Securitize iD. Scopes are passed as a space-delimited\n  `scope` query parameter on the authorize redirect and govern what investor data a partner may read once the\n  investor signs the data-share agreement. The docs state only three scopes are currently supported. The Domains\n  API is a separate surface and uses API-key auth with no scopes — see authentication/securitize-authentication.yml.\nschemes:\n- name: SecuritizeID OAuth\n  type: oauth2\n  flow: authorization-code-like\n  authorization_url: https://id.securitize.io/#/authorize\n  token_url: https://sec-id-api.securitize.io/v1/{clientId}/oauth2/authorize\n  refresh_url: https://sec-id-api.securitize.io/v1/{clientId}/oauth2/refresh\n\
  \  client_id_param: issuerId\n  redirect_param: redirecturl\n  redirect_allowlist_required: true\n  authorization_code_ttl: 5 minutes\n  source: https://sec-connect-api-docs.securitize.io/authentication-1/authentication\nscopes:\n- scope: info\n  description: >-\n    Basic investor information — the identity fields the investor agreed to share with the partner application.\n  sources:\n  - https://sec-connect-api-docs.securitize.io/authentication-1/authentication\n- scope: details\n  description: Extended investor detail, including entity and legal-signer information where applicable.\n  sources:\n  - https://sec-connect-api-docs.securitize.io/authentication-1/authentication\n- scope: verification\n  description: >-\n    Investor verification state and verification details — KYC/KYB/AML status and the supporting verification\n    records.\n  sources:\n  - https://sec-connect-api-docs.securitize.io/authentication-1/authentication\n  - https://sec-connect-api-docs.securitize.io/verification-details\n\
  notes:\n- >-\n  Scope of access is additionally governed by the commercial agreement between Securitize iD and the third-party\n  integrator, not by the scope string alone (see the Scope of Access page).\n- >-\n  The three scopes are enumerated in prose in the authentication docs (\"we currently only support\n  `info details verification`\"). Securitize publishes no OpenAPI oauth2 securityScheme and no scopes reference\n  table, so there is no machine-readable source for this list.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://sec-connect-api-docs.securitize.io/authentication-1/authentication.md\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/scopes/securitize-scopes.yml
summary_line: 3 scopes
tags:
- tokenization
- digital-securities
- real-world-assets
- capital-markets
- fund-administration
- transfer-agent
- kyc
- aml
- identity-verification
- blockchain
- broker-dealer
- private-credit
- mcp
- webhooks
token_urls: []
---
