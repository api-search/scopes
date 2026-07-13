---
api_specs:
- filename: us-bank-corporate-account-information-openapi.yml
  format: yaml
  label: US Bank Corporate Account Information API
  slug: us-bank-corporate-account-information
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-corporate-account-information-openapi.yml
- filename: us-bank-rtp-openapi.yml
  format: yaml
  label: US Bank RTP Real-Time Payments API
  slug: us-bank-rtp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-rtp-openapi.yml
- filename: us-bank-ach-originations-openapi.yml
  format: yaml
  label: US Bank ACH Originations API
  slug: us-bank-ach-originations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-ach-originations-openapi.yml
- filename: us-bank-positive-pay-openapi.yml
  format: yaml
  label: US Bank Positive Pay API
  slug: us-bank-positive-pay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-positive-pay-openapi.yml
- filename: us-bank-push-to-card-openapi.yml
  format: yaml
  label: US Bank Push to Card API
  slug: us-bank-push-to-card
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-push-to-card-openapi.yml
authorization_urls:
- https://api.usbank.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Us Bancorp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'US Bancorp publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the US Bancorp API on a user''s behalf.


  Tokens are issued from https://api.usbank.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: US Bancorp
provider_slug: us-bancorp
schemes:
- description: OAuth 2.0 with MFA using SinglePoint credentials
  flows:
  - authorizationUrl: https://api.usbank.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.usbank.com/oauth/token
  name: OAuth2MFA
  source: openapi/us-bank-corporate-account-information-openapi.yml
- description: OAuth 2.0 with MFA using SinglePoint credentials
  flows:
  - authorizationUrl: https://api.usbank.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.usbank.com/oauth/token
  name: OAuth2MFA
  source: openapi/us-bank-positive-pay-openapi.yml
- description: OAuth 2.0 with MFA using SinglePoint credentials
  flows:
  - authorizationUrl: https://api.usbank.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.usbank.com/oauth/token
  name: OAuth2MFA
  source: openapi/us-bank-push-to-card-openapi.yml
- description: OAuth 2.0 with MFA using SinglePoint credentials
  flows:
  - authorizationUrl: https://api.usbank.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.usbank.com/oauth/token
  name: OAuth2MFA
  source: openapi/us-bank-rtp-openapi.yml
scope_count: 6
scope_names:
- account.read
- payment.read
- payment.write
- positivepay.read
- positivepay.write
- transaction.read
scopes:
- description: Read account information
  flows:
  - authorizationCode
  scope: account.read
- description: Read payment status
  flows:
  - authorizationCode
  scope: payment.read
- description: Initiate card payments
  flows:
  - authorizationCode
  scope: payment.write
- description: Read exception items
  flows:
  - authorizationCode
  scope: positivepay.read
- description: Submit decisions
  flows:
  - authorizationCode
  scope: positivepay.write
- description: Read transaction data
  flows:
  - authorizationCode
  scope: transaction.read
slug: us-bancorp-scopes
source_filename: us-bancorp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/us-bank-corporate-account-information-openapi.yml, openapi/us-bank-positive-pay-openapi.yml,\n  openapi/us-bank-push-to-card-openapi.yml, openapi/us-bank-rtp-openapi.yml\nschemes:\n- name: OAuth2MFA\n  source: openapi/us-bank-corporate-account-information-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.usbank.com/oauth/authorize\n    tokenUrl: https://api.usbank.com/oauth/token\n  description: OAuth 2.0 with MFA using SinglePoint credentials\n- name: OAuth2MFA\n  source: openapi/us-bank-positive-pay-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.usbank.com/oauth/authorize\n    tokenUrl: https://api.usbank.com/oauth/token\n  description: OAuth 2.0 with MFA using SinglePoint credentials\n- name: OAuth2MFA\n  source: openapi/us-bank-push-to-card-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.usbank.com/oauth/authorize\n\
  \    tokenUrl: https://api.usbank.com/oauth/token\n  description: OAuth 2.0 with MFA using SinglePoint credentials\n- name: OAuth2MFA\n  source: openapi/us-bank-rtp-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.usbank.com/oauth/authorize\n    tokenUrl: https://api.usbank.com/oauth/token\n  description: OAuth 2.0 with MFA using SinglePoint credentials\nscopes:\n- scope: account.read\n  description: Read account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/us-bank-corporate-account-information-openapi.yml\n- scope: payment.read\n  description: Read payment status\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/us-bank-push-to-card-openapi.yml\n  - openapi/us-bank-rtp-openapi.yml\n- scope: payment.write\n  description: Initiate card payments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/us-bank-push-to-card-openapi.yml\n  - openapi/us-bank-rtp-openapi.yml\n- scope: positivepay.read\n  description: Read\
  \ exception items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/us-bank-positive-pay-openapi.yml\n- scope: positivepay.write\n  description: Submit decisions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/us-bank-positive-pay-openapi.yml\n- scope: transaction.read\n  description: Read transaction data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/us-bank-corporate-account-information-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/scopes/us-bancorp-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Banking
- Finance
- Fortune 500
- Corporate Banking
- Payments
- Open Banking
- Treasury Management
- Consumer Banking
token_urls:
- https://api.usbank.com/oauth/token
---
