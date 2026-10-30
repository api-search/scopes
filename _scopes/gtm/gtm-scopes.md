---
api_specs:
- filename: gtm-agent-api-v1-api-openapi.yml
  format: yaml
  label: Agent API
  slug: agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gtm/refs/heads/main/openapi/gtm-agent-api-v1-api-openapi.yml
- filename: gtm-copilot-api-v1-api-openapi.yml
  format: yaml
  label: Copilot API
  slug: copilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gtm/refs/heads/main/openapi/gtm-copilot-api-v1-api-openapi.yml
- filename: gtm-data-api-v1-api-openapi.yml
  format: yaml
  label: Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gtm/refs/heads/main/openapi/gtm-data-api-v1-api-openapi.yml
- filename: gtm-data-quality-api-v1-api-openapi.yml
  format: yaml
  label: Data Quality API
  slug: data-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gtm/refs/heads/main/openapi/gtm-data-quality-api-v1-api-openapi.yml
- filename: gtm-studio-api-v1-api-openapi.yml
  format: yaml
  label: Studio API
  slug: studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gtm/refs/heads/main/openapi/gtm-studio-api-v1-api-openapi.yml
- filename: gtm-marketing-api-v1-api-openapi.yml
  format: yaml
  label: Marketing API
  slug: marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gtm/refs/heads/main/openapi/gtm-marketing-api-v1-api-openapi.yml
- filename: gtm-platform-api-v1-api-openapi.yml
  format: yaml
  label: Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gtm/refs/heads/main/openapi/gtm-platform-api-v1-api-openapi.yml
- filename: gtm-vertical-datasets-api-v1-api-openapi.yml
  format: yaml
  label: Vertical Datasets API
  slug: vertical-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gtm/refs/heads/main/openapi/gtm-vertical-datasets-api-v1-api-openapi.yml
authorization_urls:
- https://login.zoominfo.com
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Gtm Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ZoomInfo publishes 28 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ZoomInfo API on a user''s behalf.


  Tokens are issued from https://okta-login.zoominfo.com/oauth2/default/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ZoomInfo
provider_slug: gtm
schemes:
- flows:
  - authorizationUrl: https://login.zoominfo.com
    flow: authorizationCode
    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token
  name: OAuth2Auth
  source: openapi/gtm-agent-api-v1-api-openapi.yml
- flows:
  - authorizationUrl: https://login.zoominfo.com
    flow: authorizationCode
    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token
  name: OAuth2Auth
  source: openapi/gtm-copilot-api-v1-api-openapi.yml
- flows:
  - authorizationUrl: https://login.zoominfo.com
    flow: authorizationCode
    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token
  name: OAuth2Auth
  source: openapi/gtm-data-api-v1-api-openapi.yml
- flows:
  - authorizationUrl: https://login.zoominfo.com
    flow: authorizationCode
    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token
  name: OAuth2Auth
  source: openapi/gtm-data-quality-api-v1-api-openapi.yml
- flows:
  - authorizationUrl: https://login.zoominfo.com
    flow: authorizationCode
    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token
  name: OAuth2Auth
  source: openapi/gtm-marketing-api-v1-api-openapi.yml
- flows:
  - authorizationUrl: https://login.zoominfo.com
    flow: authorizationCode
    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token
  name: OAuth2Auth
  source: openapi/gtm-platform-api-v1-api-openapi.yml
- flows:
  - authorizationUrl: https://login.zoominfo.com
    flow: authorizationCode
    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token
  name: OAuth2Auth
  source: openapi/gtm-studio-api-v1-api-openapi.yml
- flows:
  - authorizationUrl: https://login.zoominfo.com
    flow: authorizationCode
    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token
  name: OAuth2Auth
  source: openapi/gtm-vertical-datasets-api-v1-api-openapi.yml
scope_count: 28
scope_names:
- api:account-summary:read
- api:agent-pulses:read
- api:agent:execute
- api:agent:read
- api:audience-member:manage
- api:audience:manage
- api:audience:read
- api:central-export-service:execute
- api:central-export-service:read
- api:data-quality:execute
- api:data-quality:manage
- api:data-quality:read
- api:data:company
- api:data:contact
- api:data:intent
- api:data:lookup
- api:data:news
- api:data:scoops
- api:entitlement:read
- api:gtm-config:manage
- api:gtm-config:read
- api:gtm-data-model:manage
- api:gtm-data-model:read
- api:insights:read
- api:recommendations:read
- api:vertical-datasets:read
- api:workflows:execute
- api:workflows:read
scopes:
- description: Read Copilot Account Summary Data
  flows:
  - authorizationCode
  scope: api:account-summary:read
- description: Read the authenticated user's pulses
  flows:
  - authorizationCode
  scope: api:agent-pulses:read
- description: Allows customers to invoke available agents through registered OAuth applications.
  flows:
  - authorizationCode
  scope: api:agent:execute
- description: Allows customers to view available agents, agent details, and agent run results through registered OAuth applications.
  flows:
  - authorizationCode
  scope: api:agent:read
- description: Create and manage audience members
  flows:
  - authorizationCode
  scope: api:audience-member:manage
- description: Create and Manage Audiences
  flows:
  - authorizationCode
  scope: api:audience:manage
- description: Read Audiences
  flows:
  - authorizationCode
  scope: api:audience:read
- description: Execute a destination to activate records into an external system
  flows:
  - authorizationCode
  scope: api:central-export-service:execute
- description: List and inspect available export destinations and their execution history
  flows:
  - authorizationCode
  scope: api:central-export-service:read
- description: Execute Data Quality operations, including the prepare pipeline (parse/validate/normalize plus opt-in enrichments and custom normalization) and synchronous scoring and segmentation
  flows:
  - authorizationCode
  scope: api:data-quality:execute
- description: Create, update, and delete Data Quality configurations, including score and segmentation configs
  flows:
  - authorizationCode
  scope: api:data-quality:manage
- description: Read Data Quality configurations, including score and segmentation configs
  flows:
  - authorizationCode
  scope: api:data-quality:read
- description: Ability to search and enrich ZoomInfo Company data
  flows:
  - authorizationCode
  scope: api:data:company
- description: Ability to search and enrich ZoomInfo Contact data
  flows:
  - authorizationCode
  scope: api:data:contact
- description: Ability to search and enrich ZoomInfo Intent data
  flows:
  - authorizationCode
  scope: api:data:intent
- description: Lookup ZoomInfo Data
  flows:
  - authorizationCode
  scope: api:data:lookup
- description: Ability to search and enrich ZoomInfo News data
  flows:
  - authorizationCode
  scope: api:data:news
- description: Ability to search and enrich ZoomInfo Scoop data
  flows:
  - authorizationCode
  scope: api:data:scoops
- description: Read User entitlements
  flows:
  - authorizationCode
  scope: api:entitlement:read
- description: Manage GTM configuration data (create, update, delete)
  flows:
  - authorizationCode
  scope: api:gtm-config:manage
- description: Read GTM configuration data
  flows:
  - authorizationCode
  scope: api:gtm-config:read
- description: Ability to manage GTM Data Model entities, schemas, and data
  flows:
  - authorizationCode
  scope: api:gtm-data-model:manage
- description: Ability to read GTM Data Model entities, schemas, and data
  flows:
  - authorizationCode
  scope: api:gtm-data-model:read
- description: Read Insights Data
  flows:
  - authorizationCode
  scope: api:insights:read
- description: Read Copilot recommendation data
  flows:
  - authorizationCode
  scope: api:recommendations:read
- description: Ability to read Vertical Datasets API entities and data
  flows:
  - authorizationCode
  scope: api:vertical-datasets:read
- description: Execute Workflows
  flows:
  - authorizationCode
  scope: api:workflows:execute
- description: Read Workflows data
  flows:
  - authorizationCode
  scope: api:workflows:read
slug: gtm-scopes
source_filename: gtm-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/gtm-agent-api-v1-api-openapi.yml, openapi/gtm-copilot-api-v1-api-openapi.yml,\n  openapi/gtm-data-api-v1-api-openapi.yml, openapi/gtm-data-quality-api-v1-api-openapi.yml,\n  openapi/gtm-marketing-api-v1-api-openapi.yml, openapi/gtm-platform-api-v1-api-openapi.yml,\n  openapi/gtm-studio-api-v1-api-openapi.yml, openapi/gtm-vertical-datasets-api-v1-api-openapi.yml\nschemes:\n- name: OAuth2Auth\n  source: openapi/gtm-agent-api-v1-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.zoominfo.com\n    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token\n- name: OAuth2Auth\n  source: openapi/gtm-copilot-api-v1-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.zoominfo.com\n    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token\n- name: OAuth2Auth\n  source: openapi/gtm-data-api-v1-api-openapi.yml\n  flows:\n  - flow:\
  \ authorizationCode\n    authorizationUrl: https://login.zoominfo.com\n    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token\n- name: OAuth2Auth\n  source: openapi/gtm-data-quality-api-v1-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.zoominfo.com\n    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token\n- name: OAuth2Auth\n  source: openapi/gtm-marketing-api-v1-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.zoominfo.com\n    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token\n- name: OAuth2Auth\n  source: openapi/gtm-platform-api-v1-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.zoominfo.com\n    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token\n- name: OAuth2Auth\n  source: openapi/gtm-studio-api-v1-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.zoominfo.com\n\
  \    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token\n- name: OAuth2Auth\n  source: openapi/gtm-vertical-datasets-api-v1-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.zoominfo.com\n    tokenUrl: https://okta-login.zoominfo.com/oauth2/default/v1/token\nscopes:\n- scope: api:account-summary:read\n  description: Read Copilot Account Summary Data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-copilot-api-v1-api-openapi.yml\n- scope: api:agent-pulses:read\n  description: Read the authenticated user's pulses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-agent-api-v1-api-openapi.yml\n- scope: api:agent:execute\n  description: Allows customers to invoke available agents through registered OAuth applications.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-agent-api-v1-api-openapi.yml\n- scope: api:agent:read\n  description: Allows customers to view available agents, agent details, and agent\
  \ run results\n    through registered OAuth applications.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-agent-api-v1-api-openapi.yml\n- scope: api:audience-member:manage\n  description: Create and manage audience members\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-marketing-api-v1-api-openapi.yml\n- scope: api:audience:manage\n  description: Create and Manage Audiences\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-marketing-api-v1-api-openapi.yml\n  - openapi/gtm-studio-api-v1-api-openapi.yml\n- scope: api:audience:read\n  description: Read Audiences\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-marketing-api-v1-api-openapi.yml\n  - openapi/gtm-studio-api-v1-api-openapi.yml\n- scope: api:central-export-service:execute\n  description: Execute a destination to activate records into an external system\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-platform-api-v1-api-openapi.yml\n- scope: api:central-export-service:read\n\
  \  description: List and inspect available export destinations and their execution history\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-platform-api-v1-api-openapi.yml\n- scope: api:data-quality:execute\n  description: Execute Data Quality operations, including the prepare pipeline (parse/validate/normalize\n    plus opt-in enrichments and custom normalization) and synchronous scoring and segmentation\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-data-quality-api-v1-api-openapi.yml\n- scope: api:data-quality:manage\n  description: Create, update, and delete Data Quality configurations, including score and segmentation\n    configs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-data-quality-api-v1-api-openapi.yml\n- scope: api:data-quality:read\n  description: Read Data Quality configurations, including score and segmentation configs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-data-quality-api-v1-api-openapi.yml\n- scope:\
  \ api:data:company\n  description: Ability to search and enrich ZoomInfo Company data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-data-api-v1-api-openapi.yml\n- scope: api:data:contact\n  description: Ability to search and enrich ZoomInfo Contact data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-data-api-v1-api-openapi.yml\n- scope: api:data:intent\n  description: Ability to search and enrich ZoomInfo Intent data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-data-api-v1-api-openapi.yml\n- scope: api:data:lookup\n  description: Lookup ZoomInfo Data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-data-api-v1-api-openapi.yml\n- scope: api:data:news\n  description: Ability to search and enrich ZoomInfo News data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-data-api-v1-api-openapi.yml\n- scope: api:data:scoops\n  description: Ability to search and enrich ZoomInfo Scoop data\n  flows:\n  - authorizationCode\n \
  \ sources:\n  - openapi/gtm-data-api-v1-api-openapi.yml\n- scope: api:entitlement:read\n  description: Read User entitlements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-platform-api-v1-api-openapi.yml\n- scope: api:gtm-config:manage\n  description: Manage GTM configuration data (create, update, delete)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-copilot-api-v1-api-openapi.yml\n- scope: api:gtm-config:read\n  description: Read GTM configuration data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-copilot-api-v1-api-openapi.yml\n- scope: api:gtm-data-model:manage\n  description: Ability to manage GTM Data Model entities, schemas, and data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-platform-api-v1-api-openapi.yml\n- scope: api:gtm-data-model:read\n  description: Ability to read GTM Data Model entities, schemas, and data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-platform-api-v1-api-openapi.yml\n- scope:\
  \ api:insights:read\n  description: Read Insights Data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-copilot-api-v1-api-openapi.yml\n- scope: api:recommendations:read\n  description: Read Copilot recommendation data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-copilot-api-v1-api-openapi.yml\n- scope: api:vertical-datasets:read\n  description: Ability to read Vertical Datasets API entities and data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-vertical-datasets-api-v1-api-openapi.yml\n- scope: api:workflows:execute\n  description: Execute Workflows\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-platform-api-v1-api-openapi.yml\n- scope: api:workflows:read\n  description: Read Workflows data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gtm-platform-api-v1-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gtm/refs/heads/main/scopes/gtm-scopes.yml
summary_line: 28 scopes · authorizationCode
tags:
- Company
- B2B
- Data
- Sales
token_bound: false
token_urls:
- https://okta-login.zoominfo.com/oauth2/default/v1/token
---
