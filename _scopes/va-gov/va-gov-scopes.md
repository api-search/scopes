---
api_specs:
- filename: openapi.json
  format: json
  label: VA Facilities API
  slug: va-facilities-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/facilities/v1/openapi.json
- filename: openapi.json
  format: json
  label: VA Forms API
  slug: va-forms-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/forms/v0/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Claims API
  slug: benefits-claims-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-claims/v2/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Intake API
  slug: benefits-intake-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-intake/v1/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Documents API
  slug: benefits-documents-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-documents/v1/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Reference Data API
  slug: benefits-reference-data-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-reference-data/v1/openapi.json
- filename: openapi.json
  format: json
  label: Appeals Status API
  slug: appeals-status-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/appeals-status/v1/openapi.json
- filename: openapi.json
  format: json
  label: Appealable Issues API
  slug: appealable-issues-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/appealable-issues/v0/openapi.json
- filename: openapi.json
  format: json
  label: Legacy Appeals API
  slug: legacy-appeals-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/legacy-appeals/v0/openapi.json
- filename: metadata
  format: yaml
  label: Patient Health API (FHIR)
  slug: patient-health-api
  spec_type: OpenAPI
  url: https://api.va.gov/services/fhir/v0/r4/metadata
- filename: metadata
  format: yaml
  label: Clinical Health API (FHIR)
  slug: clinical-health-api
  spec_type: OpenAPI
  url: https://api.va.gov/services/fhir/v0/r4/metadata
- filename: openapi.json
  format: json
  label: Community Care Eligibility API
  slug: community-care-eligibility-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/community-care-eligibility/v0/openapi.json
- filename: openapi.json
  format: json
  label: Veteran Verification API
  slug: veteran-verification-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/veteran-verification/v2/openapi.json
- filename: openapi.json
  format: json
  label: Veteran Confirmation API
  slug: veteran-confirmation-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/veteran-confirmation/v1/openapi.json
- filename: openapi.json
  format: json
  label: Address Validation API
  slug: address-validation-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/address-validation/v3/openapi.json
- filename: openapi.json
  format: json
  label: Direct Deposit Management API
  slug: direct-deposit-management-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/direct-deposit-management/v1/openapi.json
- filename: openapi.json
  format: json
  label: VA Letter Generator API
  slug: va-letter-generator-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/va-letter-generator/v1/openapi.json
- filename: openapi.json
  format: json
  label: Loan Review API
  slug: loan-review-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/loan-review/v1/openapi.json
authorization_urls:
- https://api.va.gov/oauth2/appeals/v1/authorization
- https://sandbox-api.va.gov/oauth2/appeals/v1/authorization
- https://api.va.gov/oauth2/authorization
- https://sandbox-api.va.gov/oauth2/authorization
- https://api.va.gov/oauth2/veteran-verification/system/v1/authorization
- https://sandbox-api.va.gov/oauth2/veteran-verification/system/v1/authorization
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Va Gov Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'VA Lighthouse publishes 35 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the VA Lighthouse API on a user''s behalf.


  Tokens are issued from https://api.va.gov/oauth2/appeals/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: VA Lighthouse
provider_slug: va-gov
schemes:
- description: 'The authorization model for the Appealable Issues API uses OAuth 2.0/OpenID Connect. The following models are supported: [Authorization Code Grant (ACG)](/explore/api/appealable-issues/authorization-code) and [Client Credentials Grant (CCG)](/explore/api/appealable-issues/client-credentials).'
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.va.gov/oauth2/appeals/system/v1/token
  name: productionOauth
  source: openapi/va-gov-appealable-issues-v0-openapi.json
- description: 'The authorization model for the Appealable Issues API uses OAuth 2.0/OpenID Connect. The following models are supported: [Authorization Code Grant (ACG)](/explore/api/appealable-issues/authorization-code) and [Client Credentials Grant (CCG)](/explore/api/appealable-issues/client-credentials).'
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token
  name: sandboxOauth
  source: openapi/va-gov-appealable-issues-v0-openapi.json
- description: 'The authorization model for the Appeals Status API uses OAuth 2.0/OpenID Connect. The following models are supported: [Authorization Code Grant (ACG)](/explore/api/appeals-status/authorization-code) and [Client Credentials Grant (CCG)](/explore/api/appeals-status/client-credentials).'
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.va.gov/oauth2/appeals/system/v1/token
  name: productionOauth
  source: openapi/va-gov-appeals-status-v1-openapi.json
- description: 'The authorization model for the Appeals Status API uses OAuth 2.0/OpenID Connect. The following models are supported: [Authorization Code Grant (ACG)](/explore/api/appeals-status/authorization-code) and [Client Credentials Grant (CCG)](/explore/api/appeals-status/client-credentials).'
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token
  name: sandboxOauth
  source: openapi/va-gov-appeals-status-v1-openapi.json
- description: This API uses OAuth 2 with the authorization code grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/authorization-code)
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/token
  name: productionOauth
  source: openapi/va-gov-benefits-claims-v1-openapi.json
- description: This API uses OAuth 2 with the authorization code grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/authorization-code)
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/token
  name: sandboxOauth
  source: openapi/va-gov-benefits-claims-v1-openapi.json
- description: This API uses OAuth 2 with the client credential grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/client-credentials)
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/token
  name: productionOauth
  source: openapi/va-gov-benefits-claims-v2-openapi.json
- description: This API uses OAuth 2 with the client credential grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/client-credentials)
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/token
  name: sandboxOauth
  source: openapi/va-gov-benefits-claims-v2-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.va.gov/oauth2/exemplar/system/v1/token
  name: oauth2
  source: openapi/va-gov-benefits-documents-v1-openapi.json
- flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/token
  name: OauthFlow
  source: openapi/va-gov-community-care-eligibility-v0-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.va.gov/oauth2/direct-deposit-management/system/v1/token
  name: OAuth
  source: openapi/va-gov-direct-deposit-management-v1-openapi.json
- description: 'The authorization model for the Legacy Appeals API uses OAuth 2.0/OpenID Connect. The following models are supported: [Authorization Code Grant (ACG)](/explore/api/legacy-appeals/authorization-code) and [Client Credentials Grant (CCG)](/explore/api/legacy-appeals/client-credentials).'
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.va.gov/oauth2/appeals/system/v1/token
  name: productionOauth
  source: openapi/va-gov-legacy-appeals-v0-openapi.json
- description: 'The authorization model for the Legacy Appeals API uses OAuth 2.0/OpenID Connect. The following models are supported: [Authorization Code Grant (ACG)](/explore/api/legacy-appeals/authorization-code) and [Client Credentials Grant (CCG)](/explore/api/legacy-appeals/client-credentials).'
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token
  name: sandboxOauth
  source: openapi/va-gov-legacy-appeals-v0-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://staging-api.va.gov/oauth2/loan-guaranty/system/v1/token
  name: oauth2
  source: openapi/va-gov-loan-review-v1-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.va.gov/oauth2/veteran-letters/system/v1/token
  name: OAuth
  source: openapi/va-gov-va-letter-generator-v1-openapi.json
- description: This API uses OAuth 2.0 with client credentials grant flow and authorization code grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.va.gov/oauth2/veteran-verification/system/v1/token
  - authorizationUrl: https://api.va.gov/oauth2/veteran-verification/system/v1/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/veteran-verification/system/v1/token
  name: productionOauth2
  source: openapi/va-gov-veteran-verification-v2-openapi.json
- description: This API uses OAuth 2.0 with client credentials grant flow and authorization code grant flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.va.gov/oauth2/veteran-verification/system/v1/token
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/veteran-verification/system/v1/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/veteran-verification/system/v1/token
  name: sandboxOauth2
  source: openapi/va-gov-veteran-verification-v2-openapi.json
scope_count: 35
scope_names:
- aca_coverage_restricted.read
- claim.read
- claim.write
- direct-deposit-management.read
- direct-deposit-management.write
- disability_rating.read
- disability_rating_restricted.read
- disability_rating_summary.read
- disability_rating_summary_restricted.read
- documents.read
- documents.write
- enrolled_benefits.read
- flashes.read
- launch.read
- letters.read
- patient/CommunityCareEligibility.read
- permanent_and_total_disability.read
- permanent_and_total_disability_restricted.read
- representative/AppealableIssues.read
- representative/AppealsStatus.read
- representative/LegacyAppeals.read
- service_history.read
- status_restricted.read
- system.loan-review.write
- system/526-pdf.override
- system/526.override
- system/AppealableIssues.read
- system/AppealsStatus.read
- system/LegacyAppeals.read
- system/claim.read
- system/claim.write
- veteran/AppealableIssues.read
- veteran/AppealsStatus.read
- veteran/LegacyAppeals.read
- veteran_status.read
scopes:
- description: Return a Veteran's enrollment status in minimum essential coverage (MEC) as defined by the Affordable Care Act (ACA). (restricted access).
  flows:
  - authorizationCode
  - clientCredentials
  scope: aca_coverage_restricted.read
- description: Retrieve claim data
  flows:
  - authorizationCode
  scope: claim.read
- description: Submit claim data
  flows:
  - authorizationCode
  scope: claim.write
- description: The veteran's access to direct deposit management that provides viewing of current EFT settings.
  flows:
  - clientCredentials
  scope: direct-deposit-management.read
- description: The veteran's access to direct deposit management that provides updating of current EFT settings.
  flows:
  - clientCredentials
  scope: direct-deposit-management.write
- description: Retrieve Disability Rating
  flows:
  - authorizationCode
  - clientCredentials
  scope: disability_rating.read
- description: For approved federal consumers, view a Veteran's VA disability ratings and their effective dates using Social Security number and demographic information.
  flows:
  - authorizationCode
  - clientCredentials
  scope: disability_rating_restricted.read
- description: Retrieve Disability Rating Summary
  flows:
  - authorizationCode
  - clientCredentials
  scope: disability_rating_summary.read
- description: For approved federal consumers, view a Veteran's VA disability rating summary using Social Security number and demographic information.
  flows:
  - clientCredentials
  scope: disability_rating_summary_restricted.read
- description: The Veteran's access to read data about files that have been uploaded.
  flows:
  - clientCredentials
  scope: documents.read
- description: The Veteran's access to upload files that provide verification of eligibility for their benefits.
  flows:
  - clientCredentials
  scope: documents.write
- description: Retrieve Veteran Enrolled Benefits
  flows:
  - authorizationCode
  - clientCredentials
  scope: enrolled_benefits.read
- description: Retrieve Flashes
  flows:
  - authorizationCode
  - clientCredentials
  scope: flashes.read
- description: Retrieve Launch
  flows:
  - clientCredentials
  scope: launch.read
- description: The veteran's access to letters that provide verification of eligibility for their benefits.
  flows:
  - clientCredentials
  scope: letters.read
- description: Community Care Eligibility
  flows:
  - authorizationCode
  scope: patient/CommunityCareEligibility.read
- description: View a Veteran's P&T and IU disability statuses and effective dates.
  flows:
  - authorizationCode
  - clientCredentials
  scope: permanent_and_total_disability.read
- description: Vew a Veteran's P&T and IU disability statuses and effective dates, based on restricted user attributes.
  flows:
  - clientCredentials
  scope: permanent_and_total_disability_restricted.read
- description: Appealable issues info
  flows:
  - authorizationCode
  scope: representative/AppealableIssues.read
- description: Status of appeals and decision reviews
  flows:
  - authorizationCode
  scope: representative/AppealsStatus.read
- description: Legacy appeals info
  flows:
  - authorizationCode
  scope: representative/LegacyAppeals.read
- description: Retrieve Service History
  flows:
  - authorizationCode
  - clientCredentials
  scope: service_history.read
- description: For approved federal consumers, confirm the Veteran status of an individual using Social Security number and demographic information.
  flows:
  - authorizationCode
  - clientCredentials
  scope: status_restricted.read
- description: Transmit loan review documents
  flows:
  - clientCredentials
  scope: system.loan-review.write
- description: ''
  flows: []
  scope: system/526-pdf.override
- description: ''
  flows: []
  scope: system/526.override
- description: Appealable issues info
  flows:
  - clientCredentials
  scope: system/AppealableIssues.read
- description: Status of appeals and decision reviews
  flows:
  - clientCredentials
  scope: system/AppealsStatus.read
- description: Legacy appeals info
  flows:
  - clientCredentials
  scope: system/LegacyAppeals.read
- description: Retrieve claim data
  flows:
  - authorizationCode
  scope: system/claim.read
- description: Submit claim data
  flows:
  - authorizationCode
  scope: system/claim.write
- description: Appealable issues info
  flows:
  - authorizationCode
  scope: veteran/AppealableIssues.read
- description: Status of appeals and decision reviews
  flows:
  - authorizationCode
  scope: veteran/AppealsStatus.read
- description: Legacy appeals info
  flows:
  - authorizationCode
  scope: veteran/LegacyAppeals.read
- description: Retrieve Veteran Status
  flows:
  - authorizationCode
  - clientCredentials
  scope: veteran_status.read
slug: va-gov-scopes
source_filename: va-gov-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/va-gov-appealable-issues-v0-openapi.json, openapi/va-gov-appeals-status-v1-openapi.json,\n  openapi/va-gov-benefits-claims-v1-openapi.json, openapi/va-gov-benefits-claims-v2-openapi.json,\n  openapi/va-gov-benefits-documents-v1-openapi.json, openapi/va-gov-community-care-eligibility-v0-openapi.json,\n  openapi/va-gov-direct-deposit-management-v1-openapi.json, openapi/va-gov-legacy-appeals-v0-openapi.json,\n  openapi/va-gov-loan-review-v1-openapi.json, openapi/va-gov-va-letter-generator-v1-openapi.json,\n  openapi/va-gov-veteran-verification-v2-openapi.json\nschemes:\n- name: productionOauth\n  source: openapi/va-gov-appealable-issues-v0-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://api.va.gov/oauth2/appeals/system/v1/token\n  description:\
  \ 'The authorization model for the Appealable Issues API uses OAuth 2.0/OpenID\n    Connect. The following models are supported: [Authorization Code Grant (ACG)](/explore/api/appealable-issues/authorization-code)\n    and [Client Credentials Grant (CCG)](/explore/api/appealable-issues/client-credentials).'\n- name: sandboxOauth\n  source: openapi/va-gov-appealable-issues-v0-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token\n  description: 'The authorization model for the Appealable Issues API uses OAuth 2.0/OpenID\n    Connect. The following models are supported: [Authorization Code Grant (ACG)](/explore/api/appealable-issues/authorization-code)\n    and [Client Credentials Grant (CCG)](/explore/api/appealable-issues/client-credentials).'\n\
  - name: productionOauth\n  source: openapi/va-gov-appeals-status-v1-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://api.va.gov/oauth2/appeals/system/v1/token\n  description: 'The authorization model for the Appeals Status API uses OAuth 2.0/OpenID Connect.\n    The following models are supported: [Authorization Code Grant (ACG)](/explore/api/appeals-status/authorization-code)\n    and [Client Credentials Grant (CCG)](/explore/api/appeals-status/client-credentials).'\n- name: sandboxOauth\n  source: openapi/va-gov-appeals-status-v1-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token\n\
  \  description: 'The authorization model for the Appeals Status API uses OAuth 2.0/OpenID Connect.\n    The following models are supported: [Authorization Code Grant (ACG)](/explore/api/appeals-status/authorization-code)\n    and [Client Credentials Grant (CCG)](/explore/api/appeals-status/client-credentials).'\n- name: productionOauth\n  source: openapi/va-gov-benefits-claims-v1-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/authorization\n    tokenUrl: https://api.va.gov/oauth2/token\n  description: This API uses OAuth 2 with the authorization code grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/authorization-code)\n- name: sandboxOauth\n  source: openapi/va-gov-benefits-claims-v1-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/token\n  description: This API uses OAuth 2 with the\
  \ authorization code grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/authorization-code)\n- name: productionOauth\n  source: openapi/va-gov-benefits-claims-v2-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/authorization\n    tokenUrl: https://api.va.gov/oauth2/token\n  description: This API uses OAuth 2 with the client credential grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/client-credentials)\n- name: sandboxOauth\n  source: openapi/va-gov-benefits-claims-v2-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/token\n  description: This API uses OAuth 2 with the client credential grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/client-credentials)\n- name: oauth2\n  source: openapi/va-gov-benefits-documents-v1-openapi.json\n  flows:\n\
  \  - flow: clientCredentials\n    tokenUrl: https://api.va.gov/oauth2/exemplar/system/v1/token\n- name: OauthFlow\n  source: openapi/va-gov-community-care-eligibility-v0-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/token\n- name: OAuth\n  source: openapi/va-gov-direct-deposit-management-v1-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.va.gov/oauth2/direct-deposit-management/system/v1/token\n- name: productionOauth\n  source: openapi/va-gov-legacy-appeals-v0-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://api.va.gov/oauth2/appeals/system/v1/token\n  description: 'The authorization model for the Legacy Appeals API uses OAuth 2.0/OpenID Connect.\n\
  \    The following models are supported: [Authorization Code Grant (ACG)](/explore/api/legacy-appeals/authorization-code)\n    and [Client Credentials Grant (CCG)](/explore/api/legacy-appeals/client-credentials).'\n- name: sandboxOauth\n  source: openapi/va-gov-legacy-appeals-v0-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token\n  description: 'The authorization model for the Legacy Appeals API uses OAuth 2.0/OpenID Connect.\n    The following models are supported: [Authorization Code Grant (ACG)](/explore/api/legacy-appeals/authorization-code)\n    and [Client Credentials Grant (CCG)](/explore/api/legacy-appeals/client-credentials).'\n- name: oauth2\n  source: openapi/va-gov-loan-review-v1-openapi.json\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://staging-api.va.gov/oauth2/loan-guaranty/system/v1/token\n- name: OAuth\n  source: openapi/va-gov-va-letter-generator-v1-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.va.gov/oauth2/veteran-letters/system/v1/token\n- name: productionOauth2\n  source: openapi/va-gov-veteran-verification-v2-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.va.gov/oauth2/veteran-verification/system/v1/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/veteran-verification/system/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/veteran-verification/system/v1/token\n  description: This API uses OAuth 2.0 with client credentials grant flow and authorization\n    code grant flow.\n- name: sandboxOauth2\n  source: openapi/va-gov-veteran-verification-v2-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.va.gov/oauth2/veteran-verification/system/v1/token\n  - flow:\
  \ authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/veteran-verification/system/v1/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/veteran-verification/system/v1/token\n  description: This API uses OAuth 2.0 with client credentials grant flow and authorization\n    code grant flow\nscopes:\n- scope: aca_coverage_restricted.read\n  description: Return a Veteran's enrollment status in minimum essential coverage (MEC) as defined\n    by the Affordable Care Act (ACA).  (restricted access).\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- scope: claim.read\n  description: Retrieve claim data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-gov-benefits-claims-v1-openapi.json\n- scope: claim.write\n  description: Submit claim data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-gov-benefits-claims-v1-openapi.json\n- scope: direct-deposit-management.read\n\
  \  description: The veteran's access to direct deposit management that provides viewing of current\n    EFT settings.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-gov-direct-deposit-management-v1-openapi.json\n- scope: direct-deposit-management.write\n  description: The veteran's access to direct deposit management that provides updating of current\n    EFT settings.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-gov-direct-deposit-management-v1-openapi.json\n- scope: disability_rating.read\n  description: Retrieve Disability Rating\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- scope: disability_rating_restricted.read\n  description: For approved federal consumers, view a Veteran's VA disability ratings and their\n    effective dates using Social Security number and demographic information.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n\
  - scope: disability_rating_summary.read\n  description: Retrieve Disability Rating Summary\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- scope: disability_rating_summary_restricted.read\n  description: For approved federal consumers, view a Veteran's VA disability rating summary\n    using Social Security number and demographic information.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- scope: documents.read\n  description: The Veteran's access to read data about files that have been uploaded.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-gov-benefits-documents-v1-openapi.json\n- scope: documents.write\n  description: The Veteran's access to upload files that provide verification of eligibility\n    for their benefits.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-gov-benefits-documents-v1-openapi.json\n- scope: enrolled_benefits.read\n\
  \  description: Retrieve Veteran Enrolled Benefits\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- scope: flashes.read\n  description: Retrieve Flashes\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- scope: launch.read\n  description: Retrieve Launch\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- scope: letters.read\n  description: The veteran's access to letters that provide verification of eligibility for\n    their benefits.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-gov-va-letter-generator-v1-openapi.json\n- scope: patient/CommunityCareEligibility.read\n  description: Community Care Eligibility\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-gov-community-care-eligibility-v0-openapi.json\n- scope: permanent_and_total_disability.read\n  description:\
  \ View a Veteran's P&T and IU disability statuses and effective dates.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- scope: permanent_and_total_disability_restricted.read\n  description: Vew a Veteran's P&T and IU disability statuses and effective dates, based on\n    restricted user attributes.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- scope: representative/AppealableIssues.read\n  description: Appealable issues info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-gov-appealable-issues-v0-openapi.json\n- scope: representative/AppealsStatus.read\n  description: Status of appeals and decision reviews\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-gov-appeals-status-v1-openapi.json\n- scope: representative/LegacyAppeals.read\n  description: Legacy appeals info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-gov-legacy-appeals-v0-openapi.json\n\
  - scope: service_history.read\n  description: Retrieve Service History\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- scope: status_restricted.read\n  description: For approved federal consumers, confirm the Veteran status of an individual using\n    Social Security number and demographic information.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- scope: system.loan-review.write\n  description: Transmit loan review documents\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-gov-loan-review-v1-openapi.json\n- scope: system/526-pdf.override\n  sources:\n  - openapi/va-gov-benefits-claims-v2-openapi.json\n- scope: system/526.override\n  sources:\n  - openapi/va-gov-benefits-claims-v2-openapi.json\n- scope: system/AppealableIssues.read\n  description: Appealable issues info\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/va-gov-appealable-issues-v0-openapi.json\n- scope: system/AppealsStatus.read\n  description: Status of appeals and decision reviews\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-gov-appeals-status-v1-openapi.json\n- scope: system/LegacyAppeals.read\n  description: Legacy appeals info\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-gov-legacy-appeals-v0-openapi.json\n- scope: system/claim.read\n  description: Retrieve claim data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-gov-benefits-claims-v2-openapi.json\n- scope: system/claim.write\n  description: Submit claim data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-gov-benefits-claims-v2-openapi.json\n- scope: veteran/AppealableIssues.read\n  description: Appealable issues info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-gov-appealable-issues-v0-openapi.json\n- scope: veteran/AppealsStatus.read\n  description: Status of appeals and decision reviews\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-gov-appeals-status-v1-openapi.json\n- scope: veteran/LegacyAppeals.read\n  description: Legacy appeals info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-gov-legacy-appeals-v0-openapi.json\n- scope: veteran_status.read\n  description: Retrieve Veteran Status\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/va-gov/refs/heads/main/scopes/va-gov-scopes.yml
summary_line: 35 scopes · authorizationCode/clientCredentials
tags:
- Government
- Veterans Affairs
- Veterans
- Healthcare
- Benefits
- FHIR
- Open Data
- Federal
token_urls:
- https://api.va.gov/oauth2/appeals/v1/token
- https://api.va.gov/oauth2/appeals/system/v1/token
- https://sandbox-api.va.gov/oauth2/appeals/v1/token
- https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token
- https://api.va.gov/oauth2/token
- https://sandbox-api.va.gov/oauth2/token
- https://api.va.gov/oauth2/exemplar/system/v1/token
- https://api.va.gov/oauth2/direct-deposit-management/system/v1/token
- https://staging-api.va.gov/oauth2/loan-guaranty/system/v1/token
- https://api.va.gov/oauth2/veteran-letters/system/v1/token
- https://api.va.gov/oauth2/veteran-verification/system/v1/token
- https://sandbox-api.va.gov/oauth2/veteran-verification/system/v1/token
---
