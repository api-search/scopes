---
api_specs:
- filename: facebook-lead-ads-openapi.yml
  format: yaml
  label: Meta Marketing API - Lead Ads
  slug: graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-openapi.yml
authorization_urls:
- https://www.facebook.com/v22.0/dialog/oauth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Facebook Lead Ads Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Facebook Lead Ads publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Facebook Lead Ads API on a user''s behalf.


  Tokens are issued from https://graph.facebook.com/v22.0/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Facebook Lead Ads
provider_slug: facebook-lead-ads
schemes:
- description: 'Page access token obtained via Facebook Login / Meta Business

    Login with leads_retrieval, pages_show_list, and

    pages_manage_ads permissions.'
  flows:
  - authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth
    flow: authorizationCode
    tokenUrl: https://graph.facebook.com/v22.0/oauth/access_token
  name: PageAccessToken
  source: openapi/facebook-lead-ads-openapi.yml
scope_count: 3
scope_names:
- leads_retrieval
- pages_manage_ads
- pages_show_list
scopes:
- description: Read leads from lead ad forms
  flows:
  - authorizationCode
  scope: leads_retrieval
- description: Manage ads associated with a Page
  flows:
  - authorizationCode
  scope: pages_manage_ads
- description: List Pages the user manages
  flows:
  - authorizationCode
  scope: pages_show_list
slug: facebook-lead-ads-scopes
source_filename: facebook-lead-ads-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/facebook-lead-ads-openapi.yml\nschemes:\n- name: PageAccessToken\n  source: openapi/facebook-lead-ads-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth\n    tokenUrl: https://graph.facebook.com/v22.0/oauth/access_token\n  description: |-\n    Page access token obtained via Facebook Login / Meta Business\n    Login with leads_retrieval, pages_show_list, and\n    pages_manage_ads permissions.\nscopes:\n- scope: leads_retrieval\n  description: Read leads from lead ad forms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/facebook-lead-ads-openapi.yml\n- scope: pages_manage_ads\n  description: Manage ads associated with a Page\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/facebook-lead-ads-openapi.yml\n- scope: pages_show_list\n  description: List Pages the user manages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/facebook-lead-ads-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/scopes/facebook-lead-ads-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Advertising
- Lead Generation
- Lead Ads
- Marketing API
- Facebook
- Instagram
- Meta
- Webhooks
token_urls:
- https://graph.facebook.com/v22.0/oauth/access_token
---
