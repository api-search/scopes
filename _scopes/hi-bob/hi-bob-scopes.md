---
authorization_urls: []
description: ''
docs: https://apidocs.hibob.com/reference/scopes-mapping-to-endpoints
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Hi Bob Scopes
name_suffix: OAuth Scopes
note: OAuth 2.0 scopes for approved HiBob Marketplace / technology partners. Each scope maps to a specific set of Public API endpoints (endpoint counts noted where the docs state them). Service-user (Basic) integrations do not use scopes — they use category/field permission groups instead.
overview: 'Hi Bob publishes 27 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hi Bob API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hi Bob
provider_slug: hi-bob
schemes: []
scope_count: 27
scope_names:
- employee_data:read
- employee_data:write
- employee_data.history:read
- employee_data.sensitive:read
- employee_data.sensitive:write
- employee_data.sensitive.history:read
- company.metadata:read
- company.metadata:write
- timeoff:read
- timeoff:write
- timeoff.sensitive:read
- attendance:write
- tasks:write
- documents:read
- documents:write
- goals:read
- goals:write
- reports:read
- hiring:write
- job_catalog:read
- learning.integrations:write
- projects:write
- workforce_planning:read
- workforce_planning:write
- payrollhub.employee_sync:write
- payrollhub.payroll:read
- payrollhub.deductions:write
scopes:
- description: View employee profiles and org data.
  flows: []
  scope: employee_data:read
- description: Manage employee profiles and org data.
  flows: []
  scope: employee_data:write
- description: View history of profiles and org chart.
  flows: []
  scope: employee_data.history:read
- description: View sensitive categories (EEO, Financial, Bands, Payroll, UK tax, Equity, Identification, Analytics).
  flows: []
  scope: employee_data.sensitive:read
- description: Manage sensitive data categories (EEO, Financial, Payroll, UK tax, Equity, Identification).
  flows: []
  scope: employee_data.sensitive:write
- description: View history of sensitive categories (payroll history).
  flows: []
  scope: employee_data.sensitive.history:read
- description: View company fields and wizards.
  flows: []
  scope: company.metadata:read
- description: Manage company lists and employee fields.
  flows: []
  scope: company.metadata:write
- description: View employee time off, balances, settings, and company calendar events.
  flows: []
  scope: timeoff:read
- description: Manage employee time off balances and requests; fetch company calendar events.
  flows: []
  scope: timeoff:write
- description: View private time off policy data.
  flows: []
  scope: timeoff.sensitive:read
- description: Manage attendance sheets and balances.
  flows: []
  scope: attendance:write
- description: View and update employee tasks.
  flows: []
  scope: tasks:write
- description: View requests and eSign status reports.
  flows: []
  scope: documents:read
- description: Manage folders, requests, and eSign workflows.
  flows: []
  scope: documents:write
- description: View personal, team, and company goals.
  flows: []
  scope: goals:read
- description: Create, edit, and check in employee, team, and company goals.
  flows: []
  scope: goals:write
- description: Access and download reports.
  flows: []
  scope: reports:read
- description: Search and read hiring data (job ads, openings, candidates, applications, interviews, evaluations, offers).
  flows: []
  scope: hiring:write
- description: View jobs and associated competencies.
  flows: []
  scope: job_catalog:read
- description: Create, update, and delete learning integrations.
  flows: []
  scope: learning.integrations:write
- description: Create and manage projects.
  flows: []
  scope: projects:write
- description: View positions, hierarchy, and budget data.
  flows: []
  scope: workforce_planning:read
- description: Manage positions, budgets, events, and hiring plans.
  flows: []
  scope: workforce_planning:write
- description: Fetch employee data and perform payroll syncs.
  flows: []
  scope: payrollhub.employee_sync:write
- description: Fetch pay cycle metadata, paystub information, and payroll-related data.
  flows: []
  scope: payrollhub.payroll:read
- description: Fetch and update employee-level 401(k) deductions.
  flows: []
  scope: payrollhub.deductions:write
slug: hi-bob-scopes
source_filename: hi-bob-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apidocs.hibob.com/reference/scopes-mapping-to-endpoints\ndocs: https://apidocs.hibob.com/reference/scopes-mapping-to-endpoints\nscheme: OAuth2\nauthorizationUrl: https://auth.app.hibob.com/\ntokenUrl: https://auth.app.hibob.com/oauth2/v1/apps/token\nnote: >-\n  OAuth 2.0 scopes for approved HiBob Marketplace / technology partners. Each scope\n  maps to a specific set of Public API endpoints (endpoint counts noted where the docs\n  state them). Service-user (Basic) integrations do not use scopes — they use\n  category/field permission groups instead.\nscopes:\n- scope: employee_data:read\n  description: View employee profiles and org data.\n- scope: employee_data:write\n  description: Manage employee profiles and org data.\n- scope: employee_data.history:read\n  description: View history of profiles and org chart.\n- scope: employee_data.sensitive:read\n  description: >-\n    View sensitive categories (EEO, Financial,\
  \ Bands, Payroll, UK tax, Equity,\n    Identification, Analytics).\n- scope: employee_data.sensitive:write\n  description: >-\n    Manage sensitive data categories (EEO, Financial, Payroll, UK tax, Equity,\n    Identification).\n- scope: employee_data.sensitive.history:read\n  description: View history of sensitive categories (payroll history).\n- scope: company.metadata:read\n  description: View company fields and wizards.\n- scope: company.metadata:write\n  description: Manage company lists and employee fields.\n- scope: timeoff:read\n  description: View employee time off, balances, settings, and company calendar events.\n- scope: timeoff:write\n  description: Manage employee time off balances and requests; fetch company calendar events.\n- scope: timeoff.sensitive:read\n  description: View private time off policy data.\n- scope: attendance:write\n  description: Manage attendance sheets and balances.\n- scope: tasks:write\n  description: View and update employee tasks.\n- scope: documents:read\n\
  \  description: View requests and eSign status reports.\n- scope: documents:write\n  description: Manage folders, requests, and eSign workflows.\n- scope: goals:read\n  description: View personal, team, and company goals.\n- scope: goals:write\n  description: Create, edit, and check in employee, team, and company goals.\n- scope: reports:read\n  description: Access and download reports.\n- scope: hiring:write\n  description: >-\n    Search and read hiring data (job ads, openings, candidates, applications,\n    interviews, evaluations, offers).\n- scope: job_catalog:read\n  description: View jobs and associated competencies.\n- scope: learning.integrations:write\n  description: Create, update, and delete learning integrations.\n- scope: projects:write\n  description: Create and manage projects.\n- scope: workforce_planning:read\n  description: View positions, hierarchy, and budget data.\n- scope: workforce_planning:write\n  description: Manage positions, budgets, events, and hiring plans.\n\
  - scope: payrollhub.employee_sync:write\n  description: Fetch employee data and perform payroll syncs.\n- scope: payrollhub.payroll:read\n  description: Fetch pay cycle metadata, paystub information, and payroll-related data.\n- scope: payrollhub.deductions:write\n  description: Fetch and update employee-level 401(k) deductions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hi-bob/refs/heads/main/scopes/hi-bob-scopes.yml
summary_line: 27 scopes
tags:
- Company
- HR
- HRIS
- Human Resources
- Payroll
- People Analytics
- Time Off
- Workforce Planning
- Employees
- HR Tech
token_urls: []
---
