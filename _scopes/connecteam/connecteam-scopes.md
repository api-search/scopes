---
api_specs:
- filename: connecteam-openapi-original.json
  format: json
  label: Connecteam API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connecteam/refs/heads/main/openapi/connecteam-openapi-original.json
authorization_urls: []
description: ''
docs: https://developer.connecteam.com/docs/oauth-20
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Connecteam Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Connecteam publishes 62 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Connecteam API on a user''s behalf.


  Tokens are issued from /oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Connecteam
provider_slug: connecteam
schemes:
- description: OAuth2 Bearer token
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/v1/token
  name: OAuth2
  source: openapi/connecteam-openapi-original.json
scope_count: 62
scope_names:
- account_information.delete
- account_information.read
- account_information.write
- assets.delete
- assets.read
- assets.write
- attachments.delete
- attachments.read
- attachments.write
- celebrations.read
- chat.delete
- chat.read
- chat.write
- company_checklist.read
- company_checklist.write
- company_insights.read
- company_policies.delete
- company_policies.read
- company_policies.write
- daily_note.delete
- daily_note.read
- daily_note.write
- forms.delete
- forms.read
- forms.write
- jobs.delete
- jobs.read
- jobs.write
- nfc.delete
- nfc.read
- nfc.write
- onboarding.delete
- onboarding.read
- onboarding.write
- pay_rates.delete
- pay_rates.read
- pay_rates.write
- publishers.delete
- publishers.read
- publishers.write
- quick_tasks.delete
- quick_tasks.read
- quick_tasks.write
- recognitions.read
- sales_data.delete
- sales_data.read
- sales_data.write
- schedule.delete
- schedule.read
- schedule.write
- settings.delete
- settings.read
- settings.write
- time_clock.delete
- time_clock.read
- time_clock.write
- time_off.delete
- time_off.read
- time_off.write
- users.delete
- users.read
- users.write
scopes:
- description: account information - delete
  flows:
  - clientCredentials
  scope: account_information.delete
- description: account information - read
  flows:
  - clientCredentials
  scope: account_information.read
- description: account information - write
  flows:
  - clientCredentials
  scope: account_information.write
- description: assets - delete
  flows:
  - clientCredentials
  scope: assets.delete
- description: assets - read
  flows:
  - clientCredentials
  scope: assets.read
- description: assets - write
  flows:
  - clientCredentials
  scope: assets.write
- description: attachments - delete
  flows:
  - clientCredentials
  scope: attachments.delete
- description: attachments - read
  flows:
  - clientCredentials
  scope: attachments.read
- description: attachments - write
  flows:
  - clientCredentials
  scope: attachments.write
- description: celebrations - read
  flows:
  - clientCredentials
  scope: celebrations.read
- description: chat - delete
  flows:
  - clientCredentials
  scope: chat.delete
- description: chat - read
  flows:
  - clientCredentials
  scope: chat.read
- description: chat - write
  flows:
  - clientCredentials
  scope: chat.write
- description: company checklist - read
  flows:
  - clientCredentials
  scope: company_checklist.read
- description: company checklist - write
  flows:
  - clientCredentials
  scope: company_checklist.write
- description: company insights - read
  flows:
  - clientCredentials
  scope: company_insights.read
- description: company policies - delete
  flows:
  - clientCredentials
  scope: company_policies.delete
- description: company policies - read
  flows:
  - clientCredentials
  scope: company_policies.read
- description: company policies - write
  flows:
  - clientCredentials
  scope: company_policies.write
- description: daily note - delete
  flows:
  - clientCredentials
  scope: daily_note.delete
- description: daily note - read
  flows:
  - clientCredentials
  scope: daily_note.read
- description: daily note - write
  flows:
  - clientCredentials
  scope: daily_note.write
- description: forms - delete
  flows:
  - clientCredentials
  scope: forms.delete
- description: forms - read
  flows:
  - clientCredentials
  scope: forms.read
- description: forms - write
  flows:
  - clientCredentials
  scope: forms.write
- description: jobs - delete
  flows:
  - clientCredentials
  scope: jobs.delete
- description: jobs - read
  flows:
  - clientCredentials
  scope: jobs.read
- description: jobs - write
  flows:
  - clientCredentials
  scope: jobs.write
- description: nfc - delete
  flows:
  - clientCredentials
  scope: nfc.delete
- description: nfc - read
  flows:
  - clientCredentials
  scope: nfc.read
- description: nfc - write
  flows:
  - clientCredentials
  scope: nfc.write
- description: onboarding - delete
  flows:
  - clientCredentials
  scope: onboarding.delete
- description: onboarding - read
  flows:
  - clientCredentials
  scope: onboarding.read
- description: onboarding - write
  flows:
  - clientCredentials
  scope: onboarding.write
- description: pay rates - delete
  flows:
  - clientCredentials
  scope: pay_rates.delete
- description: pay rates - read
  flows:
  - clientCredentials
  scope: pay_rates.read
- description: pay rates - write
  flows:
  - clientCredentials
  scope: pay_rates.write
- description: publishers - delete
  flows:
  - clientCredentials
  scope: publishers.delete
- description: publishers - read
  flows:
  - clientCredentials
  scope: publishers.read
- description: publishers - write
  flows:
  - clientCredentials
  scope: publishers.write
- description: quick tasks - delete
  flows:
  - clientCredentials
  scope: quick_tasks.delete
- description: quick tasks - read
  flows:
  - clientCredentials
  scope: quick_tasks.read
- description: quick tasks - write
  flows:
  - clientCredentials
  scope: quick_tasks.write
- description: recognitions - read
  flows:
  - clientCredentials
  scope: recognitions.read
- description: sales data - delete
  flows:
  - clientCredentials
  scope: sales_data.delete
- description: sales data - read
  flows:
  - clientCredentials
  scope: sales_data.read
- description: sales data - write
  flows:
  - clientCredentials
  scope: sales_data.write
- description: schedule - delete
  flows:
  - clientCredentials
  scope: schedule.delete
- description: schedule - read
  flows:
  - clientCredentials
  scope: schedule.read
- description: schedule - write
  flows:
  - clientCredentials
  scope: schedule.write
- description: settings - delete
  flows:
  - clientCredentials
  scope: settings.delete
- description: settings - read
  flows:
  - clientCredentials
  scope: settings.read
- description: settings - write
  flows:
  - clientCredentials
  scope: settings.write
- description: time clock - delete
  flows:
  - clientCredentials
  scope: time_clock.delete
- description: time clock - read
  flows:
  - clientCredentials
  scope: time_clock.read
- description: time clock - write
  flows:
  - clientCredentials
  scope: time_clock.write
- description: time off - delete
  flows:
  - clientCredentials
  scope: time_off.delete
- description: time off - read
  flows:
  - clientCredentials
  scope: time_off.read
- description: time off - write
  flows:
  - clientCredentials
  scope: time_off.write
- description: users - delete
  flows:
  - clientCredentials
  scope: users.delete
- description: users - read
  flows:
  - clientCredentials
  scope: users.read
- description: users - write
  flows:
  - clientCredentials
  scope: users.write
slug: connecteam-scopes
source_filename: connecteam-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://developer.connecteam.com/docs/oauth-20 + openapi/connecteam-openapi-original.json\ndocs: https://developer.connecteam.com/docs/oauth-20\nflow: client_credentials\ntoken_endpoint: https://api.connecteam.com/oauth/v1/token\ntoken_lifetime_seconds: 86400\nnaming_convention: feature.permission (e.g. users.read, schedule.write)\ngrant_note: Scopes are selected when the OAuth app is created in Your Name -> Integration Center -> OAuth\n  2.0 and CANNOT be edited afterwards. Request the minimum set. The client secret is displayed once.\npermission_matrix:\n- feature: Account Information\n  prefix: account_information\n  read: true\n  write: true\n  delete: true\n- feature: Company Policies\n  prefix: company_policies\n  read: true\n  write: true\n  delete: true\n- feature: Users\n  prefix: users\n  read: true\n  write: true\n  delete: true\n- feature: Assets\n  prefix: assets\n  read: true\n  write: true\n  delete: true\n-\
  \ feature: Sales Data\n  prefix: sales_data\n  read: true\n  write: true\n  delete: true\n- feature: Attachments\n  prefix: attachments\n  read: true\n  write: true\n  delete: true\n- feature: Quick Tasks\n  prefix: quick_tasks\n  read: true\n  write: true\n  delete: true\n- feature: Publishers\n  prefix: publishers\n  read: true\n  write: true\n  delete: true\n- feature: Chat\n  prefix: chat\n  read: true\n  write: true\n  delete: true\n- feature: Jobs (Resources)\n  prefix: jobs\n  read: true\n  write: true\n  delete: true\n- feature: Schedule\n  prefix: schedule\n  read: true\n  write: true\n  delete: true\n- feature: Daily Note\n  prefix: daily_note\n  read: true\n  write: true\n  delete: true\n- feature: Time Clock\n  prefix: time_clock\n  read: true\n  write: true\n  delete: true\n- feature: Time Off\n  prefix: time_off\n  read: true\n  write: true\n  delete: true\n- feature: Forms\n  prefix: forms\n  read: true\n  write: true\n  delete: true\n- feature: Settings\n  prefix: settings\n\
  \  read: true\n  write: true\n  delete: true\nspec_only_scopes_note: 'The OpenAPI declares scopes the docs matrix omits: company_insights.read, nfc.{read,write,delete},\n  pay_rates.{read,write,delete}, onboarding.{read,write,delete}, company_checklist.{read,write}, recognitions.read\n  and celebrations.read. Some are read-only (company_insights, recognitions, celebrations) or write-only\n  pairs (company_checklist), which breaks the uniform read/write/delete triple the docs page implies.'\nschemes:\n- name: OAuth2\n  source: openapi/connecteam-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/v1/token\n  description: OAuth2 Bearer token\nscopes:\n- scope: account_information.delete\n  description: account information - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: account_information.read\n  description: account information - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n\
  - scope: account_information.write\n  description: account information - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: assets.delete\n  description: assets - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: assets.read\n  description: assets - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: assets.write\n  description: assets - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: attachments.delete\n  description: attachments - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: attachments.read\n  description: attachments - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: attachments.write\n  description: attachments - write\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: celebrations.read\n  description: celebrations - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: chat.delete\n  description: chat - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: chat.read\n  description: chat - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: chat.write\n  description: chat - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: company_checklist.read\n  description: company checklist - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: company_checklist.write\n  description: company checklist - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: company_insights.read\n\
  \  description: company insights - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: company_policies.delete\n  description: company policies - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: company_policies.read\n  description: company policies - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: company_policies.write\n  description: company policies - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: daily_note.delete\n  description: daily note - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: daily_note.read\n  description: daily note - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: daily_note.write\n  description: daily note - write\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: forms.delete\n  description: forms - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: forms.read\n  description: forms - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: forms.write\n  description: forms - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: jobs.delete\n  description: jobs - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: jobs.read\n  description: jobs - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: jobs.write\n  description: jobs - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: nfc.delete\n  description: nfc - delete\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: nfc.read\n  description: nfc - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: nfc.write\n  description: nfc - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: onboarding.delete\n  description: onboarding - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: onboarding.read\n  description: onboarding - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: onboarding.write\n  description: onboarding - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: pay_rates.delete\n  description: pay rates - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: pay_rates.read\n  description: pay rates - read\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: pay_rates.write\n  description: pay rates - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: publishers.delete\n  description: publishers - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: publishers.read\n  description: publishers - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: publishers.write\n  description: publishers - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: quick_tasks.delete\n  description: quick tasks - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: quick_tasks.read\n  description: quick tasks - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n\
  - scope: quick_tasks.write\n  description: quick tasks - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: recognitions.read\n  description: recognitions - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: sales_data.delete\n  description: sales data - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: sales_data.read\n  description: sales data - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: sales_data.write\n  description: sales data - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: schedule.delete\n  description: schedule - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: schedule.read\n  description: schedule - read\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: schedule.write\n  description: schedule - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: settings.delete\n  description: settings - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: settings.read\n  description: settings - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: settings.write\n  description: settings - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: time_clock.delete\n  description: time clock - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: time_clock.read\n  description: time clock - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: time_clock.write\n  description:\
  \ time clock - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: time_off.delete\n  description: time off - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: time_off.read\n  description: time off - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: time_off.write\n  description: time off - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: users.delete\n  description: users - delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: users.read\n  description: users - read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\n- scope: users.write\n  description: users - write\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/connecteam-openapi-original.json\nsummary:\n\
  \  scopes_total: 62\n  features_in_docs_matrix: 16\n  source_of_truth: the OpenAPI securitySchemes.OAuth2.flows.clientCredentials.scopes map\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connecteam/refs/heads/main/scopes/connecteam-scopes.yml
summary_line: 62 scopes · clientCredentials
tags:
- Company
- Workforce Management
- Human Resources
- Time Tracking
- Scheduling
- Employee Communication
- Task Management
- Forms
- Deskless
- SaaS
token_urls:
- /oauth/v1/token
---
