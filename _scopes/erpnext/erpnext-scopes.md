---
api_specs:
- filename: frappe_api-docs
  format: yaml
  label: ERPNext REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://github.com/alyf-de/frappe_api-docs
authorization_urls:
- /method/frappe.integrations.oauth2.authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Erpnext Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ERPNext publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ERPNext API on a user''s behalf.


  Tokens are issued from /method/frappe.integrations.oauth2.get_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ERPNext
provider_slug: erpnext
schemes:
- description: "This API uses OAuth 2 with the authorization code flow. \n[More info]https://frappe.io/docs/user/en/guides/integration/using_oauth)"
  flows:
  - authorizationUrl: /method/frappe.integrations.oauth2.authorize
    flow: authorizationCode
    tokenUrl: /method/frappe.integrations.oauth2.get_token
  name: oAuth2
  source: openapi/openapi.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Same permissions as the user who created the oAuth client
  flows:
  - authorizationCode
  scope: all
slug: erpnext-scopes
source_filename: erpnext-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nschemes:\n- name: oAuth2\n  source: openapi/openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /method/frappe.integrations.oauth2.authorize\n    tokenUrl: /method/frappe.integrations.oauth2.get_token\n  description: \"This API uses OAuth 2 with the authorization code flow. \\n[More info]https://frappe.io/docs/user/en/guides/integration/using_oauth)\"\nscopes:\n- scope: all\n  description: Same permissions as the user who created the oAuth client\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erpnext/refs/heads/main/scopes/erpnext-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- ERP
- Enterprise Resource Planning
- Accounting
- Inventory
- Manufacturing
- Sales
- CRM
- HR
- Open Source
token_urls:
- /method/frappe.integrations.oauth2.get_token
---
