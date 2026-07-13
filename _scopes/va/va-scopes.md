---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Benefits Intake API
  slug: benefits-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/department-of-veterans-affairs/vets-api-clients/master/services/benefits-intake/openapi.yaml
authorization_urls:
- https://api.va.gov/oauth2/appeals/v1/authorization
- https://sandbox-api.va.gov/oauth2/appeals/v1/authorization
- https://api.va.gov/oauth2/authorization
- https://sandbox-api.va.gov/oauth2/authorization
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Va Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Veterans Affairs publishes 35 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Veterans Affairs API on a user''s behalf.


  Tokens are issued from https://api.va.gov/oauth2/appeals/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Veterans Affairs
provider_slug: va
schemes:
- description: 'The authentication model for the Appealable Issues API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/appealable-issues/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/appealable-issues/client-credentials).'
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: To get production access, you must either work for VA or have specific VA agreements in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).
  name: productionOauth
  source: openapi/va-appealable-issues-openapi.json
- description: 'The authentication model for the Appealable Issues API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/appealable-issues/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/appealable-issues/client-credentials).'
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token
  name: sandboxOauth
  source: openapi/va-appealable-issues-openapi.json
- description: 'The authentication model for the Appeals Status API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/appeals-status/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/appeals-status/client-credentials).'
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: To get production access, you must either work for VA or have specific VA agreements in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).
  name: productionOauth
  source: openapi/va-appeals-status-openapi.json
- description: 'The authentication model for the Appeals Status API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/appeals-status/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/appeals-status/client-credentials).'
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token
  name: sandboxOauth
  source: openapi/va-appeals-status-openapi.json
- description: This API uses OAuth 2 with the client credential grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/client-credentials)
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/token
  name: productionOauth
  source: openapi/va-claims-api-openapi.json
- description: This API uses OAuth 2 with the client credential grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/client-credentials)
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/token
  name: sandboxOauth
  source: openapi/va-claims-api-openapi.json
- description: 'The authentication model for the Higher-Level Reviews API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/higher-level-reviews/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/higher-level-reviews/client-credentials).'
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: To get production access, you must either work for VA or have specific VA agreements in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).
  name: productionOauth
  source: openapi/va-higher-level-reviews-openapi.json
- description: 'The authentication model for the Higher-Level Reviews API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/higher-level-reviews/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/higher-level-reviews/client-credentials).'
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token
  name: sandboxOauth
  source: openapi/va-higher-level-reviews-openapi.json
- description: 'The authentication model for the Legacy Appeals API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/legacy-appeals/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/legacy-appeals/client-credentials).'
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: To get production access, you must either work for VA or have specific VA agreements in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).
  name: productionOauth
  source: openapi/va-legacy-appeals-openapi.json
- description: 'The authentication model for the Legacy Appeals API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/legacy-appeals/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/legacy-appeals/client-credentials).'
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token
  name: sandboxOauth
  source: openapi/va-legacy-appeals-openapi.json
- description: 'The authentication model for the Notice of Disagreements API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/notice-of-disagreements/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/notice-of-disagreements/client-credentials).'
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: To get production access, you must either work for VA or have specific VA agreements in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).
  name: productionOauth
  source: openapi/va-notice-of-disagreements-openapi.json
- description: 'The authentication model for the Notice of Disagreements API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/notice-of-disagreements/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/notice-of-disagreements/client-credentials).'
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token
  name: sandboxOauth
  source: openapi/va-notice-of-disagreements-openapi.json
- description: 'The authentication model for the Supplemental Claims API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/supplemental-claims/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/supplemental-claims/client-credentials).'
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: To get production access, you must either work for VA or have specific VA agreements in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).
  name: productionOauth
  source: openapi/va-supplemental-claims-openapi.json
- description: 'The authentication model for the Supplemental Claims API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/supplemental-claims/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/supplemental-claims/client-credentials).'
  flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token
  name: sandboxOauth
  source: openapi/va-supplemental-claims-openapi.json
scope_count: 35
scope_names:
- representative/AppealableIssues.read
- representative/AppealsStatus.read
- representative/HigherLevelReviews.read
- representative/HigherLevelReviews.write
- representative/LegacyAppeals.read
- representative/NoticeOfDisagreements.read
- representative/NoticeOfDisagreements.write
- representative/SupplementalClaims.read
- representative/SupplementalClaims.write
- representative/appeals.read
- representative/appeals.write
- system/AppealableIssues.read
- system/AppealsStatus.read
- system/HigherLevelReviews.read
- system/HigherLevelReviews.write
- system/LegacyAppeals.read
- system/NoticeOfDisagreements.read
- system/NoticeOfDisagreements.write
- system/SupplementalClaims.read
- system/SupplementalClaims.write
- system/appeals.read
- system/appeals.write
- system/claim.read
- system/claim.write
- veteran/AppealableIssues.read
- veteran/AppealsStatus.read
- veteran/HigherLevelReviews.read
- veteran/HigherLevelReviews.write
- veteran/LegacyAppeals.read
- veteran/NoticeOfDisagreements.read
- veteran/NoticeOfDisagreements.write
- veteran/SupplementalClaims.read
- veteran/SupplementalClaims.write
- veteran/appeals.read
- veteran/appeals.write
scopes:
- description: Appealable issues info
  flows:
  - authorizationCode
  scope: representative/AppealableIssues.read
- description: Status of appeals and decision reviews
  flows:
  - authorizationCode
  scope: representative/AppealsStatus.read
- description: Higher-Level Reviews info
  flows:
  - authorizationCode
  scope: representative/HigherLevelReviews.read
- description: Ability to submit Higher-Level Reviews
  flows:
  - authorizationCode
  scope: representative/HigherLevelReviews.write
- description: Legacy appeals info
  flows:
  - authorizationCode
  scope: representative/LegacyAppeals.read
- description: Board Appeals info
  flows:
  - authorizationCode
  scope: representative/NoticeOfDisagreements.read
- description: Ability to submit Board Appeals
  flows:
  - authorizationCode
  scope: representative/NoticeOfDisagreements.write
- description: Supplemental Claims info
  flows:
  - authorizationCode
  scope: representative/SupplementalClaims.read
- description: Ability to submit Supplemental Claims
  flows:
  - authorizationCode
  scope: representative/SupplementalClaims.write
- description: Appeals info
  flows:
  - authorizationCode
  scope: representative/appeals.read
- description: Ability to submit appeals
  flows:
  - authorizationCode
  scope: representative/appeals.write
- description: Appealable issues info
  flows:
  - clientCredentials
  scope: system/AppealableIssues.read
- description: Status of appeals and decision reviews
  flows:
  - clientCredentials
  scope: system/AppealsStatus.read
- description: Higher-Level Reviews info
  flows:
  - clientCredentials
  scope: system/HigherLevelReviews.read
- description: Ability to submit Higher-Level Reviews
  flows:
  - clientCredentials
  scope: system/HigherLevelReviews.write
- description: Legacy appeals info
  flows:
  - clientCredentials
  scope: system/LegacyAppeals.read
- description: Board Appeals info
  flows:
  - clientCredentials
  scope: system/NoticeOfDisagreements.read
- description: Ability to submit Board Appeals
  flows:
  - clientCredentials
  scope: system/NoticeOfDisagreements.write
- description: Supplemental Claims info
  flows:
  - clientCredentials
  scope: system/SupplementalClaims.read
- description: Ability to submit Supplemental Claims
  flows:
  - clientCredentials
  scope: system/SupplementalClaims.write
- description: Appeals info
  flows:
  - clientCredentials
  scope: system/appeals.read
- description: Ability to submit appeals
  flows:
  - clientCredentials
  scope: system/appeals.write
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
- description: Higher-Level Reviews info
  flows:
  - authorizationCode
  scope: veteran/HigherLevelReviews.read
- description: Ability to submit Higher-Level Reviews
  flows:
  - authorizationCode
  scope: veteran/HigherLevelReviews.write
- description: Legacy appeals info
  flows:
  - authorizationCode
  scope: veteran/LegacyAppeals.read
- description: Board Appeals info
  flows:
  - authorizationCode
  scope: veteran/NoticeOfDisagreements.read
- description: Ability to submit Board Appeals
  flows:
  - authorizationCode
  scope: veteran/NoticeOfDisagreements.write
- description: Supplemental Claims info
  flows:
  - authorizationCode
  scope: veteran/SupplementalClaims.read
- description: Ability to submit Supplemental Claims
  flows:
  - authorizationCode
  scope: veteran/SupplementalClaims.write
- description: Appeals info
  flows:
  - authorizationCode
  scope: veteran/appeals.read
- description: Ability to submit appeals
  flows:
  - authorizationCode
  scope: veteran/appeals.write
slug: va-scopes
source_filename: va-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/va-appealable-issues-openapi.json, openapi/va-appeals-status-openapi.json, openapi/va-claims-api-openapi.json,\n  openapi/va-higher-level-reviews-openapi.json, openapi/va-legacy-appeals-openapi.json, openapi/va-notice-of-disagreements-openapi.json,\n  openapi/va-supplemental-claims-openapi.json\nschemes:\n- name: productionOauth\n  source: openapi/va-appealable-issues-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: To get production access, you must either work for VA or have specific VA agreements\n      in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).\n  description: 'The authentication model for the Appealable Issues API uses OAuth 2.0/OpenID\n    Connect. The following authorization models are\
  \ supported: [Authorization code flow](https://developer.va.gov/explore/api/appealable-issues/authorization-code)\n    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/appealable-issues/client-credentials).'\n- name: sandboxOauth\n  source: openapi/va-appealable-issues-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token\n  description: 'The authentication model for the Appealable Issues API uses OAuth 2.0/OpenID\n    Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/appealable-issues/authorization-code)\n    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/appealable-issues/client-credentials).'\n- name: productionOauth\n\
  \  source: openapi/va-appeals-status-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: To get production access, you must either work for VA or have specific VA agreements\n      in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).\n  description: 'The authentication model for the Appeals Status API uses OAuth 2.0/OpenID Connect.\n    The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/appeals-status/authorization-code)\n    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/appeals-status/client-credentials).'\n- name: sandboxOauth\n  source: openapi/va-appeals-status-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization\n\
  \    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token\n  description: 'The authentication model for the Appeals Status API uses OAuth 2.0/OpenID Connect.\n    The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/appeals-status/authorization-code)\n    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/appeals-status/client-credentials).'\n- name: productionOauth\n  source: openapi/va-claims-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/authorization\n    tokenUrl: https://api.va.gov/oauth2/token\n  description: This API uses OAuth 2 with the client credential grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/client-credentials)\n- name: sandboxOauth\n  source: openapi/va-claims-api-openapi.json\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/token\n  description: This API uses OAuth 2 with the client credential grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/client-credentials)\n- name: productionOauth\n  source: openapi/va-higher-level-reviews-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: To get production access, you must either work for VA or have specific VA agreements\n      in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).\n  description: 'The authentication model for the Higher-Level Reviews API uses OAuth 2.0/OpenID\n    Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/higher-level-reviews/authorization-code)\n\
  \    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/higher-level-reviews/client-credentials).'\n- name: sandboxOauth\n  source: openapi/va-higher-level-reviews-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token\n  description: 'The authentication model for the Higher-Level Reviews API uses OAuth 2.0/OpenID\n    Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/higher-level-reviews/authorization-code)\n    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/higher-level-reviews/client-credentials).'\n- name: productionOauth\n  source: openapi/va-legacy-appeals-openapi.json\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: To get production access, you must either work for VA or have specific VA agreements\n      in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).\n  description: 'The authentication model for the Legacy Appeals API uses OAuth 2.0/OpenID Connect.\n    The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/legacy-appeals/authorization-code)\n    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/legacy-appeals/client-credentials).'\n- name: sandboxOauth\n  source: openapi/va-legacy-appeals-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n\
  \    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token\n  description: 'The authentication model for the Legacy Appeals API uses OAuth 2.0/OpenID Connect.\n    The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/legacy-appeals/authorization-code)\n    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/legacy-appeals/client-credentials).'\n- name: productionOauth\n  source: openapi/va-notice-of-disagreements-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: To get production access, you must either work for VA or have specific VA agreements\n      in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).\n  description: 'The authentication model for the Notice of Disagreements\
  \ API uses OAuth 2.0/OpenID\n    Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/notice-of-disagreements/authorization-code)\n    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/notice-of-disagreements/client-credentials).'\n- name: sandboxOauth\n  source: openapi/va-notice-of-disagreements-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token\n  description: 'The authentication model for the Notice of Disagreements API uses OAuth 2.0/OpenID\n    Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/notice-of-disagreements/authorization-code)\n    and [Client Credentials\
  \ Grant (CCG)](https://developer.va.gov/explore/api/notice-of-disagreements/client-credentials).'\n- name: productionOauth\n  source: openapi/va-supplemental-claims-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: To get production access, you must either work for VA or have specific VA agreements\n      in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).\n  description: 'The authentication model for the Supplemental Claims API uses OAuth 2.0/OpenID\n    Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/supplemental-claims/authorization-code)\n    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/supplemental-claims/client-credentials).'\n- name: sandboxOauth\n  source: openapi/va-supplemental-claims-openapi.json\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/appeals/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token\n  description: 'The authentication model for the Supplemental Claims API uses OAuth 2.0/OpenID\n    Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/supplemental-claims/authorization-code)\n    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/supplemental-claims/client-credentials).'\nscopes:\n- scope: representative/AppealableIssues.read\n  description: Appealable issues info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-appealable-issues-openapi.json\n- scope: representative/AppealsStatus.read\n  description: Status of appeals and decision reviews\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/va-appeals-status-openapi.json\n- scope: representative/HigherLevelReviews.read\n  description: Higher-Level Reviews info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-higher-level-reviews-openapi.json\n- scope: representative/HigherLevelReviews.write\n  description: Ability to submit Higher-Level Reviews\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-higher-level-reviews-openapi.json\n- scope: representative/LegacyAppeals.read\n  description: Legacy appeals info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-legacy-appeals-openapi.json\n- scope: representative/NoticeOfDisagreements.read\n  description: Board Appeals info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-notice-of-disagreements-openapi.json\n- scope: representative/NoticeOfDisagreements.write\n  description: Ability to submit Board Appeals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-notice-of-disagreements-openapi.json\n- scope:\
  \ representative/SupplementalClaims.read\n  description: Supplemental Claims info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-supplemental-claims-openapi.json\n- scope: representative/SupplementalClaims.write\n  description: Ability to submit Supplemental Claims\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-supplemental-claims-openapi.json\n- scope: representative/appeals.read\n  description: Appeals info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-appealable-issues-openapi.json\n  - openapi/va-appeals-status-openapi.json\n  - openapi/va-higher-level-reviews-openapi.json\n  - openapi/va-legacy-appeals-openapi.json\n  - openapi/va-notice-of-disagreements-openapi.json\n  - openapi/va-supplemental-claims-openapi.json\n- scope: representative/appeals.write\n  description: Ability to submit appeals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-higher-level-reviews-openapi.json\n  - openapi/va-notice-of-disagreements-openapi.json\n\
  \  - openapi/va-supplemental-claims-openapi.json\n- scope: system/AppealableIssues.read\n  description: Appealable issues info\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-appealable-issues-openapi.json\n- scope: system/AppealsStatus.read\n  description: Status of appeals and decision reviews\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-appeals-status-openapi.json\n- scope: system/HigherLevelReviews.read\n  description: Higher-Level Reviews info\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-higher-level-reviews-openapi.json\n- scope: system/HigherLevelReviews.write\n  description: Ability to submit Higher-Level Reviews\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-higher-level-reviews-openapi.json\n- scope: system/LegacyAppeals.read\n  description: Legacy appeals info\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-legacy-appeals-openapi.json\n- scope: system/NoticeOfDisagreements.read\n  description: Board Appeals\
  \ info\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-notice-of-disagreements-openapi.json\n- scope: system/NoticeOfDisagreements.write\n  description: Ability to submit Board Appeals\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-notice-of-disagreements-openapi.json\n- scope: system/SupplementalClaims.read\n  description: Supplemental Claims info\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-supplemental-claims-openapi.json\n- scope: system/SupplementalClaims.write\n  description: Ability to submit Supplemental Claims\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-supplemental-claims-openapi.json\n- scope: system/appeals.read\n  description: Appeals info\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-appealable-issues-openapi.json\n  - openapi/va-appeals-status-openapi.json\n  - openapi/va-higher-level-reviews-openapi.json\n  - openapi/va-legacy-appeals-openapi.json\n  - openapi/va-notice-of-disagreements-openapi.json\n\
  \  - openapi/va-supplemental-claims-openapi.json\n- scope: system/appeals.write\n  description: Ability to submit appeals\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/va-higher-level-reviews-openapi.json\n  - openapi/va-notice-of-disagreements-openapi.json\n  - openapi/va-supplemental-claims-openapi.json\n- scope: system/claim.read\n  description: Retrieve claim data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-claims-api-openapi.json\n- scope: system/claim.write\n  description: Submit claim data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-claims-api-openapi.json\n- scope: veteran/AppealableIssues.read\n  description: Appealable issues info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-appealable-issues-openapi.json\n- scope: veteran/AppealsStatus.read\n  description: Status of appeals and decision reviews\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-appeals-status-openapi.json\n- scope: veteran/HigherLevelReviews.read\n\
  \  description: Higher-Level Reviews info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-higher-level-reviews-openapi.json\n- scope: veteran/HigherLevelReviews.write\n  description: Ability to submit Higher-Level Reviews\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-higher-level-reviews-openapi.json\n- scope: veteran/LegacyAppeals.read\n  description: Legacy appeals info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-legacy-appeals-openapi.json\n- scope: veteran/NoticeOfDisagreements.read\n  description: Board Appeals info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-notice-of-disagreements-openapi.json\n- scope: veteran/NoticeOfDisagreements.write\n  description: Ability to submit Board Appeals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-notice-of-disagreements-openapi.json\n- scope: veteran/SupplementalClaims.read\n  description: Supplemental Claims info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-supplemental-claims-openapi.json\n\
  - scope: veteran/SupplementalClaims.write\n  description: Ability to submit Supplemental Claims\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-supplemental-claims-openapi.json\n- scope: veteran/appeals.read\n  description: Appeals info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-appealable-issues-openapi.json\n  - openapi/va-appeals-status-openapi.json\n  - openapi/va-higher-level-reviews-openapi.json\n  - openapi/va-legacy-appeals-openapi.json\n  - openapi/va-notice-of-disagreements-openapi.json\n  - openapi/va-supplemental-claims-openapi.json\n- scope: veteran/appeals.write\n  description: Ability to submit appeals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-higher-level-reviews-openapi.json\n  - openapi/va-notice-of-disagreements-openapi.json\n  - openapi/va-supplemental-claims-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/scopes/va-scopes.yml
summary_line: 35 scopes · authorizationCode/clientCredentials
tags:
- Veterans
- Government
- Health
- Benefits
- FHIR
- Appeals
- Federal
token_urls:
- https://api.va.gov/oauth2/appeals/v1/token
- To get production access, you must either work for VA or have specific VA agreements in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).
- https://sandbox-api.va.gov/oauth2/appeals/v1/token
- https://deptva-eval.okta.com/oauth2/auskff5o6xsoQVngk2p7/v1/token
- https://api.va.gov/oauth2/token
- https://sandbox-api.va.gov/oauth2/token
---
