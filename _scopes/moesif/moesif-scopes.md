---
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Moesif Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Moesif publishes 71 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Moesif API on a user''s behalf.


  Tokens are issued from https://api.moesif.com/v1/:orgId/oauth/access_tokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Moesif
provider_slug: moesif
schemes:
- description: "Your Management API token must be added to the request _Authorization_ header using the following format:\n\n `Authorization: Bearer YOUR_MANAGEMENT_API_KEY`"
  flows:
  - flow: password
    tokenUrl: https://api.moesif.com/v1/:orgId/oauth/access_tokens
  name: managementAPIToken
  source: openapi/moesif-openapi.json
- description: "Your Management API token must be added to the request _Authorization_ header using the following format:\n\n `Authorization: Bearer YOUR_MANAGEMENT_API_KEY`"
  flows:
  - flow: password
    tokenUrl: https://api.moesif.com/v1/:orgId/oauth/access_tokens
  name: managementAPIToken
  source: openapi/moesif-openapi.yml
scope_count: 71
scope_names:
- create:access_tokens
- create:apps
- create:billing_meters
- create:billing_reports
- create:cohorts
- create:companies
- create:dashboards
- create:email_templates
- create:encrypted_keys
- create:eth_abi
- create:events
- create:governance_rules
- create:plans
- create:prices
- create:public_workspaces
- create:reports
- create:subscriptions
- create:users
- create:virtual_eventtypes
- create:workspaces
- delete:apps
- delete:billing_meters
- delete:cohorts
- delete:companies
- delete:dashboards
- delete:email_templates
- delete:encrypted_keys
- delete:governance_rules
- delete:plans
- delete:prices
- delete:reports
- delete:users
- delete:virtual_eventtypes
- delete:workspaces
- read:apps
- read:billing_meters
- read:billing_reports
- read:cohorts
- read:companies
- read:company_properties
- read:dashboards
- read:email_templates
- read:encrypted_keys
- read:events
- read:governance_rules
- read:plans
- read:prices
- read:properties
- read:public_workspaces
- read:reports
- read:request_body_properties
- read:response_body_properties
- read:subscriptions
- read:users
- read:virtual_eventtypes
- read:workspaces
- update:apps
- update:cohorts
- update:companies
- update:dashboards
- update:email_templates
- update:encrypted_keys
- update:governance_rules
- update:organizations
- update:plans
- update:prices
- update:public_workspaces
- update:subscriptions
- update:users
- update:virtual_eventtypes
- update:workspaces
scopes:
- description: Create new tokens to access the Management API or Collector API
  flows:
  - password
  scope: create:access_tokens
- description: Create a new application/project under the organization
  flows:
  - password
  scope: create:apps
- description: ''
  flows: []
  scope: create:billing_meters
- description: ''
  flows: []
  scope: create:billing_reports
- description: Save new customer cohorts
  flows:
  - password
  scope: create:cohorts
- description: Create new companies and associated company metadata
  flows:
  - password
  scope: create:companies
- description: Create a new team dashboard that can be shared
  flows:
  - password
  scope: create:dashboards
- description: ''
  flows: []
  scope: create:email_templates
- description: Create encrypted Keys for the Moesif secure proxy
  flows:
  - password
  scope: create:encrypted_keys
- description: Create/upload new Ethereum ABI Entries
  flows:
  - password
  scope: create:eth_abi
- description: Create new events and associated event metadata
  flows:
  - password
  scope: create:events
- description: ''
  flows: []
  scope: create:governance_rules
- description: ''
  flows: []
  scope: create:plans
- description: ''
  flows: []
  scope: create:prices
- description: ''
  flows: []
  scope: create:public_workspaces
- description: Create a new report such as SmartDiff
  flows:
  - password
  scope: create:reports
- description: ''
  flows: []
  scope: create:subscriptions
- description: Create new users and associated user metadata
  flows:
  - password
  scope: create:users
- description: Create virtual events/tags
  flows:
  - password
  scope: create:virtual_eventtypes
- description: Create a new workspace/chart that can be shared
  flows:
  - password
  scope: create:workspaces
- description: Delete an existing application
  flows:
  - password
  scope: delete:apps
- description: ''
  flows: []
  scope: delete:billing_meters
- description: Delete previously saved customer cohorts
  flows:
  - password
  scope: delete:cohorts
- description: Delete existing companies and associated company metadata
  flows:
  - password
  scope: delete:companies
- description: Delete existing dashboards
  flows:
  - password
  scope: delete:dashboards
- description: ''
  flows: []
  scope: delete:email_templates
- description: Delete encrypted Keys for the Moesif secure proxy
  flows:
  - password
  scope: delete:encrypted_keys
- description: ''
  flows: []
  scope: delete:governance_rules
- description: ''
  flows: []
  scope: delete:plans
- description: ''
  flows: []
  scope: delete:prices
- description: Delete existing reports such as SmartDiff
  flows:
  - password
  scope: delete:reports
- description: Delete existing users and associated user metadata
  flows:
  - password
  scope: delete:users
- description: Delete existing virtual events/tags
  flows:
  - password
  scope: delete:virtual_eventtypes
- description: Delete existing workspaces
  flows:
  - password
  scope: delete:workspaces
- description: Read the organization's applications
  flows:
  - password
  scope: read:apps
- description: ''
  flows: []
  scope: read:billing_meters
- description: ''
  flows: []
  scope: read:billing_reports
- description: Read previously saved customer cohorts
  flows:
  - password
  scope: read:cohorts
- description: Read/query companies and associated company metadata
  flows:
  - password
  scope: read:companies
- description: ''
  flows: []
  scope: read:company_properties
- description: Read existing dashboards
  flows:
  - password
  scope: read:dashboards
- description: ''
  flows: []
  scope: read:email_templates
- description: Read encrypted Keys for the Moesif secure proxy
  flows:
  - password
  scope: read:encrypted_keys
- description: Read/query events and associated event metadata
  flows:
  - password
  scope: read:events
- description: ''
  flows: []
  scope: read:governance_rules
- description: ''
  flows: []
  scope: read:plans
- description: ''
  flows: []
  scope: read:prices
- description: ''
  flows: []
  scope: read:properties
- description: Read public workspaces/shared links
  flows:
  - password
  scope: read:public_workspaces
- description: Read reports such as SmartDiff
  flows:
  - password
  scope: read:reports
- description: ''
  flows: []
  scope: read:request_body_properties
- description: ''
  flows: []
  scope: read:response_body_properties
- description: ''
  flows: []
  scope: read:subscriptions
- description: Read/query users and associated user metadata
  flows:
  - password
  scope: read:users
- description: Read existing virtual events/tags
  flows:
  - password
  scope: read:virtual_eventtypes
- description: Read existing workspaces
  flows:
  - password
  scope: read:workspaces
- description: Update an existing application
  flows:
  - password
  scope: update:apps
- description: Update previously saved customer cohorts
  flows:
  - password
  scope: update:cohorts
- description: Update existing companies and associated company metadata
  flows:
  - password
  scope: update:companies
- description: Update existing dashboards
  flows:
  - password
  scope: update:dashboards
- description: ''
  flows: []
  scope: update:email_templates
- description: Update encrypted Keys for the Moesif secure proxy
  flows:
  - password
  scope: update:encrypted_keys
- description: ''
  flows: []
  scope: update:governance_rules
- description: Update an existing application
  flows:
  - password
  scope: update:organizations
- description: ''
  flows: []
  scope: update:plans
- description: ''
  flows: []
  scope: update:prices
- description: ''
  flows: []
  scope: update:public_workspaces
- description: ''
  flows: []
  scope: update:subscriptions
- description: Update existing users and associated user metadata
  flows:
  - password
  scope: update:users
- description: Update existing virtual events/tags
  flows:
  - password
  scope: update:virtual_eventtypes
- description: Update existing workspaces
  flows:
  - password
  scope: update:workspaces
slug: moesif-scopes
source_filename: moesif-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moesif-openapi.json, openapi/moesif-openapi.yml\nschemes:\n- name: managementAPIToken\n  source: openapi/moesif-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: https://api.moesif.com/v1/:orgId/oauth/access_tokens\n  description: |-\n    Your Management API token must be added to the request _Authorization_ header using the following format:\n\n     `Authorization: Bearer YOUR_MANAGEMENT_API_KEY`\n- name: managementAPIToken\n  source: openapi/moesif-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.moesif.com/v1/:orgId/oauth/access_tokens\n  description: |-\n    Your Management API token must be added to the request _Authorization_ header using the following format:\n\n     `Authorization: Bearer YOUR_MANAGEMENT_API_KEY`\nscopes:\n- scope: create:access_tokens\n  description: Create new tokens to access the Management API or Collector API\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n\
  \  - openapi/moesif-openapi.yml\n- scope: create:apps\n  description: Create a new application/project under the organization\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:billing_meters\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:billing_reports\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:cohorts\n  description: Save new customer cohorts\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:companies\n  description: Create new companies and associated company metadata\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:dashboards\n  description: Create a new team dashboard that can be shared\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n\
  - scope: create:email_templates\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:encrypted_keys\n  description: Create encrypted Keys for the Moesif secure proxy\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:eth_abi\n  description: Create/upload new Ethereum ABI Entries\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:events\n  description: Create new events and associated event metadata\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:governance_rules\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:plans\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:prices\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope:\
  \ create:public_workspaces\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:reports\n  description: Create a new report such as SmartDiff\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:subscriptions\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:users\n  description: Create new users and associated user metadata\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:virtual_eventtypes\n  description: Create virtual events/tags\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: create:workspaces\n  description: Create a new workspace/chart that can be shared\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:apps\n  description: Delete an existing\
  \ application\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:billing_meters\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:cohorts\n  description: Delete previously saved customer cohorts\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:companies\n  description: Delete existing companies and associated company metadata\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:dashboards\n  description: Delete existing dashboards\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:email_templates\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:encrypted_keys\n  description: Delete encrypted Keys for the Moesif secure proxy\n  flows:\n\
  \  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:governance_rules\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:plans\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:prices\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:reports\n  description: Delete existing reports such as SmartDiff\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:users\n  description: Delete existing users and associated user metadata\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:virtual_eventtypes\n  description: Delete existing virtual events/tags\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: delete:workspaces\n  description:\
  \ Delete existing workspaces\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:apps\n  description: Read the organization's applications\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:billing_meters\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:billing_reports\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:cohorts\n  description: Read previously saved customer cohorts\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:companies\n  description: Read/query companies and associated company metadata\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:company_properties\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n\
  - scope: read:dashboards\n  description: Read existing dashboards\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:email_templates\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:encrypted_keys\n  description: Read encrypted Keys for the Moesif secure proxy\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:events\n  description: Read/query events and associated event metadata\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:governance_rules\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:plans\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:prices\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:properties\n  sources:\n\
  \  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:public_workspaces\n  description: Read public workspaces/shared links\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:reports\n  description: Read reports such as SmartDiff\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:request_body_properties\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:response_body_properties\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:subscriptions\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:users\n  description: Read/query users and associated user metadata\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:virtual_eventtypes\n  description: Read\
  \ existing virtual events/tags\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: read:workspaces\n  description: Read existing workspaces\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:apps\n  description: Update an existing application\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:cohorts\n  description: Update previously saved customer cohorts\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:companies\n  description: Update existing companies and associated company metadata\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:dashboards\n  description: Update existing dashboards\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  -\
  \ openapi/moesif-openapi.yml\n- scope: update:email_templates\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:encrypted_keys\n  description: Update encrypted Keys for the Moesif secure proxy\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:governance_rules\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:organizations\n  description: Update an existing application\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:plans\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:prices\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:public_workspaces\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:subscriptions\n  sources:\n  - openapi/moesif-openapi.json\n\
  \  - openapi/moesif-openapi.yml\n- scope: update:users\n  description: Update existing users and associated user metadata\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:virtual_eventtypes\n  description: Update existing virtual events/tags\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n- scope: update:workspaces\n  description: Update existing workspaces\n  flows:\n  - password\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/scopes/moesif-scopes.yml
summary_line: 71 scopes · password
tags:
- Analytics
- Monitoring
- Monetization
- Governance
- Observability
- Billing
- AI Agents
- LLM Analytics
- OpenTelemetry
- Developer Portal
- Platform
- Insights
token_urls:
- https://api.moesif.com/v1/:orgId/oauth/access_tokens
---
