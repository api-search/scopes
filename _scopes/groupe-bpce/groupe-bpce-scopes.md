---
api_specs:
- filename: groupe-bpce-aisp-api-openapi.yml
  format: yaml
  label: Groupe BPCE AISP API
  slug: groupe-bpce-aisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-aisp-api-openapi.yml
- filename: groupe-bpce-cbpii-api-openapi.yml
  format: yaml
  label: Groupe BPCE CBPII API
  slug: groupe-bpce-cbpii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-cbpii-api-openapi.yml
- filename: groupe-bpce-external-accounts-api-openapi.yml
  format: yaml
  label: Groupe BPCE External Accounts API
  slug: groupe-bpce-external-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-external-accounts-api-openapi.yml
- filename: groupe-bpce-internal-accounts-api-openapi.yml
  format: yaml
  label: Groupe BPCE Internal Accounts API
  slug: groupe-bpce-internal-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-internal-accounts-api-openapi.yml
- filename: groupe-bpce-pisp-api-openapi.yml
  format: yaml
  label: Groupe BPCE PISP API
  slug: groupe-bpce-pisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-pisp-api-openapi.yml
- filename: groupe-bpce-registration-api-openapi.yml
  format: yaml
  label: Groupe BPCE Registration API
  slug: groupe-bpce-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-registration-api-openapi.yml
- filename: groupe-bpce-transfers-api-openapi.yml
  format: yaml
  label: Groupe BPCE Transfers API
  slug: groupe-bpce-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-transfers-api-openapi.yml
authorization_urls:
- /stet/psd2/oauth/authorize
- /api/oauth/authorize
- /psd2/oauth/authorize
description: ''
docs: https://apistore.groupebpce.com/api/psd2-registration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Groupe Bpce Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Groupe BPCE publishes 12 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Groupe BPCE API on a user''s behalf.


  Tokens are issued from /stet/psd2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Groupe BPCE
provider_slug: groupe-bpce
schemes:
- description: 'In order to access the PSU''s account information, the AISP needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token.

    In order to post a funds confirmation request, the CBPII needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token when registration of the account has not been previously processed.

    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token.

    The client_id field within the token request must be filled with the value of the organization identifier attribute that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.

    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'
  flows:
  - authorizationUrl: /stet/psd2/oauth/authorize
    flow: authorizationCode
    tokenUrl: /stet/psd2/oauth/token
  name: accessCode
  source: openapi/groupe-bpce-natixis-psd2-accounts-openapi.yml
- description: 'In order to access the PSU''s account information, the AISP needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token.

    In order to post a funds confirmation request, the CBPII needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token when registration of the account has not been previously processed.

    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token.

    The client_id field within the token request must be filled with the value of the organization identifier attribute that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.

    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'
  flows:
  - authorizationUrl: /stet/psd2/oauth/authorize
    flow: authorizationCode
    tokenUrl: /stet/psd2/oauth/token
  name: accessCode
  source: openapi/groupe-bpce-natixis-wealth-management-psd2-accounts-openapi.yml
- flows:
  - authorizationUrl: /api/oauth/authorize
    flow: authorizationCode
    tokenUrl: /api/oauth/token
  name: oauth2-authorizationCodePKCE-moneyTransfer
  source: openapi/groupe-bpce-open-finance-transfer-openapi.yml
- description: 'In order to access the PSU''s account information, the AISP needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token.

    In order to post a funds confirmation request, the CBPII needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token when registration of the account has not been previously processed.

    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token.

    The client_id field within the token request must be filled with the value of the organization identifier attribute that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.

    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'
  flows:
  - authorizationUrl: /stet/psd2/oauth/authorize
    flow: authorizationCode
    tokenUrl: /stet/psd2/oauth/token
  name: accessCode
  source: openapi/groupe-bpce-psd2-accounts-openapi.yml
- description: 'In order to access the PSU''s account information, the AISP needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token.

    In order to post a funds confirmation request, the CBPII needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token when registration of the account has not been previously processed.

    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token.

    The client_id field within the token request must be filled with the value of the organization identifier attribute that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.

    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'
  flows:
  - authorizationUrl: /stet/psd2/oauth/authorize
    flow: authorizationCode
    tokenUrl: /stet/psd2/oauth/token
  name: accessCode
  source: openapi/groupe-bpce-psd2-funds-availability-openapi.yml
- description: 'In order to post, get or cancel a Payment or Transfer Request, the PISP needs to get a client credential OAUTH2 token.

    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant or a client credential OAUTH2 token.

    In order to post a funds confirmation request, the CBPII needs to get a client credential OAUTH2 token when registration of the account has already been previously processed.

    The client_id field within the token request must be filled with the value of the organization identifier attribute that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.

    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'
  flows:
  - flow: clientCredentials
    tokenUrl: /stet/psd2/oauth/token
  name: clientCredentials
  source: openapi/groupe-bpce-psd2-funds-availability-openapi.yml
- description: 'In order to access the PSU''s account information, the AISP needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token.

    In order to post a funds confirmation request, the CBPII needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token when registration of the account has not been previously processed.

    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant or a Client Initiated Backchannel Authentication token.

    The client_id field within the token request must be filled with the value of the organization identifier attribute that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.

    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'
  flows:
  - authorizationUrl: /psd2/oauth/authorize
    flow: authorizationCode
    tokenUrl: /stet/psd2/oauth/token
  name: accessCode
  source: openapi/groupe-bpce-psd2-payments-openapi.yml
- description: 'In order to post, get or cancel a Payment or Transfer Request, the PISP needs to get a client credential OAUTH2 token.

    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant or a client credential OAUTH2 token.

    In order to post a funds confirmation request, the CBPII needs to get a client credential OAUTH2 token when registration of the account has already been previously processed.

    The client_id field within the token request must be filled with the value of the organization identifier attribute that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.

    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'
  flows:
  - flow: clientCredentials
    tokenUrl: /stet/psd2/oauth/token
  name: clientCredentials
  source: openapi/groupe-bpce-psd2-payments-openapi.yml
scope_count: 12
scope_names:
- aisp
- cbpii
- extended_transaction_history
- moneyTransfer.externalAccounts:READ
- moneyTransfer.externalAccounts:WRITE
- moneyTransfer.internalAccounts:READ
- moneyTransfer.transferRequests.confirmations:WRITE
- moneyTransfer.transferRequests:DELETE
- moneyTransfer.transferRequests:READ
- moneyTransfer.transferRequests:WRITE
- pisp
- manageRegistration
scopes:
- description: Access by an AISP to one given PSU's account
  flows:
  - authorizationCode
  scope: aisp
- description: Access by a CBPII to one given PSU's account to check payment coverage
  flows:
  - authorizationCode
  - clientCredentials
  scope: cbpii
- description: Access by an AISP to a transaction history over more than the 90 last days
  flows:
  - authorizationCode
  scope: extended_transaction_history
- description: Scope for read External accounts
  flows:
  - authorizationCode
  scope: moneyTransfer.externalAccounts:READ
- description: Scope for write External accounts
  flows:
  - authorizationCode
  scope: moneyTransfer.externalAccounts:WRITE
- description: Scope for read Internal accounts
  flows:
  - authorizationCode
  scope: moneyTransfer.internalAccounts:READ
- description: Scope for transfer requests confirmations.
  flows:
  - authorizationCode
  scope: moneyTransfer.transferRequests.confirmations:WRITE
- description: Scope to delete transfer requests.
  flows:
  - authorizationCode
  scope: moneyTransfer.transferRequests:DELETE
- description: Minimal scope for consultation of transfer requests
  flows:
  - authorizationCode
  scope: moneyTransfer.transferRequests:READ
- description: Scope to create or modify transfer requests
  flows:
  - authorizationCode
  scope: moneyTransfer.transferRequests:WRITE
- description: Access by a PISP for posting a confirmation after authentication of the PSU through OAUTH2 Authorization Code
  flows:
  - authorizationCode
  - clientCredentials
  scope: pisp
- description: Client-credentials scope for the PSD2 Registration API token (POST /token with generic client_id "PSD2_TPPRegister", mutual TLS with QWAC). Not declared in the registration spec.
  flows: []
  scope: manageRegistration
slug: groupe-bpce-scopes
source_filename: groupe-bpce-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: openapi/groupe-bpce-natixis-psd2-accounts-openapi.yml, openapi/groupe-bpce-natixis-wealth-management-psd2-accounts-openapi.yml,\n  openapi/groupe-bpce-open-finance-transfer-openapi.yml, openapi/groupe-bpce-psd2-accounts-openapi.yml, openapi/groupe-bpce-psd2-funds-availability-openapi.yml,\n  openapi/groupe-bpce-psd2-payments-openapi.yml, https://apistore.groupebpce.com/api/psd2-registration, https://apistore.groupebpce.com/api/account-information-services-3\nschemes:\n- name: accessCode\n  source: openapi/groupe-bpce-natixis-psd2-accounts-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /stet/psd2/oauth/authorize\n    tokenUrl: /stet/psd2/oauth/token\n  description: 'In order to access the PSU''s account information, the AISP needs to get either an authorization\n    code grant or a Client Initiated Backchannel Authentication token.\n\n    In order to post a funds confirmation request, the CBPII needs\
  \ to get either an authorization code grant or\n    a Client Initiated Backchannel Authentication token when registration of the account has not been previously\n    processed.\n\n    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant\n    or a Client Initiated Backchannel Authentication token.\n\n    The client_id field within the token request must be filled with the value of the organization identifier attribute\n    that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.\n\n    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'\n- name: accessCode\n  source: openapi/groupe-bpce-natixis-wealth-management-psd2-accounts-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /stet/psd2/oauth/authorize\n    tokenUrl: /stet/psd2/oauth/token\n  description: 'In order to access the PSU''s account information, the AISP\
  \ needs to get either an authorization\n    code grant or a Client Initiated Backchannel Authentication token.\n\n    In order to post a funds confirmation request, the CBPII needs to get either an authorization code grant or\n    a Client Initiated Backchannel Authentication token when registration of the account has not been previously\n    processed.\n\n    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant\n    or a Client Initiated Backchannel Authentication token.\n\n    The client_id field within the token request must be filled with the value of the organization identifier attribute\n    that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.\n\n    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'\n- name: oauth2-authorizationCodePKCE-moneyTransfer\n  source: openapi/groupe-bpce-open-finance-transfer-openapi.yml\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: /api/oauth/authorize\n    tokenUrl: /api/oauth/token\n- name: accessCode\n  source: openapi/groupe-bpce-psd2-accounts-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /stet/psd2/oauth/authorize\n    tokenUrl: /stet/psd2/oauth/token\n  description: 'In order to access the PSU''s account information, the AISP needs to get either an authorization\n    code grant or a Client Initiated Backchannel Authentication token.\n\n    In order to post a funds confirmation request, the CBPII needs to get either an authorization code grant or\n    a Client Initiated Backchannel Authentication token when registration of the account has not been previously\n    processed.\n\n    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant\n    or a Client Initiated Backchannel Authentication token.\n\n    The client_id field within the token request must be filled with the value of\
  \ the organization identifier attribute\n    that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.\n\n    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'\n- name: accessCode\n  source: openapi/groupe-bpce-psd2-funds-availability-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /stet/psd2/oauth/authorize\n    tokenUrl: /stet/psd2/oauth/token\n  description: 'In order to access the PSU''s account information, the AISP needs to get either an authorization\n    code grant or a Client Initiated Backchannel Authentication token.\n\n    In order to post a funds confirmation request, the CBPII needs to get either an authorization code grant or\n    a Client Initiated Backchannel Authentication token when registration of the account has not been previously\n    processed.\n\n    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization\
  \ code grant\n    or a Client Initiated Backchannel Authentication token.\n\n    The client_id field within the token request must be filled with the value of the organization identifier attribute\n    that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.\n\n    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'\n- name: clientCredentials\n  source: openapi/groupe-bpce-psd2-funds-availability-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /stet/psd2/oauth/token\n  description: 'In order to post, get or cancel a Payment or Transfer Request, the PISP needs to get a client credential\n    OAUTH2 token.\n\n    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant\n    or a client credential OAUTH2 token.\n\n    In order to post a funds confirmation request, the CBPII needs to get a client credential OAUTH2 token when\n\
  \    registration of the account has already been previously processed.\n\n    The client_id field within the token request must be filled with the value of the organization identifier attribute\n    that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.\n\n    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'\n- name: accessCode\n  source: openapi/groupe-bpce-psd2-payments-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /psd2/oauth/authorize\n    tokenUrl: /stet/psd2/oauth/token\n  description: 'In order to access the PSU''s account information, the AISP needs to get either an authorization\n    code grant or a Client Initiated Backchannel Authentication token.\n\n    In order to post a funds confirmation request, the CBPII needs to get either an authorization code grant or\n    a Client Initiated Backchannel Authentication token when registration of the account\
  \ has not been previously\n    processed.\n\n    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant\n    or a Client Initiated Backchannel Authentication token.\n\n    The client_id field within the token request must be filled with the value of the organization identifier attribute\n    that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.\n\n    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'\n- name: clientCredentials\n  source: openapi/groupe-bpce-psd2-payments-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /stet/psd2/oauth/token\n  description: 'In order to post, get or cancel a Payment or Transfer Request, the PISP needs to get a client credential\n    OAUTH2 token.\n\n    In order to confirm a Payment or Transfer Request, the PISP needs to get either an authorization code grant\n    or a client credential\
  \ OAUTH2 token.\n\n    In order to post a funds confirmation request, the CBPII needs to get a client credential OAUTH2 token when\n    registration of the account has already been previously processed.\n\n    The client_id field within the token request must be filled with the value of the organization identifier attribute\n    that was set in the distinguished name of eIDAS certificate of the TPP, according to ETSI recommandations.\n\n    (cf §5.2.1 of [ETSI specfication](https://www.etsi.org/standards-search#page=1&search=TS119495))'\nscopes:\n- scope: aisp\n  description: Access by an AISP to one given PSU's account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/groupe-bpce-natixis-psd2-accounts-openapi.yml\n  - openapi/groupe-bpce-natixis-wealth-management-psd2-accounts-openapi.yml\n  - openapi/groupe-bpce-psd2-accounts-openapi.yml\n- scope: cbpii\n  description: Access by a CBPII to one given PSU's account to check payment coverage\n  flows:\n  - authorizationCode\n  -\
  \ clientCredentials\n  sources:\n  - openapi/groupe-bpce-psd2-funds-availability-openapi.yml\n- scope: extended_transaction_history\n  description: Access by an AISP to a transaction history over more than the 90 last days\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/groupe-bpce-natixis-psd2-accounts-openapi.yml\n  - openapi/groupe-bpce-natixis-wealth-management-psd2-accounts-openapi.yml\n  - openapi/groupe-bpce-psd2-accounts-openapi.yml\n- scope: moneyTransfer.externalAccounts:READ\n  description: Scope for read External accounts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/groupe-bpce-open-finance-transfer-openapi.yml\n- scope: moneyTransfer.externalAccounts:WRITE\n  description: Scope for write External accounts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/groupe-bpce-open-finance-transfer-openapi.yml\n- scope: moneyTransfer.internalAccounts:READ\n  description: Scope for read Internal accounts\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/groupe-bpce-open-finance-transfer-openapi.yml\n- scope: moneyTransfer.transferRequests.confirmations:WRITE\n  description: Scope for transfer requests confirmations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/groupe-bpce-open-finance-transfer-openapi.yml\n- scope: moneyTransfer.transferRequests:DELETE\n  description: Scope to delete transfer requests.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/groupe-bpce-open-finance-transfer-openapi.yml\n- scope: moneyTransfer.transferRequests:READ\n  description: Minimal scope for consultation of transfer requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/groupe-bpce-open-finance-transfer-openapi.yml\n- scope: moneyTransfer.transferRequests:WRITE\n  description: Scope to create or modify transfer requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/groupe-bpce-open-finance-transfer-openapi.yml\n- scope: pisp\n  description: Access by a PISP for posting a confirmation after authentication\
  \ of the PSU through OAUTH2 Authorization\n    Code\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/groupe-bpce-psd2-payments-openapi.yml\n- name: manageRegistration\n  description: Client-credentials scope for the PSD2 Registration API token (POST /token with generic client_id\n    \"PSD2_TPPRegister\", mutual TLS with QWAC). Not declared in the registration spec.\n  source: https://apistore.groupebpce.com/api/psd2-registration\ndocs: https://apistore.groupebpce.com/api/psd2-registration\nnotes: 'Registration payload field \"scope\": \"TPP scopes are comma separated, and possible values are : “aisp” and/or\n  “pisp” and/or “cbpii”\". AIS docs: Authorization Code /token requests \"shall be sent WITHOUT the « scope » parameter\";\n  client_credentials uses scope=aisp.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/scopes/groupe-bpce-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials
tags:
- Company
- Banking
- Financial Services
- Open Banking
- PSD2
- Payments
- Insurance
- France
token_bound: false
token_urls:
- /stet/psd2/oauth/token
- /api/oauth/token
---
