---
api_specs:
- filename: bokio-authorization-api-openapi.yml
  format: yaml
  label: Bokio authorization API
  slug: bokio-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-authorization-api-openapi.yml
- filename: bokio-bank-payments-api-openapi.yml
  format: yaml
  label: Bokio bank-payments API
  slug: bokio-bank-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-bank-payments-api-openapi.yml
- filename: bokio-chart-of-accounts-api-openapi.yml
  format: yaml
  label: Bokio chart-of-accounts API
  slug: bokio-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-chart-of-accounts-api-openapi.yml
- filename: bokio-company-information-api-openapi.yml
  format: yaml
  label: Bokio company-information API
  slug: bokio-company-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-company-information-api-openapi.yml
- filename: bokio-connections-api-openapi.yml
  format: yaml
  label: Bokio connections API
  slug: bokio-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-connections-api-openapi.yml
- filename: bokio-credit-notes-api-openapi.yml
  format: yaml
  label: Bokio credit-notes API
  slug: bokio-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-credit-notes-api-openapi.yml
- filename: bokio-customers-api-openapi.yml
  format: yaml
  label: Bokio customers API
  slug: bokio-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-customers-api-openapi.yml
- filename: bokio-fiscal-years-api-openapi.yml
  format: yaml
  label: Bokio fiscal-years API
  slug: bokio-fiscal-years-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-fiscal-years-api-openapi.yml
- filename: bokio-invoices-api-openapi.yml
  format: yaml
  label: Bokio invoices API
  slug: bokio-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-invoices-api-openapi.yml
- filename: bokio-items-api-openapi.yml
  format: yaml
  label: Bokio items API
  slug: bokio-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-items-api-openapi.yml
- filename: bokio-journal-entries-api-openapi.yml
  format: yaml
  label: Bokio journal-entries API
  slug: bokio-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-journal-entries-api-openapi.yml
- filename: bokio-sie-files-api-openapi.yml
  format: yaml
  label: Bokio sie-files API
  slug: bokio-sie-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-sie-files-api-openapi.yml
- filename: bokio-supplier-invoices-api-openapi.yml
  format: yaml
  label: Bokio supplier-invoices API
  slug: bokio-supplier-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-supplier-invoices-api-openapi.yml
- filename: bokio-suppliers-api-openapi.yml
  format: yaml
  label: Bokio suppliers API
  slug: bokio-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-suppliers-api-openapi.yml
- filename: bokio-tag-groups-api-openapi.yml
  format: yaml
  label: Bokio tag-groups API
  slug: bokio-tag-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-tag-groups-api-openapi.yml
- filename: bokio-uploads-api-openapi.yml
  format: yaml
  label: Bokio uploads API
  slug: bokio-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-uploads-api-openapi.yml
authorization_urls:
- /authorize
description: ''
docs: https://docs.bokio.se/reference/scopes
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Bokio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bokio publishes 24 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bokio API on a user''s behalf.


  Tokens are issued from /token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bokio
provider_slug: bokio
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /token
  - authorizationUrl: /authorize
    flow: authorizationCode
    tokenUrl: /token
  name: access_token
  source: openapi/bokio-company-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: /token
  - authorizationUrl: /authorize
    flow: authorizationCode
    tokenUrl: /token
  name: access_token
  source: openapi/bokio-general-api-openapi.yml
scope_count: 24
scope_names:
- bank-payments:read-limited
- bank-payments:write
- chart-of-accounts:read
- company-information:read
- credit-notes:read
- credit-notes:write
- customers:read
- customers:write
- fiscal-years:read
- invoices:read
- invoices:write
- items:read
- items:write
- journal-entries:read
- journal-entries:write
- sie:read
- supplier-invoices:read
- supplier-invoices:write
- suppliers:read
- suppliers:write
- tags:read
- tags:write
- uploads:read
- uploads:write
scopes:
- description: Read access to bank payments created by the integration
  flows:
  - authorizationCode
  scope: bank-payments:read-limited
- description: Write access to bank payments
  flows:
  - authorizationCode
  scope: bank-payments:write
- description: Read access to chart of accounts
  flows:
  - authorizationCode
  scope: chart-of-accounts:read
- description: Read access to company information
  flows:
  - authorizationCode
  scope: company-information:read
- description: Read access to credit notes
  flows:
  - authorizationCode
  scope: credit-notes:read
- description: Write access to credit notes
  flows:
  - authorizationCode
  scope: credit-notes:write
- description: Read access to customers
  flows:
  - authorizationCode
  scope: customers:read
- description: Write access to customers
  flows:
  - authorizationCode
  scope: customers:write
- description: Read access to fiscal years
  flows:
  - authorizationCode
  scope: fiscal-years:read
- description: Read access to invoices
  flows:
  - authorizationCode
  scope: invoices:read
- description: Write access to invoices
  flows:
  - authorizationCode
  scope: invoices:write
- description: Read access to items
  flows:
  - authorizationCode
  scope: items:read
- description: Write access to items
  flows:
  - authorizationCode
  scope: items:write
- description: Read access to journal entries
  flows:
  - authorizationCode
  scope: journal-entries:read
- description: Write access to journal entries
  flows:
  - authorizationCode
  scope: journal-entries:write
- description: Read access to SIE files
  flows:
  - authorizationCode
  scope: sie:read
- description: Read access to supplier invoices
  flows:
  - authorizationCode
  scope: supplier-invoices:read
- description: Write access to supplier invoices
  flows:
  - authorizationCode
  scope: supplier-invoices:write
- description: Read access to suppliers
  flows:
  - authorizationCode
  scope: suppliers:read
- description: Write access to suppliers
  flows:
  - authorizationCode
  scope: suppliers:write
- description: Read access to tag groups and tags
  flows:
  - authorizationCode
  scope: tags:read
- description: Write access to tag groups and tags
  flows:
  - authorizationCode
  scope: tags:write
- description: Read access to uploads
  flows:
  - authorizationCode
  scope: uploads:read
- description: Write access to uploads
  flows:
  - authorizationCode
  scope: uploads:write
slug: bokio-scopes
source_filename: bokio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/bokio-company-api-openapi.yml, openapi/bokio-general-api-openapi.yml\ndocs: https://docs.bokio.se/reference/scopes\nnotes: >-\n  Scopes follow a {resource}:{action} naming pattern and are combined as a\n  space-delimited string in the OAuth authorization request. Elevated scopes\n  (e.g. bank-payments:write) are available only to public integrations under a\n  partnership contract and security review, and must be approved by Bokio's API\n  team before use.\nschemes:\n- name: access_token\n  source: openapi/bokio-company-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /token\n  - flow: authorizationCode\n    authorizationUrl: /authorize\n    tokenUrl: /token\n- name: access_token\n  source: openapi/bokio-general-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /token\n  - flow: authorizationCode\n    authorizationUrl: /authorize\n    tokenUrl: /token\nscopes:\n- scope: bank-payments:read-limited\n\
  \  description: Read access to bank payments created by the integration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: bank-payments:write\n  description: Write access to bank payments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: chart-of-accounts:read\n  description: Read access to chart of accounts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: company-information:read\n  description: Read access to company information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: credit-notes:read\n  description: Read access to credit notes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: credit-notes:write\n  description: Write access to credit notes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope:\
  \ customers:read\n  description: Read access to customers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: customers:write\n  description: Write access to customers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: fiscal-years:read\n  description: Read access to fiscal years\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: invoices:read\n  description: Read access to invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: invoices:write\n  description: Write access to invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: items:read\n  description: Read access to items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: items:write\n  description: Write access to items\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: journal-entries:read\n  description: Read access to journal entries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: journal-entries:write\n  description: Write access to journal entries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: sie:read\n  description: Read access to SIE files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: supplier-invoices:read\n  description: Read access to supplier invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: supplier-invoices:write\n  description: Write access to supplier invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: suppliers:read\n  description: Read access to suppliers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n\
  - scope: suppliers:write\n  description: Write access to suppliers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: tags:read\n  description: Read access to tag groups and tags\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: tags:write\n  description: Write access to tag groups and tags\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: uploads:read\n  description: Read access to uploads\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n- scope: uploads:write\n  description: Write access to uploads\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bokio-company-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/scopes/bokio-scopes.yml
summary_line: 24 scopes · clientCredentials/authorizationCode
tags:
- Company
- Fintech
- Accounting
- Bookkeeping
- Invoicing
- Payments
- Sweden
- SMB
- Authentication
token_urls:
- /token
---
