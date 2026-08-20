---
authorization_urls: []
description: Campaign Monitor calls its OAuth 2.0 scopes "permissions". The complete list is published verbatim on the Getting Started page under "Permissions"; there is no OpenAPI and no /.well-known/oauth-authorization-server document, so this artifact was transcribed from the provider's own reference page rather than derived from a spec. Permissions are supplied on the authorize request as a single comma-separated `scope` query parameter (URL-encoded, e.g. SendCampaigns%2CViewReports).
docs: https://www.campaignmonitor.com/api/v3-3/getting-started/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Campaignmonitor Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Campaign Monitor uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Campaign Monitor
provider_slug: campaignmonitor
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: campaignmonitor-scopes
source_filename: campaignmonitor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.campaignmonitor.com/api/v3-3/getting-started/\ndocs: https://www.campaignmonitor.com/api/v3-3/getting-started/\ndescription: >-\n  Campaign Monitor calls its OAuth 2.0 scopes \"permissions\". The complete list is\n  published verbatim on the Getting Started page under \"Permissions\"; there is no\n  OpenAPI and no /.well-known/oauth-authorization-server document, so this\n  artifact was transcribed from the provider's own reference page rather than\n  derived from a spec. Permissions are supplied on the authorize request as a\n  single comma-separated `scope` query parameter (URL-encoded, e.g.\n  SendCampaigns%2CViewReports).\nauthorization_url: https://api.createsend.com/oauth\ntoken_url: https://api.createsend.com/oauth/token\ndelimiter: \",\"\nscope_count: 12\nscopes:\n  - name: ViewReports\n    description: Permission to view reports.\n  - name: ManageLists\n    description: Permission to manage lists.\n  -\
  \ name: CreateCampaigns\n    description: Permission to create campaigns.\n  - name: ImportSubscribers\n    description: Permission to import subscribers.\n  - name: SendCampaigns\n    description: Permission to send campaigns.\n  - name: ViewSubscribersInReports\n    description: Permission to view subscribers in reports.\n  - name: ManageTemplates\n    description: Permission to manage templates.\n  - name: AdministerPersons\n    description: Permission to administer persons.\n  - name: AdministerAccount\n    description: Permission to administer your account.\n  - name: ViewTransactional\n    description: Permission to view transactional reports and logs.\n  - name: SendTransactional\n    description: Permission to send transactional email.\n  - name: Automation\n    description: Permission to view journey reports.\nnotes:\n  - >-\n    Scopes are coarse and product-shaped rather than resource/verb-shaped: there\n    is no read-only variant of ManageLists or ManageTemplates, so an integration\n\
  \    that only needs to read lists must still request write permission.\n  - >-\n    Requesting a permission the API does not recognise fails the OAuth exchange\n    with unknown_scope; calling an endpoint outside the granted permissions\n    returns HTTP 401 with error code 60.\n  - >-\n    API-key authentication has no scope surface at all — an API key carries the\n    full rights of the account or client it belongs to.\nrelated:\n  - authentication/campaignmonitor-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campaignmonitor/refs/heads/main/scopes/campaignmonitor-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Email Marketing
- Campaigns
- Subscribers
- Transactional Email
- Segments
- Newsletters
- Automation
- Marketing Automation
- Webhook
- Email Deliverability
- Marketing
token_urls: []
---
