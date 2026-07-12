---
authorization_urls:
- https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Workday Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workday publishes 29 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday API on a user''s behalf.


  Tokens are issued from https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday
provider_slug: workday
schemes:
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/absenceManagement.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/benefits.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/common.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/compensation.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/financialManagement.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/hcm.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/payroll.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/performanceManagement.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/person.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/prismAnalytics.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/raas.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/recruiting.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/staffing.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/talent.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/timeTracking.yml
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/wql.yml
scope_count: 29
scope_names:
- r_absence
- r_benefits
- r_common
- r_compensation
- r_financials
- r_payroll
- r_performance
- r_person
- r_prism
- r_recruiting
- r_reports
- r_staffing
- r_talent
- r_timeTracking
- r_worker
- r_wql
- w_absence
- w_benefits
- w_compensation
- w_financials
- w_payroll
- w_performance
- w_person
- w_prism
- w_recruiting
- w_staffing
- w_talent
- w_timeTracking
- w_worker
scopes:
- description: Read absence data
  flows:
  - authorizationCode
  scope: r_absence
- description: Read benefits data
  flows:
  - authorizationCode
  scope: r_benefits
- description: Read common reference data
  flows:
  - authorizationCode
  scope: r_common
- description: Read compensation data
  flows:
  - authorizationCode
  scope: r_compensation
- description: Read financial data
  flows:
  - authorizationCode
  scope: r_financials
- description: Read payroll data
  flows:
  - authorizationCode
  scope: r_payroll
- description: Read performance data
  flows:
  - authorizationCode
  scope: r_performance
- description: Read person data
  flows:
  - authorizationCode
  scope: r_person
- description: Read Prism Analytics data
  flows:
  - authorizationCode
  scope: r_prism
- description: Read recruiting data
  flows:
  - authorizationCode
  scope: r_recruiting
- description: Read report data
  flows:
  - authorizationCode
  scope: r_reports
- description: Read staffing data
  flows:
  - authorizationCode
  scope: r_staffing
- description: Read talent data
  flows:
  - authorizationCode
  scope: r_talent
- description: Read time tracking data
  flows:
  - authorizationCode
  scope: r_timeTracking
- description: Read worker data
  flows:
  - authorizationCode
  scope: r_worker
- description: Execute WQL queries
  flows:
  - authorizationCode
  scope: r_wql
- description: Write absence data
  flows:
  - authorizationCode
  scope: w_absence
- description: Write benefits data
  flows:
  - authorizationCode
  scope: w_benefits
- description: Write compensation data
  flows:
  - authorizationCode
  scope: w_compensation
- description: Write financial data
  flows:
  - authorizationCode
  scope: w_financials
- description: Write payroll data
  flows:
  - authorizationCode
  scope: w_payroll
- description: Write performance data
  flows:
  - authorizationCode
  scope: w_performance
- description: Write person data
  flows:
  - authorizationCode
  scope: w_person
- description: Write Prism Analytics data
  flows:
  - authorizationCode
  scope: w_prism
- description: Write recruiting data
  flows:
  - authorizationCode
  scope: w_recruiting
- description: Write staffing data
  flows:
  - authorizationCode
  scope: w_staffing
- description: Write talent data
  flows:
  - authorizationCode
  scope: w_talent
- description: Write time tracking data
  flows:
  - authorizationCode
  scope: w_timeTracking
- description: Write worker data
  flows:
  - authorizationCode
  scope: w_worker
slug: workday-scopes
source_filename: workday-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/absenceManagement.yml, openapi/benefits.yml, openapi/common.yml, openapi/compensation.yml,\n  openapi/financialManagement.yml, openapi/hcm.yml, openapi/payroll.yml, openapi/performanceManagement.yml,\n  openapi/person.yml, openapi/prismAnalytics.yml, openapi/raas.yml, openapi/recruiting.yml,\n  openapi/staffing.yml, openapi/talent.yml, openapi/timeTracking.yml, openapi/wql.yml\nschemes:\n- name: OAuth2\n  source: openapi/absenceManagement.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/benefits.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n\
  \  source: openapi/common.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/compensation.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/financialManagement.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/hcm.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n\
  - name: OAuth2\n  source: openapi/payroll.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/performanceManagement.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/person.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/prismAnalytics.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n\
  - name: OAuth2\n  source: openapi/raas.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/recruiting.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/staffing.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/talent.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n\
  - name: OAuth2\n  source: openapi/timeTracking.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/wql.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\nscopes:\n- scope: r_absence\n  description: Read absence data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/absenceManagement.yml\n- scope: r_benefits\n  description: Read benefits data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/benefits.yml\n- scope: r_common\n  description: Read common reference data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/common.yml\n- scope: r_compensation\n  description: Read compensation data\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/compensation.yml\n- scope: r_financials\n  description: Read financial data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/financialManagement.yml\n- scope: r_payroll\n  description: Read payroll data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/payroll.yml\n- scope: r_performance\n  description: Read performance data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/performanceManagement.yml\n- scope: r_person\n  description: Read person data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/person.yml\n- scope: r_prism\n  description: Read Prism Analytics data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/prismAnalytics.yml\n- scope: r_recruiting\n  description: Read recruiting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recruiting.yml\n- scope: r_reports\n  description: Read report data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/raas.yml\n- scope: r_staffing\n  description:\
  \ Read staffing data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/staffing.yml\n- scope: r_talent\n  description: Read talent data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/talent.yml\n- scope: r_timeTracking\n  description: Read time tracking data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/timeTracking.yml\n- scope: r_worker\n  description: Read worker data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hcm.yml\n- scope: r_wql\n  description: Execute WQL queries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wql.yml\n- scope: w_absence\n  description: Write absence data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/absenceManagement.yml\n- scope: w_benefits\n  description: Write benefits data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/benefits.yml\n- scope: w_compensation\n  description: Write compensation data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/compensation.yml\n- scope:\
  \ w_financials\n  description: Write financial data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/financialManagement.yml\n- scope: w_payroll\n  description: Write payroll data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/payroll.yml\n- scope: w_performance\n  description: Write performance data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/performanceManagement.yml\n- scope: w_person\n  description: Write person data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/person.yml\n- scope: w_prism\n  description: Write Prism Analytics data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/prismAnalytics.yml\n- scope: w_recruiting\n  description: Write recruiting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/recruiting.yml\n- scope: w_staffing\n  description: Write staffing data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/staffing.yml\n- scope: w_talent\n  description: Write talent data\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/talent.yml\n- scope: w_timeTracking\n  description: Write time tracking data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/timeTracking.yml\n- scope: w_worker\n  description: Write worker data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hcm.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/scopes/workday-scopes.yml
summary_line: 29 scopes · authorizationCode
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
token_urls:
- https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
---
