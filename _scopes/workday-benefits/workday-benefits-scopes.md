---
api_specs:
- filename: workday-benefits-benefit-enrollments-api-openapi.yml
  format: yaml
  label: Workday Benefits Benefit Enrollments API
  slug: workday-benefits-benefit-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-enrollments-api-openapi.yml
- filename: workday-benefits-benefit-events-api-openapi.yml
  format: yaml
  label: Workday Benefits Benefit Events API
  slug: workday-benefits-benefit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-events-api-openapi.yml
- filename: workday-benefits-benefit-plans-api-openapi.yml
  format: yaml
  label: Workday Benefits Benefit Plans API
  slug: workday-benefits-benefit-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-plans-api-openapi.yml
- filename: workday-benefits-dependents-api-openapi.yml
  format: yaml
  label: Workday Benefits Dependents API
  slug: workday-benefits-dependents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-dependents-api-openapi.yml
- filename: workday-benefits-employee-benefits-api-openapi.yml
  format: yaml
  label: Workday Benefits Employee Benefits API
  slug: workday-benefits-employee-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-employee-benefits-api-openapi.yml
- filename: workday-benefits-time-off-plans-api-openapi.yml
  format: yaml
  label: Workday Benefits Time Off Plans API
  slug: workday-benefits-time-off-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-time-off-plans-api-openapi.yml
- filename: workday-benefits-benefit-enrollment-event-offerings-openapi.json
  format: json
  label: Workday Benefit Enrollment Event Offerings API
  slug: workday-benefits-benefit-enrollment-event-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-enrollment-event-offerings-openapi.json
- filename: workday-benefits-benefit-partner-openapi.json
  format: json
  label: Workday Benefit Partner API
  slug: workday-benefits-benefit-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-partner-openapi.json
authorization_urls:
- https://<tenantAuthorizationHostname>
description: ''
docs: https://developer.workday.com/doc/GUID-6c598444-ce67-40d5-bd95-267ecfe439b8-enHYPHENus.md
flows:
- implicit
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Workday Benefits Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workday Benefits publishes 1 OAuth 2.0 scope via the implicit and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday Benefits API on a user''s behalf.


  Tokens are issued from https://{tenant}.workday.com/ccx/oauth2/{tenant}/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday Benefits
provider_slug: workday-benefits
schemes:
- flows:
  - authorizationUrl: https://<tenantAuthorizationHostname>
    flow: implicit
  name: OAuth2
  source: openapi/workday-benefits-benefit-enrollment-event-offerings-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  source: openapi/workday-benefits-benefit-enrollments-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  source: openapi/workday-benefits-benefit-events-api-openapi.yml
- flows:
  - authorizationUrl: https://<tenantAuthorizationHostname>
    flow: implicit
  name: OAuth2
  source: openapi/workday-benefits-benefit-partner-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  source: openapi/workday-benefits-benefit-plans-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  source: openapi/workday-benefits-dependents-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  source: openapi/workday-benefits-employee-benefits-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  source: openapi/workday-benefits-time-off-plans-api-openapi.yml
scope_count: 1
scope_names:
- benefits
scopes:
- description: Access to Workday Benefits API
  flows:
  - clientCredentials
  scope: benefits
slug: workday-benefits-scopes
source_filename: workday-benefits-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/workday-benefits-benefit-enrollment-event-offerings-openapi.json, openapi/workday-benefits-benefit-enrollments-api-openapi.yml,\n  openapi/workday-benefits-benefit-events-api-openapi.yml, openapi/workday-benefits-benefit-partner-openapi.json,\n  openapi/workday-benefits-benefit-plans-api-openapi.yml, openapi/workday-benefits-dependents-api-openapi.yml, openapi/workday-benefits-employee-benefits-api-openapi.yml,\n  openapi/workday-benefits-time-off-plans-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/workday-benefits-benefit-enrollment-event-offerings-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://<tenantAuthorizationHostname>\n- name: oauth2\n  source: openapi/workday-benefits-benefit-enrollments-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n- name: oauth2\n  source: openapi/workday-benefits-benefit-events-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/workday-benefits-benefit-partner-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://<tenantAuthorizationHostname>\n- name: oauth2\n  source: openapi/workday-benefits-benefit-plans-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n- name: oauth2\n  source: openapi/workday-benefits-dependents-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n- name: oauth2\n  source: openapi/workday-benefits-employee-benefits-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n- name: oauth2\n  source: openapi/workday-benefits-time-off-plans-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n\
  scopes:\n- scope: benefits\n  description: Access to Workday Benefits API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/workday-benefits-benefit-enrollments-api-openapi.yml\n  - openapi/workday-benefits-benefit-events-api-openapi.yml\n  - openapi/workday-benefits-benefit-plans-api-openapi.yml\n  - openapi/workday-benefits-dependents-api-openapi.yml\n  - openapi/workday-benefits-employee-benefits-api-openapi.yml\n  - openapi/workday-benefits-time-off-plans-api-openapi.yml\ndocs: https://developer.workday.com/doc/GUID-6c598444-ce67-40d5-bd95-267ecfe439b8-enHYPHENus.md\nscope_model:\n  style: functional-area scopes granted at API client registration\n  detail: Workday scopes are Functional Area scopes selected when the API client is registered in the tenant, not\n    string scopes enumerated in the contract. Both production Benefits contracts declare an OAuth2 scheme whose\n    scopes object is EMPTY, so no scope string can be read from the machine-readable contract - the scope\
  \ that matters\n    for this surface is the Benefits functional area plus the security domains it carries.\n  contract_declared_scopes: 0\n  note: 'The single scope \"benefits\" listed below is derived from the API Evangelist-authored scaffold specs in\n    openapi/ (x-generated-from: documentation), NOT from a Workday-published scope reference. It is retained for\n    continuity and is flagged here so it is not mistaken for a provider-published scope string.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/scopes/workday-benefits-scopes.yml
summary_line: 1 scope · implicit/clientCredentials
tags:
- Benefits
- Human Resources
- HCM
- Enterprise
- Payroll
- Employee Benefits
- SOAP
- OpenAPI
token_urls:
- https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
---
