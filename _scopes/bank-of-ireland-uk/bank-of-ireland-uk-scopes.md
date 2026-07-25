---
api_specs:
- filename: bank-of-ireland-uk-open-data-openapi.json
  format: json
  label: Bank of Ireland (UK) Open Data API
  slug: bank-of-ireland-uk-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-open-data-openapi.json
- filename: bank-of-ireland-uk-account-info-openapi.yaml
  format: yaml
  label: Bank of Ireland (UK) Account & Transaction Information API
  slug: bank-of-ireland-uk-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-account-info-openapi.yaml
- filename: bank-of-ireland-uk-payment-initiation-openapi.yaml
  format: yaml
  label: Bank of Ireland (UK) Payment Initiation API
  slug: bank-of-ireland-uk-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-payment-initiation-openapi.yaml
- filename: bank-of-ireland-uk-confirmation-funds-openapi.yaml
  format: yaml
  label: Bank of Ireland (UK) Confirmation of Funds API
  slug: bank-of-ireland-uk-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-confirmation-funds-openapi.yaml
authorization_urls:
- https://auth.obapi.bankofireland.com/oauth/as/b365/authorization.oauth2
description: ''
docs: https://auth.obapi.bankofireland.com/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Bank Of Ireland Uk Scopes
name_suffix: OAuth Scopes
note: Scope surface upgraded from the OBIE spec placeholders using the LIVE FAPI OpenID discovery document at the Bank of Ireland (UK) UK authorization host (https://auth.obapi.bankofireland.com). The discovery document advertises scopes_supported [openid, payments, accounts]; the OBIE Read/Write CBPII spec adds the fundsconfirmations scope. Real token/authorization endpoints replace the spec's authserver.example placeholders. Tokens are mutual-TLS certificate-bound (tls_client_certificate_bound_access_tokens=true) and access requires PSD2 SCA (acr urn:openbanking:psd2:sca).
overview: 'Bank of Ireland (UK) publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bank of Ireland (UK) API on a user''s behalf.


  Tokens are issued from https://api.obapi.bankofireland.com/oauth/as/token.oauth2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bank of Ireland (UK)
provider_slug: bank-of-ireland-uk
schemes:
- description: PSU authorization-code flow (hybrid code id_token, response_mode fragment, PS256 request objects) used when the PSU performs SCA with the ASPSP.
  flows:
  - authorizationUrl: https://auth.obapi.bankofireland.com/oauth/as/b365/authorization.oauth2
    flow: authorizationCode
    tokenUrl: https://api.obapi.bankofireland.com/oauth/as/token.oauth2
  name: PSUOAuth2Security
  source: well-known/bank-of-ireland-uk-openid-configuration.json
  type: oauth2
- description: TPP client-credentials flow with the ASPSP (tls_client_auth).
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.obapi.bankofireland.com/oauth/as/token.oauth2
  name: TPPOAuth2Security
  source: well-known/bank-of-ireland-uk-openid-configuration.json
  type: oauth2
scope_count: 4
scope_names:
- openid
- accounts
- payments
- fundsconfirmations
scopes:
- description: OpenID Connect authentication; required to obtain an id_token and the openbanking_intent_id claim.
  flows:
  - authorizationCode
  scope: openid
- description: Read access to account, balance, transaction, beneficiary, standing-order, direct-debit and product information (AIS).
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts
- description: Initiate domestic/international single, scheduled, standing-order and file payments (PIS).
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
- description: Confirm availability of funds on a PSU account for a card-based payment instrument issuer (CBPII).
  flows:
  - authorizationCode
  - clientCredentials
  scope: fundsconfirmations
slug: bank-of-ireland-uk-scopes
source_filename: bank-of-ireland-uk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/bank-of-ireland-uk-account-info-openapi.yaml, openapi/bank-of-ireland-uk-confirmation-funds-openapi.yaml, openapi/bank-of-ireland-uk-payment-initiation-openapi.yaml\ndocs: https://auth.obapi.bankofireland.com/.well-known/openid-configuration\nnote: >-\n  Scope surface upgraded from the OBIE spec placeholders using the LIVE FAPI\n  OpenID discovery document at the Bank of Ireland (UK) UK authorization host\n  (https://auth.obapi.bankofireland.com). The discovery document advertises\n  scopes_supported [openid, payments, accounts]; the OBIE Read/Write CBPII spec\n  adds the fundsconfirmations scope. Real token/authorization endpoints replace\n  the spec's authserver.example placeholders. Tokens are mutual-TLS\n  certificate-bound (tls_client_certificate_bound_access_tokens=true) and access\n  requires PSD2 SCA (acr urn:openbanking:psd2:sca).\nschemes:\n- name: PSUOAuth2Security\n  type: oauth2\n  source: well-known/bank-of-ireland-uk-openid-configuration.json\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.obapi.bankofireland.com/oauth/as/b365/authorization.oauth2\n    tokenUrl: https://api.obapi.bankofireland.com/oauth/as/token.oauth2\n  description: >-\n    PSU authorization-code flow (hybrid code id_token, response_mode fragment,\n    PS256 request objects) used when the PSU performs SCA with the ASPSP.\n- name: TPPOAuth2Security\n  type: oauth2\n  source: well-known/bank-of-ireland-uk-openid-configuration.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.obapi.bankofireland.com/oauth/as/token.oauth2\n  description: TPP client-credentials flow with the ASPSP (tls_client_auth).\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; required to obtain an id_token and the openbanking_intent_id claim.\n  flows: [authorizationCode]\n  sources: [well-known/bank-of-ireland-uk-openid-configuration.json]\n- scope: accounts\n  description: Read access to account, balance, transaction,\
  \ beneficiary, standing-order, direct-debit and product information (AIS).\n  flows: [authorizationCode, clientCredentials]\n  sources:\n  - well-known/bank-of-ireland-uk-openid-configuration.json\n  - openapi/bank-of-ireland-uk-account-info-openapi.yaml\n- scope: payments\n  description: Initiate domestic/international single, scheduled, standing-order and file payments (PIS).\n  flows: [authorizationCode, clientCredentials]\n  sources:\n  - well-known/bank-of-ireland-uk-openid-configuration.json\n  - openapi/bank-of-ireland-uk-payment-initiation-openapi.yaml\n- scope: fundsconfirmations\n  description: Confirm availability of funds on a PSU account for a card-based payment instrument issuer (CBPII).\n  flows: [authorizationCode, clientCredentials]\n  sources: [openapi/bank-of-ireland-uk-confirmation-funds-openapi.yaml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/scopes/bank-of-ireland-uk-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
- Open Data
- FAPI
- Fintech
token_urls:
- https://api.obapi.bankofireland.com/oauth/as/token.oauth2
---
