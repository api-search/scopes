---
api_specs:
- filename: nift-partners-openapi.yml
  format: yaml
  label: Nift Partners API
  slug: nift-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nift/refs/heads/main/openapi/nift-partners-openapi.yml
authorization_urls: []
description: ''
docs: https://github.com/nift-sdks/nift-flow-sdk-docs/blob/main/docs/sdk/customer-status-server.md
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Nift Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NIFT publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the NIFT API on a user''s behalf.


  Tokens are issued from https://www.gonift.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NIFT
provider_slug: nift
schemes:
- description: OAuth 2.0 client credentials issued by Nift; token endpoint at /oauth/token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://www.gonift.com/oauth/token
  name: oauth2
  source: openapi/nift-partners-openapi.yml
scope_count: 2
scope_names:
- read:customers
- write:customers
scopes:
- description: Read access to customer status.
  flows:
  - clientCredentials
  scope: read:customers
- description: Submit customer deletion (anonymization) requests.
  flows:
  - clientCredentials
  scope: write:customers
slug: nift-scopes
source_filename: nift-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nift-partners-openapi.yml\ndocs: https://github.com/nift-sdks/nift-flow-sdk-docs/blob/main/docs/sdk/customer-status-server.md\nschemes:\n- name: oauth2\n  source: openapi/nift-partners-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.gonift.com/oauth/token\n  description: OAuth 2.0 client credentials issued by Nift; token endpoint at /oauth/token.\nscopes:\n- scope: read:customers\n  description: Read access to customer status.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/nift-partners-openapi.yml\n- scope: write:customers\n  description: Submit customer deletion (anonymization) requests.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/nift-partners-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nift/refs/heads/main/scopes/nift-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Marketing
- Gifting
- Customer Acquisition
- Loyalty
- Rewards
- SDK
- Partners
token_urls:
- https://www.gonift.com/oauth/token
---
