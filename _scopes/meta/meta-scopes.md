---
api_specs:
- filename: meta-openapi.yml
  format: yaml
  label: Facebook Graph API - User
  slug: facebook-graph-api-user
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/openapi/meta-openapi.yml
authorization_urls:
- https://www.facebook.com/v25.0/dialog/oauth
description: Meta uses OAuth 2.0 "permissions" as its scope surface (Facebook Login / Graph API). The baseline (public_profile) was derived from openapi/meta-openapi.yml; the remaining entries are the canonical documented permissions from the Meta Permissions Reference (https://developers.facebook.com/docs/permissions). Most permissions require App Review before use in Production. This is a representative subset across the major products, not the full registry.
docs: https://developers.facebook.com/docs/permissions
flows:
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Meta Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Meta publishes 15 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Meta API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Meta
provider_slug: meta
schemes:
- flows:
  - authorizationUrl: https://www.facebook.com/v25.0/dialog/oauth
    flow: implicit
  name: userAccessToken
  source: openapi/meta-openapi.yml
scope_count: 15
scope_names:
- public_profile
- email
- pages_show_list
- pages_read_engagement
- pages_manage_posts
- instagram_basic
- instagram_content_publish
- instagram_manage_messages
- ads_read
- ads_management
- business_management
- whatsapp_business_messaging
- whatsapp_business_management
- threads_basic
- threads_content_publish
scopes:
- description: Access basic profile info (name, profile picture).
  flows:
  - implicit
  scope: public_profile
- description: Access the person's primary email address.
  flows: []
  scope: email
- description: Read the list of Pages a person manages.
  flows: []
  scope: pages_show_list
- description: Read content, metadata, and engagement on Pages a person manages.
  flows: []
  scope: pages_read_engagement
- description: Create, edit, and delete Page posts.
  flows: []
  scope: pages_manage_posts
- description: Read an Instagram Business/Creator account profile and media.
  flows: []
  scope: instagram_basic
- description: Publish media to an Instagram Business/Creator account.
  flows: []
  scope: instagram_content_publish
- description: Send and receive messages on Instagram.
  flows: []
  scope: instagram_manage_messages
- description: Read ad account campaigns, ad sets, ads, and insights.
  flows: []
  scope: ads_read
- description: Create and manage ads and audiences.
  flows: []
  scope: ads_management
- description: Read and manage business assets (Business Manager).
  flows: []
  scope: business_management
- description: Send and receive WhatsApp messages via the Cloud API.
  flows: []
  scope: whatsapp_business_messaging
- description: Manage WhatsApp Business accounts, phone numbers, and templates.
  flows: []
  scope: whatsapp_business_management
- description: Read a Threads profile and content.
  flows: []
  scope: threads_basic
- description: Publish content to Threads.
  flows: []
  scope: threads_content_publish
slug: meta-scopes
source_filename: meta-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/meta-openapi.yml\ndocs: https://developers.facebook.com/docs/permissions\ndescription: >-\n  Meta uses OAuth 2.0 \"permissions\" as its scope surface (Facebook Login /\n  Graph API). The baseline (public_profile) was derived from\n  openapi/meta-openapi.yml; the remaining entries are the canonical documented\n  permissions from the Meta Permissions Reference\n  (https://developers.facebook.com/docs/permissions). Most permissions require\n  App Review before use in Production. This is a representative subset across\n  the major products, not the full registry.\nschemes:\n  - name: userAccessToken\n    source: openapi/meta-openapi.yml\n    flows:\n      - flow: implicit\n        authorizationUrl: https://www.facebook.com/v25.0/dialog/oauth\nscopes:\n  - scope: public_profile\n    description: Access basic profile info (name, profile picture).\n    flows: [implicit]\n    sources: [openapi/meta-openapi.yml]\n  - scope:\
  \ email\n    description: Access the person's primary email address.\n    product: facebook-login\n  - scope: pages_show_list\n    description: Read the list of Pages a person manages.\n    product: pages\n  - scope: pages_read_engagement\n    description: Read content, metadata, and engagement on Pages a person manages.\n    product: pages\n  - scope: pages_manage_posts\n    description: Create, edit, and delete Page posts.\n    product: pages\n  - scope: instagram_basic\n    description: Read an Instagram Business/Creator account profile and media.\n    product: instagram\n  - scope: instagram_content_publish\n    description: Publish media to an Instagram Business/Creator account.\n    product: instagram\n  - scope: instagram_manage_messages\n    description: Send and receive messages on Instagram.\n    product: instagram\n  - scope: ads_read\n    description: Read ad account campaigns, ad sets, ads, and insights.\n    product: marketing-api\n  - scope: ads_management\n    description:\
  \ Create and manage ads and audiences.\n    product: marketing-api\n  - scope: business_management\n    description: Read and manage business assets (Business Manager).\n    product: business\n  - scope: whatsapp_business_messaging\n    description: Send and receive WhatsApp messages via the Cloud API.\n    product: whatsapp\n  - scope: whatsapp_business_management\n    description: Manage WhatsApp Business accounts, phone numbers, and templates.\n    product: whatsapp\n  - scope: threads_basic\n    description: Read a Threads profile and content.\n    product: threads\n  - scope: threads_content_publish\n    description: Publish content to Threads.\n    product: threads\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/scopes/meta-scopes.yml
summary_line: 15 scopes · implicit
tags:
- Advertising
- Analytics
- Artificial Intelligence
- Messaging
- Social
- Social Media
- Virtual Reality
token_urls: []
---
