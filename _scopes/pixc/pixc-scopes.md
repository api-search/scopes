---
api_specs:
- filename: schema
  format: yaml
  label: Pixc Public API
  slug: pixc-public-api
  spec_type: OpenAPI
  url: https://dashboard.pixc.com/v1/schema
authorization_urls:
- https://dashboard.pixc.com/v1/oauth
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Pixc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pixc publishes 11 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pixc API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pixc
provider_slug: pixc
schemes:
- description: 'OAuth 2.0 implicit flow. A personal Access Token can also be obtained from Account Settings > API Access in the Pixc Dashboard and sent as `Authorization: Bearer ACCESS_TOKEN`.'
  flows:
  - authorizationUrl: https://dashboard.pixc.com/v1/oauth
    flow: implicit
  name: pixc_auth
  source: openapi/pixc-orders-api-openapi.yml
- description: 'OAuth 2.0 implicit flow. A personal Access Token can also be obtained from Account Settings > API Access in the Pixc Dashboard and sent as `Authorization: Bearer ACCESS_TOKEN`.'
  flows:
  - authorizationUrl: https://dashboard.pixc.com/v1/oauth
    flow: implicit
  name: pixc_auth
  source: openapi/pixc-templates-api-openapi.yml
- description: 'OAuth 2.0 implicit flow. A personal Access Token can also be obtained from Account Settings > API Access in the Pixc Dashboard and sent as `Authorization: Bearer ACCESS_TOKEN`.'
  flows:
  - authorizationUrl: https://dashboard.pixc.com/v1/oauth
    flow: implicit
  name: pixc_auth
  source: openapi/pixc-webhooks-api-openapi.yml
scope_count: 11
scope_names:
- api:order:cancel
- api:order:create
- api:order:view
- api:template:create
- api:template:remove
- api:template:update
- api:template:view
- api:webhook:create
- api:webhook:remove
- api:webhook:update
- api:webhook:view
scopes:
- description: Cancel orders
  flows:
  - implicit
  scope: api:order:cancel
- description: Create new orders
  flows:
  - implicit
  scope: api:order:create
- description: View orders
  flows:
  - implicit
  scope: api:order:view
- description: Create new templates
  flows:
  - implicit
  scope: api:template:create
- description: Remove templates
  flows:
  - implicit
  scope: api:template:remove
- description: Update templates
  flows:
  - implicit
  scope: api:template:update
- description: View templates
  flows:
  - implicit
  scope: api:template:view
- description: Create new webhook
  flows:
  - implicit
  scope: api:webhook:create
- description: Remove webhook
  flows:
  - implicit
  scope: api:webhook:remove
- description: Update webhook
  flows:
  - implicit
  scope: api:webhook:update
- description: View webhooks
  flows:
  - implicit
  scope: api:webhook:view
slug: pixc-scopes
source_filename: pixc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/pixc-orders-api-openapi.yml, openapi/pixc-templates-api-openapi.yml, openapi/pixc-webhooks-api-openapi.yml\nschemes:\n- name: pixc_auth\n  source: openapi/pixc-orders-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://dashboard.pixc.com/v1/oauth\n  description: 'OAuth 2.0 implicit flow. A personal Access Token can also be obtained from Account\n    Settings > API Access in the Pixc Dashboard and sent as `Authorization: Bearer ACCESS_TOKEN`.'\n- name: pixc_auth\n  source: openapi/pixc-templates-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://dashboard.pixc.com/v1/oauth\n  description: 'OAuth 2.0 implicit flow. A personal Access Token can also be obtained from Account\n    Settings > API Access in the Pixc Dashboard and sent as `Authorization: Bearer ACCESS_TOKEN`.'\n- name: pixc_auth\n  source: openapi/pixc-webhooks-api-openapi.yml\n  flows:\n  - flow: implicit\n\
  \    authorizationUrl: https://dashboard.pixc.com/v1/oauth\n  description: 'OAuth 2.0 implicit flow. A personal Access Token can also be obtained from Account\n    Settings > API Access in the Pixc Dashboard and sent as `Authorization: Bearer ACCESS_TOKEN`.'\nscopes:\n- scope: api:order:cancel\n  description: Cancel orders\n  flows:\n  - implicit\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n  - openapi/pixc-webhooks-api-openapi.yml\n- scope: api:order:create\n  description: Create new orders\n  flows:\n  - implicit\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n  - openapi/pixc-webhooks-api-openapi.yml\n- scope: api:order:view\n  description: View orders\n  flows:\n  - implicit\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n  - openapi/pixc-webhooks-api-openapi.yml\n- scope: api:template:create\n  description: Create new templates\n\
  \  flows:\n  - implicit\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n  - openapi/pixc-webhooks-api-openapi.yml\n- scope: api:template:remove\n  description: Remove templates\n  flows:\n  - implicit\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n  - openapi/pixc-webhooks-api-openapi.yml\n- scope: api:template:update\n  description: Update templates\n  flows:\n  - implicit\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n  - openapi/pixc-webhooks-api-openapi.yml\n- scope: api:template:view\n  description: View templates\n  flows:\n  - implicit\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n  - openapi/pixc-webhooks-api-openapi.yml\n- scope: api:webhook:create\n  description: Create new webhook\n  flows:\n  - implicit\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n\
  \  - openapi/pixc-webhooks-api-openapi.yml\n- scope: api:webhook:remove\n  description: Remove webhook\n  flows:\n  - implicit\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n  - openapi/pixc-webhooks-api-openapi.yml\n- scope: api:webhook:update\n  description: Update webhook\n  flows:\n  - implicit\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n  - openapi/pixc-webhooks-api-openapi.yml\n- scope: api:webhook:view\n  description: View webhooks\n  flows:\n  - implicit\n  sources:\n  - openapi/pixc-orders-api-openapi.yml\n  - openapi/pixc-templates-api-openapi.yml\n  - openapi/pixc-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixc/refs/heads/main/scopes/pixc-scopes.yml
summary_line: 11 scopes · implicit
tags:
- Company
- Shopify
- E-Commerce
- Photo Editing
- Image Optimization
- Image Processing
- Product Photography
- Background Removal
- SEO
- Automation
- Artificial Intelligence
- Webhook
- Digital Asset Management
token_urls: []
---
