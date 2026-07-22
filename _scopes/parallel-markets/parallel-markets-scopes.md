---
authorization_urls:
- https://api.parallelmarkets.com/v1/oauth/authorize
description: ''
docs: https://developer.parallelmarkets.com/docs/1.x/server/scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Parallel Markets Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Parallel Markets publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Parallel Markets API on a user''s behalf.


  Tokens are issued from https://api.parallelmarkets.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Parallel Markets
provider_slug: parallel-markets
schemes:
- flows:
  - authorizationUrl: https://api.parallelmarkets.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.parallelmarkets.com/v1/oauth/token
  name: oauth2AuthorizationCode
  type: oauth2
scope_count: 4
scope_names:
- profile
- accreditation_status
- identity
- blockchain
scopes:
- description: Access to the Profile API and basic information about an individual or business. This scope should always be included.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the Accreditations API and the full accreditation history for an individual or business.
  flows:
  - authorizationCode
  scope: accreditation_status
- description: Access to the Identity API and detailed KYC/AML data, contact information, identity documents, and Taxpayer Identification Certification (W-9).
  flows:
  - authorizationCode
  scope: identity
- description: Access to the Blockchain API and information about confirmed wallets and Parallel Identity (PID) Token ownership.
  flows:
  - authorizationCode
  scope: blockchain
slug: parallel-markets-scopes
source_filename: parallel-markets-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.parallelmarkets.com/docs/1.x/server/scopes\ndocs: https://developer.parallelmarkets.com/docs/1.x/server/scopes\nschemes:\n- name: oauth2AuthorizationCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.parallelmarkets.com/v1/oauth/authorize\n    tokenUrl: https://api.parallelmarkets.com/v1/oauth/token\nscopes:\n- scope: profile\n  description: >-\n    Access to the Profile API and basic information about an individual or business.\n    This scope should always be included.\n  flows: [authorizationCode]\n- scope: accreditation_status\n  description: >-\n    Access to the Accreditations API and the full accreditation history for an\n    individual or business.\n  flows: [authorizationCode]\n- scope: identity\n  description: >-\n    Access to the Identity API and detailed KYC/AML data, contact information,\n    identity documents, and Taxpayer Identification Certification\
  \ (W-9).\n  flows: [authorizationCode]\n- scope: blockchain\n  description: >-\n    Access to the Blockchain API and information about confirmed wallets and\n    Parallel Identity (PID) Token ownership.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel-markets/refs/heads/main/scopes/parallel-markets-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Identity
- Identity Verification
- KYC
- AML
- Accreditation
- Compliance
- Financial Services
- Onboarding
- Investor Verification
- Webhooks
token_urls:
- https://api.parallelmarkets.com/v1/oauth/token
---
