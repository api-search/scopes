---
authorization_urls: []
description: ''
docs: https://docs.solarisgroup.com/api-reference/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Solaris Scopes
name_suffix: OAuth Scopes
note: Solaris uses OAuth2 client-credentials with a single documented access scope ("partners"). Fine-grained access is not expressed as OAuth scopes but as per-partner "policies" granted by the Solaris Partner Manager per product and use case (see permissions_model in authentication/). This file records the one published OAuth scope; the policy-based permission grants are not self-service and are not enumerated in public docs.
overview: 'Solaris publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Solaris API on a user''s behalf.


  Tokens are issued from https://auth.solarisbank.de/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Solaris
provider_slug: solaris
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.solarisbank.de/oauth2/token
  name: OAuth2
  source: https://docs.solarisgroup.com/api-reference/authentication
scope_count: 1
scope_names:
- partners
scopes:
- description: Required scope for standard partner API access.
  flows:
  - clientCredentials
  scope: partners
slug: solaris-scopes
source_filename: solaris-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.solarisgroup.com/api-reference/authentication\ndocs: https://docs.solarisgroup.com/api-reference/authentication\nnote: >-\n  Solaris uses OAuth2 client-credentials with a single documented access scope\n  (\"partners\"). Fine-grained access is not expressed as OAuth scopes but as\n  per-partner \"policies\" granted by the Solaris Partner Manager per product and\n  use case (see permissions_model in authentication/). This file records the\n  one published OAuth scope; the policy-based permission grants are not\n  self-service and are not enumerated in public docs.\nschemes:\n  - name: OAuth2\n    source: https://docs.solarisgroup.com/api-reference/authentication\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://auth.solarisbank.de/oauth2/token\nscopes:\n  - scope: partners\n    description: Required scope for standard partner API access.\n    flows: [clientCredentials]\n    sources: [https://docs.solarisgroup.com/api-reference/authentication]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solaris/refs/heads/main/scopes/solaris-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Fintech
- Banking
- Banking as a Service
- Embedded Finance
- Payments
- SEPA
- Cards
- KYC
- Lending
- Compliance
- OAuth2
- Webhooks
- Germany
token_urls:
- https://auth.solarisbank.de/oauth2/token
---
