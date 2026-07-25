---
api_specs:
- filename: keap-resthooks-asyncapi.yml
  format: yaml
  label: Keap REST Hooks
  slug: rest-hooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/asyncapi/keap-resthooks-asyncapi.yml
- filename: keap-campaigns-api-openapi.yml
  format: yaml
  label: Keap Campaigns API
  slug: keap-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/openapi/keap-campaigns-api-openapi.yml
- filename: keap-companies-api-openapi.yml
  format: yaml
  label: Keap Companies API
  slug: keap-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/openapi/keap-companies-api-openapi.yml
- filename: keap-contacts-api-openapi.yml
  format: yaml
  label: Keap Contacts API
  slug: keap-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/openapi/keap-contacts-api-openapi.yml
- filename: keap-opportunities-api-openapi.yml
  format: yaml
  label: Keap Opportunities API
  slug: keap-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/openapi/keap-opportunities-api-openapi.yml
- filename: keap-orders-api-openapi.yml
  format: yaml
  label: Keap Orders API
  slug: keap-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/openapi/keap-orders-api-openapi.yml
- filename: keap-products-api-openapi.yml
  format: yaml
  label: Keap Products API
  slug: keap-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/openapi/keap-products-api-openapi.yml
- filename: keap-tags-api-openapi.yml
  format: yaml
  label: Keap Tags API
  slug: keap-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/openapi/keap-tags-api-openapi.yml
- filename: keap-tasks-api-openapi.yml
  format: yaml
  label: Keap Tasks API
  slug: keap-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/openapi/keap-tasks-api-openapi.yml
authorization_urls:
- https://accounts.infusionsoft.com/app/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Keap Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Keap publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Keap API on a user''s behalf.


  Tokens are issued from https://api.infusionsoft.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Keap
provider_slug: keap
schemes:
- description: Keap uses OAuth 2.0 for authentication. See https://developer.infusionsoft.com/getting-started-oauth-keys/
  flows:
  - authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.infusionsoft.com/token
  name: oauth2
  source: openapi/keap-openapi.yml
scope_count: 1
scope_names:
- full
scopes:
- description: Full access to the Keap CRM REST API.
  flows:
  - authorizationCode
  scope: full
slug: keap-scopes
source_filename: keap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keap-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/keap-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize\n    tokenUrl: https://api.infusionsoft.com/token\n  description: Keap uses OAuth 2.0 for authentication. See https://developer.infusionsoft.com/getting-started-oauth-keys/\nscopes:\n- scope: full\n  description: Full access to the Keap CRM REST API.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/keap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/scopes/keap-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- CRM
- Sales
- Marketing Automation
- Small Business
- E-Commerce
- Contacts
token_urls:
- https://api.infusionsoft.com/token
---
