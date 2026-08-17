---
api_specs:
- filename: optum-dental-attachment-api-openapi.yml
  format: yaml
  label: Optum Medical Network Eligibility and Claims API
  slug: optum-medical-network-eligibility-and-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-dental-attachment-api-openapi.yml
- filename: optum-attachment-openapi.yml
  format: yaml
  label: Optum Real (Medical) API
  slug: optum-real-medical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-attachment-openapi.yml
- filename: optum-dental-pre-care-estimate-api-openapi.yml
  format: yaml
  label: Optum Real for Dental API
  slug: optum-real-for-dental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-dental-pre-care-estimate-api-openapi.yml
- filename: optum-formatting-rule-api-openapi.yml
  format: yaml
  label: Optum Pharmacy Solutions API
  slug: optum-pharmacy-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-formatting-rule-api-openapi.yml
- filename: optum-edi-enrollment-v1-openapi.yml
  format: yaml
  label: Optum Payment and Reimbursement API
  slug: optum-payment-and-reimbursement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-edi-enrollment-v1-openapi.yml
- filename: optum-cms-common-facility-openapi.yml
  format: yaml
  label: Optum Insight Platform (Platform and Interoperability) API
  slug: optum-insight-platform-platform-and-interoperability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-cms-common-facility-openapi.yml
- filename: optum-abm-care-decision-support-api-openapi.yml
  format: yaml
  label: Optum Analytics and Insights API
  slug: optum-analytics-and-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-abm-care-decision-support-api-openapi.yml
- filename: optum-security-and-authorization-v2-openapi.yml
  format: yaml
  label: Optum API Tools — Security and Authorization
  slug: optum-api-tools-security-and-authorization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-security-and-authorization-v2-openapi.yml
authorization_urls:
- https://idx.linkhealth.com/auth
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Optum Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Optum publishes 7 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Optum API on a user''s behalf.


  Tokens are issued from /apip/auth/sntl/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Optum
provider_slug: optum
schemes:
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-attachment-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-auth-referral-submission-api-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-auth-referral-submission-health-check-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-benefit-check-api-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-claim-actions-api-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/v2/token
  name: oAuth
  source: openapi/optum-claim-actions-health-check-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-claim-inquiry-api-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-claim-inquiry-health-check-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/v2/token
  name: oAuth
  source: openapi/optum-claim-pre-check-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: '{{baseUrl}}/apip/auth/v2/token'
  name: Bearer
  source: openapi/optum-dental-attachment-api-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-document-search-api-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-document-search-health-check-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox-apigw.optum.com/apip/auth/sntl/v1/token
  name: oauth2
  source: openapi/optum-edi-enrollment-v1-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-eligibility-pre-service-health-check-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow. [More info](https://api.example.com/docs/auth)
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/v2/token
  name: oAuth
  source: openapi/optum-enhanced-eligibility-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://idx-stage.linkhealth.com/auth/realms/developer-platform/protocol/openid-connect/token
  name: oauth2_security
  source: openapi/optum-formatting-rule-api-openapi.yml
- flows:
  - authorizationUrl: https://idx.linkhealth.com/auth
    flow: authorizationCode
    tokenUrl: https://idx.linkhealth.com/auth/token
  name: ncc_auth
  source: openapi/optum-ncc-data-acquisition-api-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/v2/token
  name: oAuth
  source: openapi/optum-optum-real-health-check-api-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-optum-real-pre-service-eligibility-api-openapi.yml
- flows:
  - authorizationUrl: https://idx.linkhealth.com/auth
    flow: authorizationCode
    tokenUrl: https://idx.linkhealth.com/auth/token
  name: ws_auth
  source: openapi/optum-optum-real-time-econtent-web-services-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-patient-benefit-check-health-check-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/v2/token
  name: oAuth
  source: openapi/optum-real-prior-authorization-api-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/v2/token
  name: oAuth
  source: openapi/optum-real-provider-access-api-openapi.yml
- description: This API uses OAuth 2 with the client_credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /apip/auth/sntl/v1/token
  name: oAuth
  source: openapi/optum-submitter-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://idx-stage.linkhealth.com/auth/realms/developer-platform/protocol/openid-connect/token
  name: oauth2_security
  source: openapi/optum-telecom-formatter-api-openapi.yml
scope_count: 7
scope_names:
- create_coveragediscovery
- create_txn
- profile
- read_coveragediscovery
- read_healthcheck
- read_txn
- scope-1
scopes:
- description: submit a new coverage discovery task
  flows:
  - clientCredentials
  scope: create_coveragediscovery
- description: submit a new transaction request
  flows:
  - clientCredentials
  scope: create_txn
- description: ''
  flows:
  - clientCredentials
  scope: profile
- description: read coverage discovery tasks
  flows:
  - clientCredentials
  scope: read_coveragediscovery
- description: check the status of the system
  flows:
  - clientCredentials
  scope: read_healthcheck
- description: read transactions
  flows:
  - clientCredentials
  scope: read_txn
- description: required scope for API access
  flows:
  - authorizationCode
  scope: scope-1
slug: optum-scopes
source_filename: optum-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/optum-attachment-openapi.yml, openapi/optum-auth-referral-submission-api-openapi.yml,\n  openapi/optum-auth-referral-submission-health-check-openapi.yml, openapi/optum-benefit-check-api-openapi.yml,\n  openapi/optum-claim-actions-api-openapi.yml, openapi/optum-claim-actions-health-check-openapi.yml,\n  openapi/optum-claim-inquiry-api-openapi.yml, openapi/optum-claim-inquiry-health-check-openapi.yml,\n  openapi/optum-claim-pre-check-api-openapi.yml, openapi/optum-dental-attachment-api-openapi.yml,\n  openapi/optum-document-search-api-openapi.yml, openapi/optum-document-search-health-check-openapi.yml,\n  openapi/optum-edi-enrollment-v1-openapi.yml, openapi/optum-eligibility-pre-service-health-check-openapi.yml,\n  openapi/optum-enhanced-eligibility-api-openapi.yml, openapi/optum-formatting-rule-api-openapi.yml,\n  openapi/optum-ncc-data-acquisition-api-openapi.yml, openapi/optum-optum-real-health-check-api-openapi.yml,\n\
  \  openapi/optum-optum-real-pre-service-eligibility-api-openapi.yml, openapi/optum-optum-real-time-econtent-web-services-openapi.yml,\n  openapi/optum-patient-benefit-check-health-check-openapi.yml, openapi/optum-real-prior-authorization-api-openapi.yml,\n  openapi/optum-real-provider-access-api-openapi.yml, openapi/optum-submitter-api-openapi.yml,\n  openapi/optum-telecom-formatter-api-openapi.yml\nschemes:\n- name: oAuth\n  source: openapi/optum-attachment-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-auth-referral-submission-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-auth-referral-submission-health-check-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-benefit-check-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-claim-actions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-claim-actions-health-check-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/v2/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-claim-inquiry-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials\
  \ grant flow.\n- name: oAuth\n  source: openapi/optum-claim-inquiry-health-check-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-claim-pre-check-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/v2/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: Bearer\n  source: openapi/optum-dental-attachment-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: '{{baseUrl}}/apip/auth/v2/token'\n- name: oAuth\n  source: openapi/optum-document-search-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-document-search-health-check-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oauth2\n  source: openapi/optum-edi-enrollment-v1-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox-apigw.optum.com/apip/auth/sntl/v1/token\n- name: oAuth\n  source: openapi/optum-eligibility-pre-service-health-check-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-enhanced-eligibility-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/v2/token\n  description: This API uses OAuth 2 with the client_credentials grant flow. [More info](https://api.example.com/docs/auth)\n- name: oauth2_security\n  source: openapi/optum-formatting-rule-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://idx-stage.linkhealth.com/auth/realms/developer-platform/protocol/openid-connect/token\n\
  - name: ncc_auth\n  source: openapi/optum-ncc-data-acquisition-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://idx.linkhealth.com/auth\n    tokenUrl: https://idx.linkhealth.com/auth/token\n- name: oAuth\n  source: openapi/optum-optum-real-health-check-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/v2/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-optum-real-pre-service-eligibility-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: ws_auth\n  source: openapi/optum-optum-real-time-econtent-web-services-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://idx.linkhealth.com/auth\n    tokenUrl: https://idx.linkhealth.com/auth/token\n- name: oAuth\n  source: openapi/optum-patient-benefit-check-health-check-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-real-prior-authorization-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/v2/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-real-provider-access-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/v2/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oAuth\n  source: openapi/optum-submitter-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /apip/auth/sntl/v1/token\n  description: This API uses OAuth 2 with the client_credentials grant flow.\n- name: oauth2_security\n  source: openapi/optum-telecom-formatter-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://idx-stage.linkhealth.com/auth/realms/developer-platform/protocol/openid-connect/token\n\
  scopes:\n- scope: create_coveragediscovery\n  description: submit a new coverage discovery task\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/optum-attachment-openapi.yml\n  - openapi/optum-auth-referral-submission-api-openapi.yml\n  - openapi/optum-auth-referral-submission-health-check-openapi.yml\n  - openapi/optum-benefit-check-api-openapi.yml\n  - openapi/optum-claim-actions-api-openapi.yml\n  - openapi/optum-claim-actions-health-check-openapi.yml\n  - openapi/optum-claim-inquiry-api-openapi.yml\n  - openapi/optum-claim-inquiry-health-check-openapi.yml\n  - openapi/optum-claim-pre-check-api-openapi.yml\n  - openapi/optum-document-search-api-openapi.yml\n  - openapi/optum-document-search-health-check-openapi.yml\n  - openapi/optum-eligibility-pre-service-health-check-openapi.yml\n  - openapi/optum-enhanced-eligibility-api-openapi.yml\n  - openapi/optum-optum-real-health-check-api-openapi.yml\n  - openapi/optum-optum-real-pre-service-eligibility-api-openapi.yml\n  - openapi/optum-patient-benefit-check-health-check-openapi.yml\n\
  \  - openapi/optum-real-prior-authorization-api-openapi.yml\n  - openapi/optum-real-provider-access-api-openapi.yml\n  - openapi/optum-submitter-api-openapi.yml\n- scope: create_txn\n  description: submit a new transaction request\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/optum-attachment-openapi.yml\n  - openapi/optum-auth-referral-submission-api-openapi.yml\n  - openapi/optum-auth-referral-submission-health-check-openapi.yml\n  - openapi/optum-benefit-check-api-openapi.yml\n  - openapi/optum-claim-actions-api-openapi.yml\n  - openapi/optum-claim-actions-health-check-openapi.yml\n  - openapi/optum-claim-inquiry-api-openapi.yml\n  - openapi/optum-claim-inquiry-health-check-openapi.yml\n  - openapi/optum-claim-pre-check-api-openapi.yml\n  - openapi/optum-document-search-api-openapi.yml\n  - openapi/optum-document-search-health-check-openapi.yml\n  - openapi/optum-eligibility-pre-service-health-check-openapi.yml\n  - openapi/optum-enhanced-eligibility-api-openapi.yml\n  -\
  \ openapi/optum-optum-real-health-check-api-openapi.yml\n  - openapi/optum-optum-real-pre-service-eligibility-api-openapi.yml\n  - openapi/optum-patient-benefit-check-health-check-openapi.yml\n  - openapi/optum-real-prior-authorization-api-openapi.yml\n  - openapi/optum-real-provider-access-api-openapi.yml\n  - openapi/optum-submitter-api-openapi.yml\n- scope: profile\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/optum-edi-enrollment-v1-openapi.yml\n- scope: read_coveragediscovery\n  description: read coverage discovery tasks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/optum-attachment-openapi.yml\n  - openapi/optum-auth-referral-submission-api-openapi.yml\n  - openapi/optum-auth-referral-submission-health-check-openapi.yml\n  - openapi/optum-benefit-check-api-openapi.yml\n  - openapi/optum-claim-actions-api-openapi.yml\n  - openapi/optum-claim-actions-health-check-openapi.yml\n  - openapi/optum-claim-inquiry-api-openapi.yml\n  - openapi/optum-claim-inquiry-health-check-openapi.yml\n\
  \  - openapi/optum-claim-pre-check-api-openapi.yml\n  - openapi/optum-document-search-api-openapi.yml\n  - openapi/optum-document-search-health-check-openapi.yml\n  - openapi/optum-eligibility-pre-service-health-check-openapi.yml\n  - openapi/optum-enhanced-eligibility-api-openapi.yml\n  - openapi/optum-optum-real-health-check-api-openapi.yml\n  - openapi/optum-optum-real-pre-service-eligibility-api-openapi.yml\n  - openapi/optum-patient-benefit-check-health-check-openapi.yml\n  - openapi/optum-real-prior-authorization-api-openapi.yml\n  - openapi/optum-real-provider-access-api-openapi.yml\n  - openapi/optum-submitter-api-openapi.yml\n- scope: read_healthcheck\n  description: check the status of the system\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/optum-attachment-openapi.yml\n  - openapi/optum-auth-referral-submission-api-openapi.yml\n  - openapi/optum-auth-referral-submission-health-check-openapi.yml\n  - openapi/optum-benefit-check-api-openapi.yml\n  - openapi/optum-claim-actions-api-openapi.yml\n\
  \  - openapi/optum-claim-actions-health-check-openapi.yml\n  - openapi/optum-claim-inquiry-api-openapi.yml\n  - openapi/optum-claim-inquiry-health-check-openapi.yml\n  - openapi/optum-claim-pre-check-api-openapi.yml\n  - openapi/optum-document-search-api-openapi.yml\n  - openapi/optum-document-search-health-check-openapi.yml\n  - openapi/optum-eligibility-pre-service-health-check-openapi.yml\n  - openapi/optum-enhanced-eligibility-api-openapi.yml\n  - openapi/optum-optum-real-health-check-api-openapi.yml\n  - openapi/optum-optum-real-pre-service-eligibility-api-openapi.yml\n  - openapi/optum-patient-benefit-check-health-check-openapi.yml\n  - openapi/optum-real-prior-authorization-api-openapi.yml\n  - openapi/optum-real-provider-access-api-openapi.yml\n  - openapi/optum-submitter-api-openapi.yml\n- scope: read_txn\n  description: read transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/optum-attachment-openapi.yml\n  - openapi/optum-auth-referral-submission-api-openapi.yml\n\
  \  - openapi/optum-auth-referral-submission-health-check-openapi.yml\n  - openapi/optum-benefit-check-api-openapi.yml\n  - openapi/optum-claim-actions-api-openapi.yml\n  - openapi/optum-claim-actions-health-check-openapi.yml\n  - openapi/optum-claim-inquiry-api-openapi.yml\n  - openapi/optum-claim-inquiry-health-check-openapi.yml\n  - openapi/optum-claim-pre-check-api-openapi.yml\n  - openapi/optum-document-search-api-openapi.yml\n  - openapi/optum-document-search-health-check-openapi.yml\n  - openapi/optum-eligibility-pre-service-health-check-openapi.yml\n  - openapi/optum-enhanced-eligibility-api-openapi.yml\n  - openapi/optum-optum-real-health-check-api-openapi.yml\n  - openapi/optum-optum-real-pre-service-eligibility-api-openapi.yml\n  - openapi/optum-patient-benefit-check-health-check-openapi.yml\n  - openapi/optum-real-prior-authorization-api-openapi.yml\n  - openapi/optum-real-provider-access-api-openapi.yml\n  - openapi/optum-submitter-api-openapi.yml\n- scope: scope-1\n  description:\
  \ required scope for API access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/optum-ncc-data-acquisition-api-openapi.yml\n  - openapi/optum-optum-real-time-econtent-web-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/scopes/optum-scopes.yml
summary_line: 7 scopes · clientCredentials/authorizationCode
tags:
- Company
- Healthcare
- Health Insurance
- Claims
- Eligibility
- FHIR
- Interoperability
- Pharmacy
- EDI
- X12
- Payments
- Prior Authorization
- Clearinghouse
- Revenue Cycle
- Dental
- Da Vinci
- Patient Access
- Remittance
- Attachments
- Payer Directory
token_urls:
- /apip/auth/sntl/v1/token
- /apip/auth/v2/token
- '{{baseUrl}}/apip/auth/v2/token'
- https://sandbox-apigw.optum.com/apip/auth/sntl/v1/token
- https://idx-stage.linkhealth.com/auth/realms/developer-platform/protocol/openid-connect/token
- https://idx.linkhealth.com/auth/token
---
