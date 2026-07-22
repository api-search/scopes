---
api_specs:
- filename: opply-openapi-original.yml
  format: yaml
  label: Opply API
  slug: opply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opply/refs/heads/main/openapi/opply-openapi-original.yml
authorization_urls:
- https://api.opply.com/api/v1/oauth/authorize/
description: ''
docs: https://api.opply.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Opply Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Opply publishes 29 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Opply API on a user''s behalf.


  Tokens are issued from https://api.opply.com/api/v1/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Opply
provider_slug: opply
schemes:
- flows:
  - authorizationUrl: https://api.opply.com/api/v1/oauth/authorize/
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://api.opply.com/api/v1/oauth/register/
    revocationUrl: https://api.opply.com/api/v1/oauth/revoke_token/
    tokenUrl: https://api.opply.com/api/v1/oauth/token/
  name: OAuth2
  source: https://api.opply.com/.well-known/oauth-authorization-server
scope_count: 29
scope_names:
- all:read
- all:write
- orders:read
- orders:write
- companies:read
- companies:write
- crm:read
- crm:write
- catalog:read
- catalog:write
- activities:read
- activities:write
- tasks:read
- tasks:write
- payments:read
- payments:write
- agreements:read
- agreements:write
- onboarding:read
- onboarding:write
- agents:read
- agents:write
- files:read
- insights:read
- recommendations:read
- recommendations:write
- zendesk:read
- zendesk:write
- unleashed:read
scopes:
- description: Read access across all resources
  flows: []
  scope: all:read
- description: Write access across all resources
  flows: []
  scope: all:write
- description: Read orders
  flows: []
  scope: orders:read
- description: Create and modify orders
  flows: []
  scope: orders:write
- description: Read companies
  flows: []
  scope: companies:read
- description: Create and modify companies
  flows: []
  scope: companies:write
- description: Read CRM data
  flows: []
  scope: crm:read
- description: Create and modify CRM data
  flows: []
  scope: crm:write
- description: Read catalog / ingredients
  flows: []
  scope: catalog:read
- description: Create and modify catalog / ingredients
  flows: []
  scope: catalog:write
- description: Read activity feed
  flows: []
  scope: activities:read
- description: Write activity feed items
  flows: []
  scope: activities:write
- description: Read tasks
  flows: []
  scope: tasks:read
- description: Create and modify tasks
  flows: []
  scope: tasks:write
- description: Read payments
  flows: []
  scope: payments:read
- description: Create and modify payments
  flows: []
  scope: payments:write
- description: Read agreements
  flows: []
  scope: agreements:read
- description: Create and modify agreements
  flows: []
  scope: agreements:write
- description: Read buyer onboarding
  flows: []
  scope: onboarding:read
- description: Create and modify buyer onboarding
  flows: []
  scope: onboarding:write
- description: Read agents
  flows: []
  scope: agents:read
- description: Create and modify agents
  flows: []
  scope: agents:write
- description: Read files
  flows: []
  scope: files:read
- description: Read insights
  flows: []
  scope: insights:read
- description: Read recommendations
  flows: []
  scope: recommendations:read
- description: Act on recommendations
  flows: []
  scope: recommendations:write
- description: Read Zendesk integration data (Zendesk MCP)
  flows: []
  scope: zendesk:read
- description: Write Zendesk integration data (Zendesk MCP)
  flows: []
  scope: zendesk:write
- description: Read Unleashed integration data (Unleashed MCP)
  flows: []
  scope: unleashed:read
slug: opply-scopes
source_filename: opply-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.opply.com/.well-known/oauth-authorization-server\ndocs: https://api.opply.com/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: https://api.opply.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.opply.com/api/v1/oauth/authorize/\n    tokenUrl: https://api.opply.com/api/v1/oauth/token/\n    revocationUrl: https://api.opply.com/api/v1/oauth/revoke_token/\n    registrationUrl: https://api.opply.com/api/v1/oauth/register/\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\nscopes:\n- {scope: 'all:read', description: Read access across all resources}\n- {scope: 'all:write', description: Write access across all resources}\n- {scope: 'orders:read', description: Read orders}\n- {scope: 'orders:write', description: Create and modify orders}\n- {scope: 'companies:read', description: Read companies}\n\
  - {scope: 'companies:write', description: Create and modify companies}\n- {scope: 'crm:read', description: Read CRM data}\n- {scope: 'crm:write', description: Create and modify CRM data}\n- {scope: 'catalog:read', description: Read catalog / ingredients}\n- {scope: 'catalog:write', description: Create and modify catalog / ingredients}\n- {scope: 'activities:read', description: Read activity feed}\n- {scope: 'activities:write', description: Write activity feed items}\n- {scope: 'tasks:read', description: Read tasks}\n- {scope: 'tasks:write', description: Create and modify tasks}\n- {scope: 'payments:read', description: Read payments}\n- {scope: 'payments:write', description: Create and modify payments}\n- {scope: 'agreements:read', description: Read agreements}\n- {scope: 'agreements:write', description: Create and modify agreements}\n- {scope: 'onboarding:read', description: Read buyer onboarding}\n- {scope: 'onboarding:write', description: Create and modify buyer onboarding}\n- {scope:\
  \ 'agents:read', description: Read agents}\n- {scope: 'agents:write', description: Create and modify agents}\n- {scope: 'files:read', description: Read files}\n- {scope: 'insights:read', description: Read insights}\n- {scope: 'recommendations:read', description: Read recommendations}\n- {scope: 'recommendations:write', description: Act on recommendations}\n- {scope: 'zendesk:read', description: Read Zendesk integration data (Zendesk MCP)}\n- {scope: 'zendesk:write', description: Write Zendesk integration data (Zendesk MCP)}\n- {scope: 'unleashed:read', description: Read Unleashed integration data (Unleashed MCP)}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opply/refs/heads/main/scopes/opply-scopes.yml
summary_line: 29 scopes · authorizationCode
tags:
- Company
- Food and Beverage
- Supply Chain
- Procurement
- Ordering
- Payments
- Sourcing
- Logistics
- AI Agents
- MCP
token_urls:
- https://api.opply.com/api/v1/oauth/token/
---
