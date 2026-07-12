---
authorization_urls:
- https://webflow.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Webflow Api And Documentation Webflow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Webflow API and Documentation publishes 29 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Webflow API and Documentation API on a user''s behalf.


  Tokens are issued from https://api.webflow.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Webflow API and Documentation
provider_slug: webflow-api-and-documentation-webflow
schemes:
- flows:
  - authorizationUrl: https://webflow.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.webflow.com/oauth/token
  name: OAuth2
  source: openapi/webflow-collections-openapi.yml
- flows:
  - authorizationUrl: https://webflow.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.webflow.com/oauth/token
  name: OAuth2
  source: openapi/webflow-data-api-openapi.yml
- flows:
  - authorizationUrl: https://webflow.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.webflow.com/oauth/token
  name: OAuth2
  source: openapi/webflow-items-openapi.yml
- flows:
  - authorizationUrl: https://webflow.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.webflow.com/oauth/token
  name: OAuth2
  source: openapi/webflow-sites-openapi.yml
- flows:
  - authorizationUrl: https://webflow.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.webflow.com/oauth/token
  name: OAuth2
  source: openapi/webflow-webhooks-openapi.yml
scope_count: 29
scope_names:
- assets:read
- assets:write
- authorized_user:read
- cms:read
- cms:write
- comments:read
- comments:write
- components:read
- components:write
- custom_code:read
- custom_code:write
- ecommerce:read
- ecommerce:write
- forms:read
- forms:write
- page:read
- page:write
- pages:read
- pages:write
- site_activity:read
- site_config:read
- site_config:write
- sites:read
- sites:write
- users:read
- users:write
- workspace:read
- workspace:write
- workspace_activity:read
scopes:
- description: read assets on the site
  flows:
  - authorizationCode
  scope: assets:read
- description: write assets on a site
  flows:
  - authorizationCode
  scope: assets:write
- description: read details about the authorized user
  flows:
  - authorizationCode
  scope: authorized_user:read
- description: read collections and items for a site
  flows:
  - authorizationCode
  scope: cms:read
- description: write to collections and items for a site
  flows:
  - authorizationCode
  scope: cms:write
- description: read comments on the site
  flows:
  - authorizationCode
  scope: comments:read
- description: write comments on the site
  flows:
  - authorizationCode
  scope: comments:write
- description: read component data
  flows:
  - authorizationCode
  scope: components:read
- description: write component data
  flows:
  - authorizationCode
  scope: components:write
- description: read custom code on the site
  flows:
  - authorizationCode
  scope: custom_code:read
- description: modify custom code on the site
  flows:
  - authorizationCode
  scope: custom_code:write
- description: read ecommerce data
  flows:
  - authorizationCode
  scope: ecommerce:read
- description: edit ecommerce data
  flows:
  - authorizationCode
  scope: ecommerce:write
- description: read form data
  flows:
  - authorizationCode
  scope: forms:read
- description: write form data
  flows:
  - authorizationCode
  scope: forms:write
- description: ''
  flows: []
  scope: page:read
- description: ''
  flows: []
  scope: page:write
- description: read pages on the site
  flows:
  - authorizationCode
  scope: pages:read
- description: write to pages on the site
  flows:
  - authorizationCode
  scope: pages:write
- description: read site activity logs
  flows:
  - authorizationCode
  scope: site_activity:read
- description: read site configuration data
  flows:
  - authorizationCode
  scope: site_config:read
- description: write site configuration data
  flows:
  - authorizationCode
  scope: site_config:write
- description: read sites on the site
  flows:
  - authorizationCode
  scope: sites:read
- description: modify pages on the site
  flows:
  - authorizationCode
  scope: sites:write
- description: read users on the site
  flows:
  - authorizationCode
  scope: users:read
- description: modify users on the site
  flows:
  - authorizationCode
  scope: users:write
- description: read workspace resource data
  flows:
  - authorizationCode
  scope: workspace:read
- description: write workspace resource data
  flows:
  - authorizationCode
  scope: workspace:write
- description: ''
  flows: []
  scope: workspace_activity:read
slug: webflow-api-and-documentation-webflow-scopes
source_filename: webflow-api-and-documentation-webflow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/webflow-collections-openapi.yml, openapi/webflow-data-api-openapi.yml, openapi/webflow-items-openapi.yml,\n  openapi/webflow-sites-openapi.yml, openapi/webflow-webhooks-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/webflow-collections-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://webflow.com/oauth/authorize\n    tokenUrl: https://api.webflow.com/oauth/token\n- name: OAuth2\n  source: openapi/webflow-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://webflow.com/oauth/authorize\n    tokenUrl: https://api.webflow.com/oauth/token\n- name: OAuth2\n  source: openapi/webflow-items-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://webflow.com/oauth/authorize\n    tokenUrl: https://api.webflow.com/oauth/token\n- name: OAuth2\n  source: openapi/webflow-sites-openapi.yml\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://webflow.com/oauth/authorize\n    tokenUrl: https://api.webflow.com/oauth/token\n- name: OAuth2\n  source: openapi/webflow-webhooks-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://webflow.com/oauth/authorize\n    tokenUrl: https://api.webflow.com/oauth/token\nscopes:\n- scope: assets:read\n  description: read assets on the site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: assets:write\n  description: write assets on a site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: authorized_user:read\n  description:\
  \ read details about the authorized user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: cms:read\n  description: read collections and items for a site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: cms:write\n  description: write to collections and items for a site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: comments:read\n  description: read comments\
  \ on the site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: comments:write\n  description: write comments on the site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: components:read\n  description: read component data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: components:write\n  description: write component data\n  flows:\n  - authorizationCode\n \
  \ sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: custom_code:read\n  description: read custom code on the site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: custom_code:write\n  description: modify custom code on the site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: ecommerce:read\n  description: read ecommerce data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n\
  \  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: ecommerce:write\n  description: edit ecommerce data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: forms:read\n  description: read form data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: forms:write\n  description: write form data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n\
  \  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: page:read\n  sources:\n  - openapi/webflow-data-api-openapi.yml\n- scope: page:write\n  sources:\n  - openapi/webflow-data-api-openapi.yml\n- scope: pages:read\n  description: read pages on the site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: pages:write\n  description: write to pages on the site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: site_activity:read\n  description: read site activity logs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n\
  \  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: site_config:read\n  description: read site configuration data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: site_config:write\n  description: write site configuration data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: sites:read\n  description: read sites on the site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n\
  \  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: sites:write\n  description: modify pages on the site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: users:read\n  description: read users on the site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: users:write\n  description: modify users on the site\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n\
  \  - openapi/webflow-webhooks-openapi.yml\n- scope: workspace:read\n  description: read workspace resource data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: workspace:write\n  description: write workspace resource data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- scope: workspace_activity:read\n  sources:\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webflow-api-and-documentation-webflow/refs/heads/main/scopes/webflow-api-and-documentation-webflow-scopes.yml
summary_line: 29 scopes · authorizationCode
tags:
- CMS
- Content Management
- Ecommerce
- No-Code
- Publishing
- Web Development
token_urls:
- https://api.webflow.com/oauth/token
---
