---
api_specs:
- filename: remote-companies-api-openapi.yml
  format: yaml
  label: Remote Companies API
  slug: remote-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-companies-api-openapi.yml
- filename: remote-employments-api-openapi.yml
  format: yaml
  label: Remote Employments API
  slug: remote-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-employments-api-openapi.yml
- filename: remote-contractors-api-openapi.yml
  format: yaml
  label: Remote Contractors API
  slug: remote-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-contractors-api-openapi.yml
- filename: remote-payroll-billing-api-openapi.yml
  format: yaml
  label: Remote Payroll and Billing API
  slug: remote-payroll-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-payroll-billing-api-openapi.yml
- filename: remote-time-attendance-api-openapi.yml
  format: yaml
  label: Remote Time and Attendance API
  slug: remote-time-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-time-attendance-api-openapi.yml
- filename: remote-benefits-api-openapi.yml
  format: yaml
  label: Remote Benefits API
  slug: remote-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-benefits-api-openapi.yml
- filename: remote-files-api-openapi.yml
  format: yaml
  label: Remote Files and Custom Fields API
  slug: remote-files-and-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-files-api-openapi.yml
- filename: remote-oauth-api-openapi.yml
  format: yaml
  label: Remote OAuth 2.0 API
  slug: remote-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/openapi/remote-oauth-api-openapi.yml
- filename: remote-webhooks-asyncapi.yml
  format: yaml
  label: Remote Webhooks
  slug: remote-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/asyncapi/remote-webhooks-asyncapi.yml
authorization_urls:
- https://gateway.remote.com/auth/oauth2/authorize
description: ''
docs: https://developer.remote.com/docs/authentication
flows:
- authorizationCode
- clientCredentials
- urn:ietf:params:oauth:grant-type:jwt-bearer
kind: oauth-scopes
layout: scope
method: searched
name: Remote Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Remote publishes 74 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and urn:ietf:params:oauth:grant-type:jwt-bearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Remote API on a user''s behalf.


  Tokens are issued from https://gateway.remote.com/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Remote
provider_slug: remote-com
schemes:
- flows:
  - authorizationUrl: https://gateway.remote.com/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://gateway.remote.com/auth/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://gateway.remote.com/auth/oauth2/token
  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://gateway.remote.com/auth/oauth2/token
  name: OAuth2
  sandbox:
    authorizationUrl: https://gateway.remote-sandbox.com/auth/oauth2/authorize
    tokenUrl: https://gateway.remote-sandbox.com/auth/oauth2/token
  type: oauth2
scope_count: 74
scope_names:
- address:read
- address:write
- background_check:read
- bank_account:read
- bank_account:write
- benefit_offer:read
- benefit_offer:write
- benefit_renewal:read
- benefit_renewal:write
- company:read
- company:write
- company_currencies:read
- company_department:read
- company_department:write
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
- expense:read
- expense:write
- form:read
- help_center_article:read
- identity_verification:read
- identity_verification:write
- incentive:read
- incentive:write
- invoices:read
- invoices:write
- magic_link:write
- offboarding:read
- offboarding:write
- onboarding:write
- pay_item:read
- pay_item:write
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
- description: View addresses
  flows: []
  scope: address:read
- description: Manage addresses
  flows: []
  scope: address:write
- description: View background checks
  flows: []
  scope: background_check:read
- description: View bank accounts
  flows: []
  scope: bank_account:read
- description: Manage bank accounts
  flows: []
  scope: bank_account:write
- description: View benefit offers
  flows: []
  scope: benefit_offer:read
- description: Manage benefit offers
  flows: []
  scope: benefit_offer:write
- description: View benefit renewals
  flows: []
  scope: benefit_renewal:read
- description: Manage benefit renewals
  flows: []
  scope: benefit_renewal:write
- description: View companies
  flows: []
  scope: company:read
- description: Manage companies
  flows: []
  scope: company:write
- description: View company currencies
  flows: []
  scope: company_currencies:read
- description: View departments
  flows: []
  scope: company_department:read
- description: Manage departments
  flows: []
  scope: company_department:write
- description: View managers
  flows: []
  scope: company_manager:read
- description: Manage managers
  flows: []
  scope: company_manager:write
- description: View company structure
  flows: []
  scope: company_structure:read
- description: View contracts
  flows: []
  scope: contract:read
- description: View contract amendments
  flows: []
  scope: contract_amendment:read
- description: Manage contract amendments
  flows: []
  scope: contract_amendment:write
- description: Manage contract eligibility
  flows: []
  scope: contract_eligibility:write
- description: Convert currencies
  flows: []
  scope: convert_currency:read
- description: View countries
  flows: []
  scope: country:read
- description: View custom fields
  flows: []
  scope: custom_field:read
- description: Manage custom fields
  flows: []
  scope: custom_field:write
- description: View custom field values
  flows: []
  scope: custom_field_value:read
- description: Manage custom field values
  flows: []
  scope: custom_field_value:write
- description: View documents
  flows: []
  scope: document:read
- description: Manage documents
  flows: []
  scope: document:write
- description: View emergency contacts
  flows: []
  scope: emergency_contact:read
- description: Manage emergency contacts
  flows: []
  scope: emergency_contact:write
- description: View employments
  flows: []
  scope: employment:read
- description: Manage employments
  flows: []
  scope: employment:write
- description: View expenses
  flows: []
  scope: expense:read
- description: Manage expenses
  flows: []
  scope: expense:write
- description: View forms
  flows: []
  scope: form:read
- description: View help articles
  flows: []
  scope: help_center_article:read
- description: View identity verification
  flows: []
  scope: identity_verification:read
- description: Manage identity verification
  flows: []
  scope: identity_verification:write
- description: View incentives
  flows: []
  scope: incentive:read
- description: Manage incentives
  flows: []
  scope: incentive:write
- description: View invoices
  flows: []
  scope: invoices:read
- description: Manage invoices
  flows: []
  scope: invoices:write
- description: Create magic links
  flows: []
  scope: magic_link:write
- description: View offboarding requests
  flows: []
  scope: offboarding:read
- description: Manage offboarding
  flows: []
  scope: offboarding:write
- description: Manage onboarding
  flows: []
  scope: onboarding:write
- description: View pay items
  flows: []
  scope: pay_item:read
- description: Manage pay items
  flows: []
  scope: pay_item:write
- description: View payroll calendars
  flows: []
  scope: payroll_calendar:read
- description: View payroll runs
  flows: []
  scope: payroll_run:read
- description: View payslips
  flows: []
  scope: payslip:read
- description: View personal details
  flows: []
  scope: personal_detail:read
- description: Manage personal details
  flows: []
  scope: personal_detail:write
- description: View pricing plans
  flows: []
  scope: pricing_plan:read
- description: Manage pricing plans
  flows: []
  scope: pricing_plan:write
- description: View probation documents
  flows: []
  scope: probation_document:read
- description: Manage probation documents
  flows: []
  scope: probation_document:write
- description: View resignations
  flows: []
  scope: resignation:read
- description: Manage resignations
  flows: []
  scope: resignation:write
- description: View resignation letters
  flows: []
  scope: resignation_letter:read
- description: Manage risk reserves
  flows: []
  scope: risk_reserve:write
- description: View SSO configuration
  flows: []
  scope: sso_configuration:read
- description: Manage SSO
  flows: []
  scope: sso_configuration:write
- description: View timeoffs
  flows: []
  scope: timeoff:read
- description: Manage timeoffs
  flows: []
  scope: timeoff:write
- description: View timesheets
  flows: []
  scope: timesheet:read
- description: Manage timesheets
  flows: []
  scope: timesheet:write
- description: View travel letters
  flows: []
  scope: travel_letter:read
- description: Manage travel letters
  flows: []
  scope: travel_letter:write
- description: View webhooks
  flows: []
  scope: webhook:read
- description: Manage webhooks
  flows: []
  scope: webhook:write
- description: View work authorizations
  flows: []
  scope: work_authorization:read
- description: Manage work authorizations
  flows: []
  scope: work_authorization:write
slug: remote-com-scopes
source_filename: remote-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://developer.remote.com/llms.txt (per-endpoint Scopes tables) + https://developer.remote.com/docs/authorization-code-flow\ndocs: https://developer.remote.com/docs/authentication\nnotes: Remote uses OAuth 2.0 (authorization code, client credentials, JWT assertion, refresh). The single\n  authorization-request scope is https://gateway.remote.com/company.manage; the value does not change\n  between production and sandbox. Beyond that grant, Remote enforces a fine-grained permission model of\n  read/write scopes grouped into 8 categories, documented per-endpoint in the API reference. Write scopes\n  imply read access for the same resource. These were harvested from the per-endpoint Scopes tables in\n  the published llms.txt.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://gateway.remote.com/auth/oauth2/authorize\n    tokenUrl: https://gateway.remote.com/auth/oauth2/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://gateway.remote.com/auth/oauth2/token\n  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer\n    tokenUrl: https://gateway.remote.com/auth/oauth2/token\n  sandbox:\n    authorizationUrl: https://gateway.remote-sandbox.com/auth/oauth2/authorize\n    tokenUrl: https://gateway.remote-sandbox.com/auth/oauth2/token\nauthorization_scopes:\n- scope: https://gateway.remote.com/company.manage\n  description: Grants an API partner permission to manage a company and its employments. The single scope\n    requested during the OAuth 2.0 authorization flow; unchanged between production and sandbox.\ncategories:\n- category: company_admin\n  label: Manage company resources\n- category: company_management\n  label: Manage companies\n- category: employment_documents\n  label: Manage employment documents\n- category: employment_payments\n  label: Manage expenses\n- category: employments\n  label: Manage employments\n- category: invoices\n  label: Manage\
  \ invoices\n- category: payroll\n  label: Manage payroll runs\n- category: time_and_attendance\n  label: Manage timeoffs\nscopes:\n- scope: address:read\n  description: View addresses\n  category: employments\n  access: read\n- scope: address:write\n  description: Manage addresses\n  category: employments\n  access: write\n  implies_read: true\n- scope: background_check:read\n  description: View background checks\n  category: employments\n  access: read\n- scope: bank_account:read\n  description: View bank accounts\n  category: employments\n  access: read\n- scope: bank_account:write\n  description: Manage bank accounts\n  category: employments\n  access: write\n  implies_read: true\n- scope: benefit_offer:read\n  description: View benefit offers\n  category: company_admin\n  access: read\n- scope: benefit_offer:write\n  description: Manage benefit offers\n  category: company_admin\n  access: write\n  implies_read: true\n- scope: benefit_renewal:read\n  description: View benefit renewals\n\
  \  category: company_admin\n  access: read\n- scope: benefit_renewal:write\n  description: Manage benefit renewals\n  category: company_admin\n  access: write\n  implies_read: true\n- scope: company:read\n  description: View companies\n  category: company_admin\n  access: read\n- scope: company:write\n  description: Manage companies\n  category: company_admin\n  access: write\n  implies_read: true\n- scope: company_currencies:read\n  description: View company currencies\n  category: company_admin\n  access: read\n- scope: company_department:read\n  description: View departments\n  category: company_admin\n  access: read\n- scope: company_department:write\n  description: Manage departments\n  category: company_admin\n  access: write\n  implies_read: true\n- scope: company_manager:read\n  description: View managers\n  category: company_admin\n  access: read\n- scope: company_manager:write\n  description: Manage managers\n  category: company_admin\n  access: write\n  implies_read: true\n\
  - scope: company_structure:read\n  description: View company structure\n  category: company_admin\n  access: read\n- scope: contract:read\n  description: View contracts\n  category: employments\n  access: read\n- scope: contract_amendment:read\n  description: View contract amendments\n  category: employments\n  access: read\n- scope: contract_amendment:write\n  description: Manage contract amendments\n  category: employments\n  access: write\n  implies_read: true\n- scope: contract_eligibility:write\n  description: Manage contract eligibility\n  category: employment_documents\n  access: write\n  implies_read: true\n- scope: convert_currency:read\n  description: Convert currencies\n  category: company_admin\n  access: read\n- scope: country:read\n  description: View countries\n  category: company_admin\n  access: read\n- scope: custom_field:read\n  description: View custom fields\n  category: employments\n  access: read\n- scope: custom_field:write\n  description: Manage custom fields\n\
  \  category: employments\n  access: write\n  implies_read: true\n- scope: custom_field_value:read\n  description: View custom field values\n  category: employments\n  access: read\n- scope: custom_field_value:write\n  description: Manage custom field values\n  category: employments\n  access: write\n  implies_read: true\n- scope: document:read\n  description: View documents\n  category: employment_documents\n  access: read\n- scope: document:write\n  description: Manage documents\n  category: employment_documents\n  access: write\n  implies_read: true\n- scope: emergency_contact:read\n  description: View emergency contacts\n  category: employments\n  access: read\n- scope: emergency_contact:write\n  description: Manage emergency contacts\n  category: employments\n  access: write\n  implies_read: true\n- scope: employment:read\n  description: View employments\n  category: employments\n  access: read\n- scope: employment:write\n  description: Manage employments\n  category: employments\n\
  \  access: write\n  implies_read: true\n- scope: expense:read\n  description: View expenses\n  category: employment_payments\n  access: read\n- scope: expense:write\n  description: Manage expenses\n  category: employment_payments\n  access: write\n  implies_read: true\n- scope: form:read\n  description: View forms\n  category: company_admin\n  access: read\n- scope: help_center_article:read\n  description: View help articles\n  category: company_admin\n  access: read\n- scope: identity_verification:read\n  description: View identity verification\n  category: employment_documents\n  access: read\n- scope: identity_verification:write\n  description: Manage identity verification\n  category: employment_documents\n  access: write\n  implies_read: true\n- scope: incentive:read\n  description: View incentives\n  category: employment_payments\n  access: read\n- scope: incentive:write\n  description: Manage incentives\n  category: employment_payments\n  access: write\n  implies_read: true\n- scope:\
  \ invoices:read\n  description: View invoices\n  category: invoices\n  access: read\n- scope: invoices:write\n  description: Manage invoices\n  category: invoices\n  access: write\n  implies_read: true\n- scope: magic_link:write\n  description: Create magic links\n  category: company_admin\n  access: write\n  implies_read: true\n- scope: offboarding:read\n  description: View offboarding requests\n  category: employments\n  access: read\n- scope: offboarding:write\n  description: Manage offboarding\n  category: employments\n  access: write\n  implies_read: true\n- scope: onboarding:write\n  description: Manage onboarding\n  category: employments\n  access: write\n  implies_read: true\n- scope: pay_item:read\n  description: View pay items\n  category: payroll\n  access: read\n- scope: pay_item:write\n  description: Manage pay items\n  category: payroll\n  access: write\n  implies_read: true\n- scope: payroll_calendar:read\n  description: View payroll calendars\n  category: payroll\n  access:\
  \ read\n- scope: payroll_run:read\n  description: View payroll runs\n  category: payroll\n  access: read\n- scope: payslip:read\n  description: View payslips\n  category: employment_documents\n  access: read\n- scope: personal_detail:read\n  description: View personal details\n  category: employments\n  access: read\n- scope: personal_detail:write\n  description: Manage personal details\n  category: employments\n  access: write\n  implies_read: true\n- scope: pricing_plan:read\n  description: View pricing plans\n  category: company_management\n  access: read\n- scope: pricing_plan:write\n  description: Manage pricing plans\n  category: company_management\n  access: write\n  implies_read: true\n- scope: probation_document:read\n  description: View probation documents\n  category: employment_documents\n  access: read\n- scope: probation_document:write\n  description: Manage probation documents\n  category: employment_documents\n  access: write\n  implies_read: true\n- scope: resignation:read\n\
  \  description: View resignations\n  category: employments\n  access: read\n- scope: resignation:write\n  description: Manage resignations\n  category: employments\n  access: write\n  implies_read: true\n- scope: resignation_letter:read\n  description: View resignation letters\n  category: employment_documents\n  access: read\n- scope: risk_reserve:write\n  description: Manage risk reserves\n  category: company_admin\n  access: write\n  implies_read: true\n- scope: sso_configuration:read\n  description: View SSO configuration\n  category: company_admin\n  access: read\n- scope: sso_configuration:write\n  description: Manage SSO\n  category: company_admin\n  access: write\n  implies_read: true\n- scope: timeoff:read\n  description: View timeoffs\n  category: time_and_attendance\n  access: read\n- scope: timeoff:write\n  description: Manage timeoffs\n  category: time_and_attendance\n  access: write\n  implies_read: true\n- scope: timesheet:read\n  description: View timesheets\n  category:\
  \ time_and_attendance\n  access: read\n- scope: timesheet:write\n  description: Manage timesheets\n  category: time_and_attendance\n  access: write\n  implies_read: true\n- scope: travel_letter:read\n  description: View travel letters\n  category: employment_documents\n  access: read\n- scope: travel_letter:write\n  description: Manage travel letters\n  category: employment_documents\n  access: write\n  implies_read: true\n- scope: webhook:read\n  description: View webhooks\n  category: company_admin\n  access: read\n- scope: webhook:write\n  description: Manage webhooks\n  category: company_admin\n  access: write\n  implies_read: true\n- scope: work_authorization:read\n  description: View work authorizations\n  category: employments\n  access: read\n- scope: work_authorization:write\n  description: Manage work authorizations\n  category: employments\n  access: write\n  implies_read: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remote-com/refs/heads/main/scopes/remote-com-scopes.yml
summary_line: 74 scopes · authorizationCode/clientCredentials/urn:ietf:params:oauth:grant-type:jwt-bearer
tags:
- Global Payroll
- EOR
- Contractor Management
- Contractor of Record
- PEO
- HRIS
- Recruiting
- Benefits
- Employment
- HR
- Compliance
- Workforce
- MCP
- AI Agents
token_urls:
- https://gateway.remote.com/auth/oauth2/token
---
