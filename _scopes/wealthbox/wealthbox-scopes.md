---
authorization_urls:
- https://app.crmworkspace.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wealthbox Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wealthbox publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wealthbox API on a user''s behalf.


  Tokens are issued from https://app.crmworkspace.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wealthbox
provider_slug: wealthbox
schemes:
- description: OAuth 2.0 authorization code flow for third-party integrations.
  flows:
  - authorizationUrl: https://app.crmworkspace.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.crmworkspace.com/oauth/token
  name: oauth2
  source: openapi/wealthbox-openapi.yml
scope_count: 2
scope_names:
- data
- login
scopes:
- description: Read and write CRM data
  flows:
  - authorizationCode
  scope: data
- description: Access basic profile information
  flows:
  - authorizationCode
  scope: login
slug: wealthbox-scopes
source_filename: wealthbox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wealthbox-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/wealthbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.crmworkspace.com/oauth/authorize\n    tokenUrl: https://app.crmworkspace.com/oauth/token\n  description: OAuth 2.0 authorization code flow for third-party integrations.\nscopes:\n- scope: data\n  description: Read and write CRM data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wealthbox-openapi.yml\n- scope: login\n  description: Access basic profile information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wealthbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/scopes/wealthbox-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- CRM
- Financial Advisors
- Wealth Management
- Contact Management
- Workflow Automation
- SaaS
token_urls:
- https://app.crmworkspace.com/oauth/token
---
