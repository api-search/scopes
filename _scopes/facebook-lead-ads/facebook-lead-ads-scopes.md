---
api_specs:
- filename: facebook-lead-ads-bulk-leads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Bulk Leads API
  slug: facebook-lead-ads-bulk-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-bulk-leads-api-openapi.yml
- filename: facebook-lead-ads-leadgen-forms-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Leadgen Forms API
  slug: facebook-lead-ads-leadgen-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-leadgen-forms-api-openapi.yml
- filename: facebook-lead-ads-leads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Leads API
  slug: facebook-lead-ads-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-leads-api-openapi.yml
- filename: facebook-lead-ads-meta-marketing-api-lead-ads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Meta Marketing API Lead Ads API
  slug: facebook-lead-ads-meta-marketing-api-lead-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-meta-marketing-api-lead-ads-api-openapi.yml
- filename: facebook-lead-ads-subscribed-apps-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Subscribed Apps API
  slug: facebook-lead-ads-subscribed-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-subscribed-apps-api-openapi.yml
- filename: facebook-lead-ads-subscriptions-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Subscriptions API
  slug: facebook-lead-ads-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-subscriptions-api-openapi.yml
authorization_urls:
- https://www.facebook.com/v22.0/dialog/oauth
description: ''
docs: https://developers.facebook.com/docs/permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Facebook Lead Ads Scopes
name_suffix: OAuth Scopes
note: 'Upgraded from derived to searched. The OpenAPI in this repo declares three scopes; Meta''s lead-ads retrieval guide documents six, and which subset you need depends on WHICH lead fields you read — ad-level fields (ad_id, campaign_id) require a different permission set than the lead body. The three the spec omits are recorded below with in_spec: false so the gap stays visible. Meta calls these "permissions", not "scopes"; they are OAuth 2.0 scope strings on the wire. Every permission is additionally gated by an ACCESS LEVEL (Standard vs Advanced) — see plans/facebook-lead-ads-plans-pricing.yml — so being granted a scope and being able to use it against arbitrary users are two different things.'
overview: 'Facebook Lead Ads publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Facebook Lead Ads API on a user''s behalf.


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
scope_count: 6
scope_names:
- leads_retrieval
- pages_show_list
- pages_manage_ads
- ads_management
- pages_read_engagement
- pages_manage_metadata
scopes:
- description: Read leads from lead ad forms. The core permission for this product — without it, /{form-id}/leads and /{lead-id} return an error rather than lead data.
  flows:
  - authorizationCode
  scope: leads_retrieval
- description: List the Pages a user manages — needed to resolve the page-id that owns the forms.
  flows:
  - authorizationCode
  scope: pages_show_list
- description: Manage ads associated with a Page.
  flows:
  - authorizationCode
  scope: pages_manage_ads
- description: Required to read ad-level lead fields (ad_id, campaign_id) and for the full lead-data permission set documented on the retrieval guide.
  flows:
  - authorizationCode
  scope: ads_management
- description: Required alongside ads_management for ad-level fields and for the full lead-data permission set.
  flows:
  - authorizationCode
  scope: pages_read_engagement
- description: Required to subscribe a Page to leadgen webhooks — the operations subscribeAppWebhook and pageSubscribedApps in this repo.
  flows:
  - authorizationCode
  scope: pages_manage_metadata
slug: facebook-lead-ads-scopes
source_filename: facebook-lead-ads-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/facebook-lead-ads-openapi.yml\ndocs: https://developers.facebook.com/docs/permissions\nalso:\n  - https://developers.facebook.com/docs/marketing-api/guides/lead-ads/retrieving\n  - https://developers.facebook.com/docs/marketing-api/guides/lead-ads/\n  - https://developers.facebook.com/docs/graph-api/overview/access-levels\nnote: >-\n  Upgraded from derived to searched. The OpenAPI in this repo declares three scopes; Meta's\n  lead-ads retrieval guide documents six, and which subset you need depends on WHICH lead\n  fields you read — ad-level fields (ad_id, campaign_id) require a different permission set\n  than the lead body. The three the spec omits are recorded below with\n  in_spec: false so the gap stays visible.\n  Meta calls these \"permissions\", not \"scopes\"; they are OAuth 2.0 scope strings on the\n  wire. Every permission is additionally gated by an ACCESS LEVEL (Standard vs Advanced) —\n  see plans/facebook-lead-ads-plans-pricing.yml\
  \ — so being granted a scope and being able to\n  use it against arbitrary users are two different things.\nschemes:\n  - name: PageAccessToken\n    source: openapi/facebook-lead-ads-openapi.yml\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth\n        tokenUrl: https://graph.facebook.com/v22.0/oauth/access_token\n    description: |-\n      Page access token obtained via Facebook Login / Meta Business\n      Login with leads_retrieval, pages_show_list, and\n      pages_manage_ads permissions.\nscopes:\n  - scope: leads_retrieval\n    description: >-\n      Read leads from lead ad forms. The core permission for this product — without it,\n      /{form-id}/leads and /{lead-id} return an error rather than lead data.\n    flows: [authorizationCode]\n    in_spec: true\n    app_review_required: true\n    sources: [openapi/facebook-lead-ads-openapi.yml]\n  - scope: pages_show_list\n    description: List the Pages a user manages\
  \ — needed to resolve the page-id that owns the forms.\n    flows: [authorizationCode]\n    in_spec: true\n    sources: [openapi/facebook-lead-ads-openapi.yml]\n  - scope: pages_manage_ads\n    description: Manage ads associated with a Page.\n    flows: [authorizationCode]\n    in_spec: true\n    app_review_required: true\n    sources: [openapi/facebook-lead-ads-openapi.yml]\n  - scope: ads_management\n    description: >-\n      Required to read ad-level lead fields (ad_id, campaign_id) and for the full lead-data\n      permission set documented on the retrieval guide.\n    flows: [authorizationCode]\n    in_spec: false\n    sources: [https://developers.facebook.com/docs/marketing-api/guides/lead-ads/retrieving]\n  - scope: pages_read_engagement\n    description: >-\n      Required alongside ads_management for ad-level fields and for the full lead-data\n      permission set.\n    flows: [authorizationCode]\n    in_spec: false\n    sources: [https://developers.facebook.com/docs/marketing-api/guides/lead-ads/retrieving]\n\
  \  - scope: pages_manage_metadata\n    description: >-\n      Required to subscribe a Page to leadgen webhooks — the operations subscribeAppWebhook\n      and pageSubscribedApps in this repo.\n    flows: [authorizationCode]\n    in_spec: false\n    webhooks_only: true\n    sources: [https://developers.facebook.com/docs/marketing-api/guides/lead-ads/retrieving]\npermission_sets:\n  - use_case: Read ad-level fields (ad_id, campaign_id)\n    scopes: [ads_management, pages_read_engagement, pages_show_list]\n    plus_for_webhooks: [pages_manage_metadata]\n  - use_case: Read all lead data and ad-level data\n    scopes: [ads_management, leads_retrieval, pages_show_list, pages_read_engagement, pages_manage_ads]\n  - use_case: App Review submission for lead ads\n    scopes: [leads_retrieval, pages_manage_ads]\n    note: The two permissions Meta's lead ads guide names as requiring App Review.\naccess_levels:\n  detail: plans/facebook-lead-ads-plans-pricing.yml\n  levels:\n    - name: Standard Access\n\
  \      description: The permission works only for users who have a role on the app.\n    - name: Advanced Access\n      description: >-\n        The permission works for any app user; requires Business Verification and\n        App Review.\nsummary:\n  total: 6\n  in_spec: 3\n  docs_only: 3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/scopes/facebook-lead-ads-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Advertising
- Lead Generation
- Lead Ads
- Marketing API
- Facebook
- Instagram
- Meta
- Webhook
token_urls:
- https://graph.facebook.com/v22.0/oauth/access_token
---
