---
api_specs:
- filename: connexis-cash-account-information-psd2-stet-mock-openapi.yml
  format: yaml
  label: Connexis Cash PSD2 Account Information API (STET)
  slug: psd2-account-information
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml
- filename: connexis-cash-accounts-api-openapi.yml
  format: yaml
  label: Connexis Cash Accounts API
  slug: connexis-cash-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-accounts-api-openapi.yml
- filename: connexis-cash-balances-api-openapi.yml
  format: yaml
  label: Connexis Cash Balances API
  slug: connexis-cash-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-balances-api-openapi.yml
- filename: connexis-cash-beneficiaries-api-openapi.yml
  format: yaml
  label: Connexis Cash Beneficiaries API
  slug: connexis-cash-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-beneficiaries-api-openapi.yml
- filename: connexis-cash-consents-api-openapi.yml
  format: yaml
  label: Connexis Cash Consents API
  slug: connexis-cash-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-consents-api-openapi.yml
- filename: connexis-cash-transactions-api-openapi.yml
  format: yaml
  label: Connexis Cash Transactions API
  slug: connexis-cash-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-transactions-api-openapi.yml
authorization_urls:
- https://api.cib.bnpparibas.com/oauth2/v1/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Connexis Cash Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Connexis Cash publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Connexis Cash API on a user''s behalf.


  Tokens are issued from https://api.sandbox.cib.bnpparibas.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Connexis Cash
provider_slug: connexis-cash
schemes:
- description: 'In order to access each of the 3 scopes in Production environment, the TPP needs to get an authorization code grant OAUTH2 token.

    The client_id field within the token request must be filled with the value of the organization identifier attribute that has been set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.

    (cf §5.2.1 of https://docbox.etsi.org/ESI/Open/Latest_Drafts/ts_119495v000003_for-public-review.pdf)'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.sandbox.cib.bnpparibas.com/oauth2/v1/token
  name: OAuth2
  source: openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml
- flows:
  - authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  name: oauth2
  source: openapi/connexis-cash-accounts-api-openapi.yml
- flows:
  - authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  name: oauth2
  source: openapi/connexis-cash-balances-api-openapi.yml
- flows:
  - authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  name: oauth2
  source: openapi/connexis-cash-beneficiaries-api-openapi.yml
- flows:
  - authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  name: oauth2
  source: openapi/connexis-cash-consents-api-openapi.yml
- flows:
  - authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  name: oauth2
  source: openapi/connexis-cash-transactions-api-openapi.yml
scope_count: 3
scope_names:
- aisp
- cib-gb-account-information-psd2-stet-mock:piisp
- cib-gb-account-information-psd2-stet-mock:pisp
scopes:
- description: Access by an AISP to one given PSU's account
  flows:
  - authorizationCode
  - clientCredentials
  scope: aisp
- description: Access by a PIISP to one given PSU's account to check payment coverage
  flows:
  - clientCredentials
  scope: cib-gb-account-information-psd2-stet-mock:piisp
- description: Access by a PISP to payments resources
  flows:
  - clientCredentials
  scope: cib-gb-account-information-psd2-stet-mock:pisp
slug: connexis-cash-scopes
source_filename: connexis-cash-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml, openapi/connexis-cash-accounts-api-openapi.yml,\n  openapi/connexis-cash-balances-api-openapi.yml, openapi/connexis-cash-beneficiaries-api-openapi.yml,\n  openapi/connexis-cash-consents-api-openapi.yml, openapi/connexis-cash-transactions-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.sandbox.cib.bnpparibas.com/oauth2/v1/token\n  description: |-\n    In order to access each of the 3 scopes in Production environment, the TPP needs to get an authorization code grant OAUTH2 token.\n    The client_id field within the token request must be filled with the value of the organization identifier attribute that has been set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.\n    (cf §5.2.1\
  \ of https://docbox.etsi.org/ESI/Open/Latest_Drafts/ts_119495v000003_for-public-review.pdf)\n- name: oauth2\n  source: openapi/connexis-cash-accounts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n- name: oauth2\n  source: openapi/connexis-cash-balances-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n- name: oauth2\n  source: openapi/connexis-cash-beneficiaries-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n- name: oauth2\n  source: openapi/connexis-cash-consents-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n- name: oauth2\n  source: openapi/connexis-cash-transactions-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\nscopes:\n- scope: aisp\n  description: Access by an AISP to one given PSU's account\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml\n\
  \  - openapi/connexis-cash-accounts-api-openapi.yml\n  - openapi/connexis-cash-balances-api-openapi.yml\n  - openapi/connexis-cash-beneficiaries-api-openapi.yml\n  - openapi/connexis-cash-consents-api-openapi.yml\n  - openapi/connexis-cash-transactions-api-openapi.yml\n- scope: cib-gb-account-information-psd2-stet-mock:piisp\n  description: Access by a PIISP to one given PSU's account to check payment coverage\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml\n- scope: cib-gb-account-information-psd2-stet-mock:pisp\n  description: Access by a PISP to payments resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/scopes/connexis-cash-scopes.yml
summary_line: 3 scopes · clientCredentials/authorizationCode
tags:
- Account Information
- BNP Paribas
- Cash Management
- Corporate Banking
- Digital Banking
- Liquidity Management
- Open Banking
- Payments
- PSD2
- SCA
- STET
token_urls:
- https://api.sandbox.cib.bnpparibas.com/oauth2/v1/token
- https://api.cib.bnpparibas.com/oauth2/v1/token
---
