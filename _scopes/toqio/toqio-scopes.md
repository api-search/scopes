---
api_specs:
- filename: toqio-accounts-openapi.yml
  format: yaml
  label: Toqio Accounts API
  slug: toqio-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-accounts-openapi.yml
- filename: toqio-cards-openapi.yml
  format: yaml
  label: Toqio Cards API
  slug: toqio-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-cards-openapi.yml
- filename: toqio-transactions-openapi.yml
  format: yaml
  label: Toqio Transactions API
  slug: toqio-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-transactions-openapi.yml
- filename: toqio-beneficiaries-openapi.yml
  format: yaml
  label: Toqio Beneficiaries API
  slug: toqio-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-beneficiaries-openapi.yml
- filename: toqio-fees-openapi.yml
  format: yaml
  label: Toqio Fees API
  slug: toqio-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-fees-openapi.yml
- filename: toqio-clients-openapi.yml
  format: yaml
  label: Toqio Clients API
  slug: toqio-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-clients-openapi.yml
- filename: toqio-compliance-endpoints-openapi.yml
  format: yaml
  label: Toqio Compliance API
  slug: toqio-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-compliance-endpoints-openapi.yml
- filename: toqio-upload-kyb-documents-openapi.yml
  format: yaml
  label: Toqio KYB Documents API
  slug: toqio-kyb-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-upload-kyb-documents-openapi.yml
- filename: toqio-create-lead-service-openapi.yml
  format: yaml
  label: Toqio Create Lead API
  slug: toqio-create-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-create-lead-service-openapi.yml
- filename: toqio-revenue-collections-openapi.yml
  format: yaml
  label: Toqio Revenue Collections API
  slug: toqio-revenue-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-revenue-collections-openapi.yml
- filename: toqio-custom-notifications-openapi.yml
  format: yaml
  label: Toqio Custom Notifications API
  slug: toqio-custom-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-custom-notifications-openapi.yml
- filename: toqio-security-openapi.yml
  format: yaml
  label: Toqio Security API
  slug: toqio-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-security-openapi.yml
- filename: toqio-integration-hub-api-openapi.yml
  format: yaml
  label: Toqio Integration Hub API
  slug: toqio-integration-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-integration-hub-api-openapi.yml
- filename: toqio-card-management-api-openapi.yml
  format: yaml
  label: Toqio Card Management API (Integration Hub)
  slug: toqio-card-management-api-integration-hub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-card-management-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
- password
kind: oauth-scopes
layout: scope
method: derived
name: Toqio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Toqio publishes 3 OAuth 2.0 scopes via the clientCredentials and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Toqio API on a user''s behalf.


  Tokens are issued from https://api.toq.io/iam/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Toqio
provider_slug: toqio
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: clientCredentials
  source: openapi/toqio-accounts-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: clientCredentials
  source: openapi/toqio-beneficiaries-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: bearer-jwt
  source: openapi/toqio-cards-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: clientCredentials
  source: openapi/toqio-cards-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: clientCredentials
  source: openapi/toqio-clients-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: clientCredentials
  source: openapi/toqio-compliance-endpoints-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: OAuth2
  source: openapi/toqio-create-lead-service-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: clientCredentials
  source: openapi/toqio-custom-notifications-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: clientCredentials
  source: openapi/toqio-fees-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: OAuth2
  source: openapi/toqio-get-pre-signed-url-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: bearer-jwt
  source: openapi/toqio-security-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: clientCredentials
  source: openapi/toqio-security-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: clientCredentials
  source: openapi/toqio-transactions-openapi.yml
- flows:
  - flow: password
    tokenUrl: https://api.toq.io/iam/oauth/token
  name: OAuth2
  source: openapi/toqio-upload-kyb-documents-openapi.yml
scope_count: 3
scope_names:
- openid
- read
- write
scopes:
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: read
- description: ''
  flows: []
  scope: write
slug: toqio-scopes
source_filename: toqio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/toqio-accounts-openapi.yml, openapi/toqio-beneficiaries-openapi.yml, openapi/toqio-cards-openapi.yml,\n  openapi/toqio-clients-openapi.yml, openapi/toqio-compliance-endpoints-openapi.yml, openapi/toqio-create-lead-service-openapi.yml,\n  openapi/toqio-custom-notifications-openapi.yml, openapi/toqio-fees-openapi.yml, openapi/toqio-get-pre-signed-url-openapi.yml,\n  openapi/toqio-security-openapi.yml, openapi/toqio-transactions-openapi.yml, openapi/toqio-upload-kyb-documents-openapi.yml\nschemes:\n- name: clientCredentials\n  source: openapi/toqio-accounts-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.toq.io/iam/oauth/token\n- name: clientCredentials\n  source: openapi/toqio-beneficiaries-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.toq.io/iam/oauth/token\n- name: bearer-jwt\n  source: openapi/toqio-cards-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl:\
  \ https://api.toq.io/iam/oauth/token\n- name: clientCredentials\n  source: openapi/toqio-cards-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.toq.io/iam/oauth/token\n- name: clientCredentials\n  source: openapi/toqio-clients-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.toq.io/iam/oauth/token\n- name: clientCredentials\n  source: openapi/toqio-compliance-endpoints-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.toq.io/iam/oauth/token\n- name: OAuth2\n  source: openapi/toqio-create-lead-service-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.toq.io/iam/oauth/token\n- name: clientCredentials\n  source: openapi/toqio-custom-notifications-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.toq.io/iam/oauth/token\n- name: clientCredentials\n  source: openapi/toqio-fees-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.toq.io/iam/oauth/token\n\
  - name: OAuth2\n  source: openapi/toqio-get-pre-signed-url-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.toq.io/iam/oauth/token\n- name: bearer-jwt\n  source: openapi/toqio-security-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.toq.io/iam/oauth/token\n- name: clientCredentials\n  source: openapi/toqio-security-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.toq.io/iam/oauth/token\n- name: clientCredentials\n  source: openapi/toqio-transactions-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.toq.io/iam/oauth/token\n- name: OAuth2\n  source: openapi/toqio-upload-kyb-documents-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.toq.io/iam/oauth/token\nscopes:\n- scope: openid\n  sources:\n  - openapi/toqio-create-lead-service-openapi.yml\n  - openapi/toqio-get-pre-signed-url-openapi.yml\n  - openapi/toqio-upload-kyb-documents-openapi.yml\n- scope: read\n  sources:\n \
  \ - openapi/toqio-cards-openapi.yml\n  - openapi/toqio-security-openapi.yml\n- scope: write\n  sources:\n  - openapi/toqio-cards-openapi.yml\n  - openapi/toqio-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/scopes/toqio-scopes.yml
summary_line: 3 scopes · clientCredentials/password
tags:
- Embedded Finance
- Fintech
- Banking as a Service
- Payments
- Cards
- Corporate Banking
- Lending
- Compliance
- SMEs
token_urls:
- https://api.toq.io/iam/oauth/token
---
