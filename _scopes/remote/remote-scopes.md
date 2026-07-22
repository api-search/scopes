---
api_specs:
- filename: remote-openapi-original.json
  format: json
  label: Remote API
  slug: remote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote/refs/heads/main/openapi/remote-openapi-original.json
authorization_urls:
- /auth/oauth2/authorize
description: ''
docs: https://developer.remote.com/docs/authentication
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Remote Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Remote publishes 86 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Remote API on a user''s behalf.


  Tokens are issued from /auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Remote
provider_slug: remote
schemes:
- description: Authenticate using OAuth 2.0 protocol.
  flows:
  - authorizationUrl: /auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: /auth/oauth2/token
  - flow: clientCredentials
    tokenUrl: /auth/oauth2/token
  name: OAuth2
  source: openapi/remote-openapi-original.json
- description: Authenticate as the employee using the `urn:ietf:params:oauth:grant-type:jwt-bearer` grant in the OAuth2 protocol.
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/oauth2/token
  name: OAuth2Assertion
  source: openapi/remote-openapi-original.json
- description: Authenticate as the token authorizer using `authorization_code` / `refresh_token` grants in the OAuth 2.0 protocol.
  flows:
  - authorizationUrl: /auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: /auth/oauth2/token
  name: OAuth2AuthorizationCode
  source: openapi/remote-openapi-original.json
- description: Authenticate using `client_credentials` grant in the OAuth 2.0 protocol.
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/oauth2/token
  name: OAuth2ClientCredentials
  source: openapi/remote-openapi-original.json
scope_count: 86
scope_names:
- address:read
- address:write
- all:read
- all:write
- background_check:read
- bank_account:read
- bank_account:write
- benefit_offer:read
- benefit_offer:write
- benefit_renewal:read
- benefit_renewal:write
- company:read
- company:write
- company_admin
- company_currencies:read
- company_department:read
- company_department:write
- company_management
- company_manager:read
- company_manager:write
- company_structure:read
- contract:read
- contract_amendment:read
- contract_amendment:write
- contract_eligibility:write
- convert_currency:read
- country:read
- custom_field:read
- custom_field:write
- custom_field_value:read
- custom_field_value:write
- document:read
- document:write
- emergency_contact:read
- emergency_contact:write
- employment:read
- employment:write
- employment_documents
- employment_payments
- employments
- expense:read
- expense:write
- form:read
- help_center_article:read
- https://gateway.remote.com/company.manage
- https://gateway.remote.com/employment.manage
- identity_verification:read
- identity_verification:write
- incentive:read
- incentive:write
- invoices
- invoices:read
- invoices:write
- magic_link:write
- offboarding:read
- offboarding:write
- onboarding:write
- pay_item:read
- pay_item:write
- payroll
- payroll_calendar:read
- payroll_run:read
- payslip:read
- personal_detail:read
- personal_detail:write
- pricing_plan:read
- pricing_plan:write
- probation_document:read
- probation_document:write
- resignation:read
- resignation:write
- resignation_letter:read
- risk_reserve:write
- sso_configuration:read
- sso_configuration:write
- time_and_attendance
- timeoff:read
- timeoff:write
- timesheet:read
- timesheet:write
- travel_letter:read
- travel_letter:write
- webhook:read
- webhook:write
- work_authorization:read
- work_authorization:write
scopes:
- description: address:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: address:read
- description: address:write
  flows:
  - authorizationCode
  - clientCredentials
  scope: address:write
- description: ''
  flows: []
  scope: all:read
- description: ''
  flows: []
  scope: all:write
- description: background_check:read
  flows:
  - authorizationCode
  scope: background_check:read
- description: bank_account:read
  flows:
  - clientCredentials
  scope: bank_account:read
- description: bank_account:write
  flows:
  - clientCredentials
  scope: bank_account:write
- description: benefit_offer:read
  flows:
  - authorizationCode
  scope: benefit_offer:read
- description: benefit_offer:write
  flows:
  - authorizationCode
  scope: benefit_offer:write
- description: benefit_renewal:read
  flows:
  - authorizationCode
  scope: benefit_renewal:read
- description: benefit_renewal:write
  flows:
  - authorizationCode
  scope: benefit_renewal:write
- description: company:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: company:read
- description: company:write
  flows:
  - clientCredentials
  scope: company:write
- description: company_admin
  flows:
  - authorizationCode
  - clientCredentials
  scope: company_admin
- description: company_currencies:read
  flows:
  - authorizationCode
  scope: company_currencies:read
- description: company_department:read
  flows:
  - authorizationCode
  scope: company_department:read
- description: company_department:write
  flows:
  - authorizationCode
  scope: company_department:write
- description: company_management
  flows:
  - clientCredentials
  scope: company_management
- description: company_manager:read
  flows:
  - authorizationCode
  scope: company_manager:read
- description: company_manager:write
  flows:
  - authorizationCode
  scope: company_manager:write
- description: company_structure:read
  flows:
  - authorizationCode
  scope: company_structure:read
- description: contract:read
  flows:
  - authorizationCode
  scope: contract:read
- description: contract_amendment:read
  flows:
  - authorizationCode
  scope: contract_amendment:read
- description: contract_amendment:write
  flows:
  - authorizationCode
  scope: contract_amendment:write
- description: contract_eligibility:write
  flows:
  - authorizationCode
  scope: contract_eligibility:write
- description: convert_currency:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: convert_currency:read
- description: country:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: country:read
- description: custom_field:read
  flows:
  - authorizationCode
  scope: custom_field:read
- description: custom_field:write
  flows:
  - authorizationCode
  scope: custom_field:write
- description: custom_field_value:read
  flows:
  - authorizationCode
  scope: custom_field_value:read
- description: custom_field_value:write
  flows:
  - authorizationCode
  scope: custom_field_value:write
- description: document:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: document:read
- description: document:write
  flows:
  - authorizationCode
  - clientCredentials
  scope: document:write
- description: emergency_contact:read
  flows:
  - clientCredentials
  scope: emergency_contact:read
- description: emergency_contact:write
  flows:
  - clientCredentials
  scope: emergency_contact:write
- description: employment:read
  flows:
  - authorizationCode
  scope: employment:read
- description: employment:write
  flows:
  - authorizationCode
  scope: employment:write
- description: employment_documents
  flows:
  - authorizationCode
  - clientCredentials
  scope: employment_documents
- description: employment_payments
  flows:
  - authorizationCode
  - clientCredentials
  scope: employment_payments
- description: employments
  flows:
  - authorizationCode
  - clientCredentials
  scope: employments
- description: expense:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: expense:read
- description: expense:write
  flows:
  - authorizationCode
  scope: expense:write
- description: form:read
  flows:
  - authorizationCode
  scope: form:read
- description: help_center_article:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: help_center_article:read
- description: ''
  flows: []
  scope: https://gateway.remote.com/company.manage
- description: ''
  flows: []
  scope: https://gateway.remote.com/employment.manage
- description: identity_verification:read
  flows:
  - authorizationCode
  scope: identity_verification:read
- description: identity_verification:write
  flows:
  - authorizationCode
  scope: identity_verification:write
- description: incentive:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: incentive:read
- description: incentive:write
  flows:
  - authorizationCode
  scope: incentive:write
- description: invoices
  flows:
  - authorizationCode
  - clientCredentials
  scope: invoices
- description: invoices:read
  flows:
  - authorizationCode
  scope: invoices:read
- description: invoices:write
  flows:
  - authorizationCode
  scope: invoices:write
- description: magic_link:write
  flows:
  - authorizationCode
  scope: magic_link:write
- description: offboarding:read
  flows:
  - authorizationCode
  scope: offboarding:read
- description: offboarding:write
  flows:
  - authorizationCode
  scope: offboarding:write
- description: onboarding:write
  flows:
  - authorizationCode
  scope: onboarding:write
- description: pay_item:read
  flows:
  - authorizationCode
  scope: pay_item:read
- description: pay_item:write
  flows:
  - authorizationCode
  scope: pay_item:write
- description: payroll
  flows:
  - authorizationCode
  - clientCredentials
  scope: payroll
- description: payroll_calendar:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: payroll_calendar:read
- description: payroll_run:read
  flows:
  - authorizationCode
  scope: payroll_run:read
- description: payslip:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: payslip:read
- description: personal_detail:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: personal_detail:read
- description: personal_detail:write
  flows:
  - clientCredentials
  scope: personal_detail:write
- description: pricing_plan:read
  flows:
  - clientCredentials
  scope: pricing_plan:read
- description: pricing_plan:write
  flows:
  - clientCredentials
  scope: pricing_plan:write
- description: probation_document:read
  flows:
  - authorizationCode
  scope: probation_document:read
- description: probation_document:write
  flows:
  - authorizationCode
  scope: probation_document:write
- description: resignation:read
  flows:
  - authorizationCode
  scope: resignation:read
- description: resignation:write
  flows:
  - authorizationCode
  scope: resignation:write
- description: resignation_letter:read
  flows:
  - authorizationCode
  scope: resignation_letter:read
- description: risk_reserve:write
  flows:
  - authorizationCode
  scope: risk_reserve:write
- description: sso_configuration:read
  flows:
  - authorizationCode
  scope: sso_configuration:read
- description: sso_configuration:write
  flows:
  - authorizationCode
  scope: sso_configuration:write
- description: time_and_attendance
  flows:
  - authorizationCode
  - clientCredentials
  scope: time_and_attendance
- description: timeoff:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: timeoff:read
- description: timeoff:write
  flows:
  - authorizationCode
  - clientCredentials
  scope: timeoff:write
- description: timesheet:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: timesheet:read
- description: timesheet:write
  flows:
  - authorizationCode
  scope: timesheet:write
- description: travel_letter:read
  flows:
  - authorizationCode
  scope: travel_letter:read
- description: travel_letter:write
  flows:
  - authorizationCode
  scope: travel_letter:write
- description: webhook:read
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhook:read
- description: webhook:write
  flows:
  - authorizationCode
  - clientCredentials
  scope: webhook:write
- description: work_authorization:read
  flows:
  - authorizationCode
  scope: work_authorization:read
- description: work_authorization:write
  flows:
  - authorizationCode
  scope: work_authorization:write
slug: remote-scopes
source_filename: remote-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/remote-openapi-original.json\ndocs: https://developer.remote.com/docs/authentication\nnotes: >-\n  86 OAuth 2.0 scopes across authorization_code, client_credentials, and\n  jwt-bearer assertion flows, following a resource:action naming convention\n  (e.g. employment:read, timeoff:write, webhook:write, payroll, invoices).\nschemes:\n- name: OAuth2\n  source: openapi/remote-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /auth/oauth2/authorize\n    tokenUrl: /auth/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: /auth/oauth2/token\n  description: Authenticate using OAuth 2.0 protocol.\n- name: OAuth2Assertion\n  source: openapi/remote-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/oauth2/token\n  description: Authenticate as the employee using the `urn:ietf:params:oauth:grant-type:jwt-bearer`\n    grant in the OAuth2 protocol.\n- name: OAuth2AuthorizationCode\n\
  \  source: openapi/remote-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /auth/oauth2/authorize\n    tokenUrl: /auth/oauth2/token\n  description: Authenticate as the token authorizer using `authorization_code` / `refresh_token`\n    grants in the OAuth 2.0 protocol.\n- name: OAuth2ClientCredentials\n  source: openapi/remote-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/oauth2/token\n  description: Authenticate using `client_credentials` grant in the OAuth 2.0 protocol.\nscopes:\n- scope: address:read\n  description: address:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: address:write\n  description: address:write\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: all:read\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: all:write\n  sources:\n  - openapi/remote-openapi-original.json\n\
  - scope: background_check:read\n  description: background_check:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: bank_account:read\n  description: bank_account:read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: bank_account:write\n  description: bank_account:write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: benefit_offer:read\n  description: benefit_offer:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: benefit_offer:write\n  description: benefit_offer:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: benefit_renewal:read\n  description: benefit_renewal:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: benefit_renewal:write\n  description: benefit_renewal:write\n  flows:\n  -\
  \ authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: company:read\n  description: company:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: company:write\n  description: company:write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: company_admin\n  description: company_admin\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: company_currencies:read\n  description: company_currencies:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: company_department:read\n  description: company_department:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: company_department:write\n  description: company_department:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n\
  - scope: company_management\n  description: company_management\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: company_manager:read\n  description: company_manager:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: company_manager:write\n  description: company_manager:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: company_structure:read\n  description: company_structure:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: contract:read\n  description: contract:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: contract_amendment:read\n  description: contract_amendment:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: contract_amendment:write\n  description: contract_amendment:write\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: contract_eligibility:write\n  description: contract_eligibility:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: convert_currency:read\n  description: convert_currency:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: country:read\n  description: country:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: custom_field:read\n  description: custom_field:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: custom_field:write\n  description: custom_field:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: custom_field_value:read\n  description: custom_field_value:read\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/remote-openapi-original.json\n- scope: custom_field_value:write\n  description: custom_field_value:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: document:read\n  description: document:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: document:write\n  description: document:write\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: emergency_contact:read\n  description: emergency_contact:read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: emergency_contact:write\n  description: emergency_contact:write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: employment:read\n  description: employment:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n\
  - scope: employment:write\n  description: employment:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: employment_documents\n  description: employment_documents\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: employment_payments\n  description: employment_payments\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: employments\n  description: employments\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: expense:read\n  description: expense:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: expense:write\n  description: expense:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: form:read\n  description: form:read\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: help_center_article:read\n  description: help_center_article:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: https://gateway.remote.com/company.manage\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: https://gateway.remote.com/employment.manage\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: identity_verification:read\n  description: identity_verification:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: identity_verification:write\n  description: identity_verification:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: incentive:read\n  description: incentive:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope:\
  \ incentive:write\n  description: incentive:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: invoices\n  description: invoices\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: invoices:read\n  description: invoices:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: invoices:write\n  description: invoices:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: magic_link:write\n  description: magic_link:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: offboarding:read\n  description: offboarding:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: offboarding:write\n  description: offboarding:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n\
  - scope: onboarding:write\n  description: onboarding:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: pay_item:read\n  description: pay_item:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: pay_item:write\n  description: pay_item:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: payroll\n  description: payroll\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: payroll_calendar:read\n  description: payroll_calendar:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: payroll_run:read\n  description: payroll_run:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: payslip:read\n  description: payslip:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/remote-openapi-original.json\n- scope: personal_detail:read\n  description: personal_detail:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: personal_detail:write\n  description: personal_detail:write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: pricing_plan:read\n  description: pricing_plan:read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: pricing_plan:write\n  description: pricing_plan:write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: probation_document:read\n  description: probation_document:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: probation_document:write\n  description: probation_document:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n\
  - scope: resignation:read\n  description: resignation:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: resignation:write\n  description: resignation:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: resignation_letter:read\n  description: resignation_letter:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: risk_reserve:write\n  description: risk_reserve:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: sso_configuration:read\n  description: sso_configuration:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: sso_configuration:write\n  description: sso_configuration:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: time_and_attendance\n  description: time_and_attendance\n  flows:\n\
  \  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: timeoff:read\n  description: timeoff:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: timeoff:write\n  description: timeoff:write\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: timesheet:read\n  description: timesheet:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: timesheet:write\n  description: timesheet:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: travel_letter:read\n  description: travel_letter:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: travel_letter:write\n  description: travel_letter:write\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/remote-openapi-original.json\n- scope: webhook:read\n  description: webhook:read\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: webhook:write\n  description: webhook:write\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: work_authorization:read\n  description: work_authorization:read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n- scope: work_authorization:write\n  description: work_authorization:write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/remote-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remote/refs/heads/main/scopes/remote-scopes.yml
summary_line: 86 scopes · authorizationCode/clientCredentials
tags:
- Company
- HR
- Payroll
- Employer of Record
- Global Employment
- Contractors
- Benefits
- Compliance
- Human Resources
token_urls:
- /auth/oauth2/token
---
