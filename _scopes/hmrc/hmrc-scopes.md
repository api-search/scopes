---
authorization_urls:
- https://api.service.hmrc.gov.uk/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Hmrc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HMRC UK Tax Authority publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HMRC UK Tax Authority API on a user''s behalf.


  Tokens are issued from https://api.service.hmrc.gov.uk/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HMRC UK Tax Authority
provider_slug: hmrc
schemes:
- description: HMRC OAuth 2.0 Authorization Code grant (user-restricted)
  flows:
  - authorizationUrl: https://api.service.hmrc.gov.uk/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.service.hmrc.gov.uk/oauth/token
  name: OAuth2UserRestricted
  source: openapi/hmrc-vat-mtd-openapi.yml
scope_count: 2
scope_names:
- read:vat
- write:vat
scopes:
- description: Read VAT data
  flows:
  - authorizationCode
  scope: read:vat
- description: Submit VAT returns
  flows:
  - authorizationCode
  scope: write:vat
slug: hmrc-scopes
source_filename: hmrc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hmrc-vat-mtd-openapi.yml\nschemes:\n- name: OAuth2UserRestricted\n  source: openapi/hmrc-vat-mtd-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.service.hmrc.gov.uk/oauth/authorize\n    tokenUrl: https://api.service.hmrc.gov.uk/oauth/token\n  description: HMRC OAuth 2.0 Authorization Code grant (user-restricted)\nscopes:\n- scope: read:vat\n  description: Read VAT data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hmrc-vat-mtd-openapi.yml\n- scope: write:vat\n  description: Submit VAT returns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hmrc-vat-mtd-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hmrc/refs/heads/main/scopes/hmrc-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Government
- Making Tax Digital
- Regulatory
- Tax
- UK
token_urls:
- https://api.service.hmrc.gov.uk/oauth/token
---
