---
api_specs:
- filename: facebook-business-manager-ad-accounts-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Accounts API
  slug: facebook-business-manager-ad-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-accounts-api-openapi.yml
- filename: facebook-business-manager-ad-creatives-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Creatives API
  slug: facebook-business-manager-ad-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-creatives-api-openapi.yml
- filename: facebook-business-manager-ad-images-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Images API
  slug: facebook-business-manager-ad-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-images-api-openapi.yml
- filename: facebook-business-manager-ad-sets-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Sets API
  slug: facebook-business-manager-ad-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-sets-api-openapi.yml
- filename: facebook-business-manager-ads-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ads API
  slug: facebook-business-manager-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ads-api-openapi.yml
- filename: facebook-business-manager-campaigns-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Campaigns API
  slug: facebook-business-manager-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-campaigns-api-openapi.yml
- filename: facebook-business-manager-comments-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Comments API
  slug: facebook-business-manager-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-comments-api-openapi.yml
- filename: facebook-business-manager-custom-audiences-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Custom Audiences API
  slug: facebook-business-manager-custom-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-custom-audiences-api-openapi.yml
- filename: facebook-business-manager-insights-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Insights API
  slug: facebook-business-manager-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-insights-api-openapi.yml
- filename: facebook-business-manager-page-insights-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Page Insights API
  slug: facebook-business-manager-page-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-page-insights-api-openapi.yml
- filename: facebook-business-manager-pages-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Pages API
  slug: facebook-business-manager-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-pages-api-openapi.yml
- filename: facebook-business-manager-photos-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Photos API
  slug: facebook-business-manager-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-photos-api-openapi.yml
- filename: facebook-business-manager-posts-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Posts API
  slug: facebook-business-manager-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-posts-api-openapi.yml
- filename: facebook-business-manager-videos-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Videos API
  slug: facebook-business-manager-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-videos-api-openapi.yml
authorization_urls: []
description: 'Meta calls OAuth scopes "permissions" and publishes them in a single Permissions Reference for Meta Technologies APIs. Permissions are app-user-granted and gated by App Review; Advanced Access to any permission additionally requires Business Verification. The list below was read from that reference page on 2026-08-13, plus the machine-readable scopes_supported arrays served by Meta''s two MCP servers at /.well-known/oauth-protected-resource/{ads,devtools}. Note: derive-oauth-scopes.py produced nothing for this repo because the OpenAPI files in openapi/ declare a bearer http securityScheme rather than an oauth2 scheme with a scopes map — the scopes below are searched from the docs, not derived from a spec.'
docs: https://developers.facebook.com/docs/permissions
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Facebook Business Manager Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Facebook Business Manager uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Facebook Business Manager
provider_slug: facebook-business-manager
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: facebook-business-manager-scopes
source_filename: facebook-business-manager-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.facebook.com/docs/permissions\ndocs: https://developers.facebook.com/docs/permissions\nspecification: API Commons OAuthScopes\nspecificationVersion: '0.1'\nprovider: Facebook Business Manager\nproviderId: facebook-business-manager\ndescription: >-\n  Meta calls OAuth scopes \"permissions\" and publishes them in a single Permissions Reference for Meta\n  Technologies APIs. Permissions are app-user-granted and gated by App Review; Advanced Access to any\n  permission additionally requires Business Verification. The list below was read from that reference page on\n  2026-08-13, plus the machine-readable scopes_supported arrays served by Meta's two MCP servers at\n  /.well-known/oauth-protected-resource/{ads,devtools}.\n  Note: derive-oauth-scopes.py produced nothing for this repo because the OpenAPI files in openapi/ declare a\n  bearer http securityScheme rather than an oauth2 scheme with a scopes map — the\
  \ scopes below are searched\n  from the docs, not derived from a spec.\naccess_tiers:\n  - name: Standard Access\n    description: Default tier. Applies to data the app owns or manages. No App Review required for most permissions.\n  - name: Advanced Access\n    description: >-\n      Required to access data owned by other businesses/users. Requires App Review, Business Verification,\n      and (for permissions touching user data) an annual Data Use Checkup and, for advanced permissions, a\n      Data Protection Assessment.\npolicies:\n  - name: 90-day regrant\n    description: If an app does not use a permission for 90 days, the app user must grant it again.\n  - name: Granular consent\n    description: App users may grant or deny any subset of the permissions an app requests.\n  - name: Least privilege\n    description: >-\n      Meta names over-requesting as a common cause of App Review rejection (\"Only select permissions that\n      your app needs to function as intended\").\nmcp_scopes:\n\
  \  - server: https://mcp.facebook.com/ads\n    source: https://mcp.facebook.com/.well-known/oauth-protected-resource/ads\n    method: probed\n    scopes:\n      - ads_management\n      - ads_read\n      - catalog_management\n      - business_management\n      - pages_show_list\n      - instagram_basic\n      - ads_mcp_management\n  - server: https://mcp.facebook.com/devtools\n    source: https://mcp.facebook.com/.well-known/oauth-protected-resource/devtools\n    method: probed\n    scopes:\n      - developer_tools_mcp_app_read\n      - developer_tools_mcp_app_management\nscopes:\n  - name: public_profile\n    group: default\n    description: Default permission granted with every Facebook Login. Basic profile fields.\n  - name: email\n    group: default\n    description: The app user's primary email address.\n  - name: ads_management\n    group: ads\n    description: >-\n      Read and manage the ad accounts the app owns or has been granted access to. Programmatically create\n      campaigns,\
  \ manage ads, fetch ad metrics. Dependencies: pages_read_engagement, pages_show_list.\n  - name: ads_read\n    group: ads\n    description: Read-only access to ads performance data for owned or granted ad accounts.\n  - name: ads_mcp_management\n    group: ads\n    description: >-\n      Access the Meta ads Model Context Protocol (MCP) server and enable AI agents to interact with Meta Ads\n      on behalf of advertisers — create and manage campaigns, retrieve insights and reporting, and manage\n      business assets like catalogs, ad accounts and pixels.\n  - name: attribution_read\n    group: ads\n    description: Read Meta attribution and measurement data.\n  - name: read_insights\n    group: insights\n    description: Read Insights data for Pages, apps and web domains the app user owns.\n  - name: read_audience_network_insights\n    group: insights\n    description: Read Audience Network insights for apps the app user administers.\n  - name: business_management\n    group: business\n\
  \    description: Read and write Business Manager assets, users and asset assignments.\n  - name: catalog_management\n    group: commerce\n    description: Create, read, update and delete product catalogs owned by a business.\n  - name: commerce_manage_accounts\n    group: commerce\n    description: Manage commerce accounts for a business.\n  - name: commerce_account_manage_orders\n    group: commerce\n    description: Manage orders on a commerce account.\n  - name: commerce_account_read_orders\n    group: commerce\n    description: Read orders on a commerce account.\n  - name: commerce_account_read_reports\n    group: commerce\n    description: Read commerce account reports.\n  - name: commerce_account_read_settings\n    group: commerce\n    description: Read commerce account settings.\n  - name: leads_retrieval\n    group: ads\n    description: Download lead data generated by Lead Ads forms on Pages the app user manages.\n  - name: pages_show_list\n    group: pages\n    description:\
  \ List the Pages the app user manages.\n  - name: pages_read_engagement\n    group: pages\n    description: Read content, engagement and metadata on Pages the app user manages.\n  - name: pages_read_user_content\n    group: pages\n    description: Read user-generated content (posts, comments, ratings) on managed Pages.\n  - name: pages_manage_posts\n    group: pages\n    description: Create, edit and delete posts on managed Pages.\n  - name: pages_manage_engagement\n    group: pages\n    description: Create, edit and delete comments and likes on managed Pages.\n  - name: pages_manage_metadata\n    group: pages\n    description: Manage Page settings and subscribe/unsubscribe apps to Page webhooks.\n  - name: pages_manage_ads\n    group: pages\n    description: Manage ads associated with a Page.\n  - name: pages_manage_cta\n    group: pages\n    description: Manage the call-to-action button on a Page.\n  - name: pages_manage_instant_articles\n    group: pages\n    description: Manage Instant\
  \ Articles on behalf of Pages the app user administers.\n  - name: pages_messaging\n    group: messaging\n    description: Send and receive messages through a Page (Messenger Platform).\n  - name: pages_utility_messaging\n    group: messaging\n    description: Send utility (non-promotional) messages through a Page.\n  - name: pages_events\n    group: pages\n    description: Log Page events for advertising and analytics.\n  - name: pages_user_gender\n    group: pages\n    description: Read the gender of a user interacting with a managed Page.\n  - name: pages_user_locale\n    group: pages\n    description: Read the locale of a user interacting with a managed Page.\n  - name: pages_user_timezone\n    group: pages\n    description: Read the time zone of a user interacting with a managed Page.\n  - name: publish_video\n    group: media\n    description: Publish live and on-demand video to a Page, group or user.\n  - name: instagram_basic\n    group: instagram\n    description: Read basic metadata\
  \ and media for an Instagram Business or Creator account.\n  - name: instagram_business_basic\n    group: instagram\n    description: Basic access under Business Login for Instagram.\n  - name: instagram_content_publish\n    group: instagram\n    description: Publish content to an Instagram Business account.\n  - name: instagram_business_content_publish\n    group: instagram\n    description: Publish content under Business Login for Instagram.\n  - name: instagram_manage_comments\n    group: instagram\n    description: Read and manage comments on Instagram media.\n  - name: instagram_business_manage_comments\n    group: instagram\n    description: Manage comments under Business Login for Instagram.\n  - name: instagram_manage_insights\n    group: instagram\n    description: Read insights for an Instagram Business account and its media.\n  - name: instagram_manage_messages\n    group: instagram\n    description: Send and receive Instagram Direct messages.\n  - name: instagram_business_manage_messages\n\
  \    group: instagram\n    description: Messaging under Business Login for Instagram.\n  - name: instagram_manage_events\n    group: instagram\n    description: Log events for an Instagram Business account.\n  - name: instagram_manage_upcoming_events\n    group: instagram\n    description: Manage upcoming events on an Instagram Business account.\n  - name: instagram_manage_contents\n    group: instagram\n    description: Manage content on an Instagram Business account.\n  - name: instagram_manage_engagement\n    group: instagram\n    description: Manage engagement on an Instagram Business account.\n  - name: instagram_shopping_tag_products\n    group: instagram\n    description: Tag products from a catalog in Instagram media.\n  - name: instagram_branded_content_brand\n    group: instagram\n    description: Branded content access on the brand side.\n  - name: instagram_branded_content_ads_brand\n    group: instagram\n    description: Run partnership ads against creator branded content.\n\
  \  - name: instagram_branded_content_creator\n    group: instagram\n    description: Branded content access on the creator side.\n  - name: instagram_creator_marketplace_discovery\n    group: instagram\n    description: Discover creators in the Instagram Creator Marketplace.\n  - name: instagram_creator_marketplace_messaging\n    group: instagram\n    description: Message creators in the Instagram Creator Marketplace.\n  - name: whatsapp_business_management\n    group: whatsapp\n    description: Manage WhatsApp Business Accounts, phone numbers, templates and settings.\n  - name: whatsapp_business_messaging\n    group: whatsapp\n    description: Send and receive messages through the WhatsApp Business Platform Cloud API.\n  - name: whatsapp_business_manage_events\n    group: whatsapp\n    description: Log WhatsApp business events.\n  - name: threads_basic\n    group: threads\n    description: Read basic profile and media data for a Threads account.\n  - name: threads_business_basic\n   \
  \ group: threads\n    description: Basic access for Threads business accounts.\n  - name: threads_content_publish\n    group: threads\n    description: Publish posts to Threads.\n  - name: threads_delete\n    group: threads\n    description: Delete Threads posts.\n  - name: threads_read_replies\n    group: threads\n    description: Read replies to Threads posts.\n  - name: threads_manage_replies\n    group: threads\n    description: Hide, unhide and reply to Threads replies.\n  - name: threads_manage_mentions\n    group: threads\n    description: Read and respond to Threads mentions.\n  - name: threads_manage_insights\n    group: threads\n    description: Read Threads media and account insights.\n  - name: threads_keyword_search\n    group: threads\n    description: Search Threads by keyword.\n  - name: threads_location_tagging\n    group: threads\n    description: Tag locations on Threads posts.\n  - name: threads_profile_discovery\n    group: threads\n    description: Discover public\
  \ Threads profiles.\n  - name: threads_share_to_instagram\n    group: threads\n    description: Share Threads content to Instagram.\n  - name: threads_user_id\n    group: threads\n    description: Access the Threads user id.\n  - name: manage_app_solutions\n    group: apps\n    description: Manage app solutions on behalf of a business.\n  - name: manage_fundraisers\n    group: social\n    description: Create and manage fundraisers on behalf of the app user.\n  - name: user_age_range\n    group: user\n    description: The app user's age range bucket.\n  - name: user_birthday\n    group: user\n    description: The app user's birthday.\n  - name: user_friends\n    group: user\n    description: The app user's friends who also use the app.\n  - name: user_gender\n    group: user\n    description: The app user's gender.\n  - name: user_hometown\n    group: user\n    description: The app user's hometown.\n  - name: user_likes\n    group: user\n    description: Pages the app user has liked.\n\
  \  - name: user_link\n    group: user\n    description: The URL of the app user's Facebook profile.\n  - name: user_location\n    group: user\n    description: The app user's current city.\n  - name: user_messenger_contact\n    group: user\n    description: Contact the app user on Messenger following a defined interaction.\n  - name: user_photos\n    group: user\n    description: Photos the app user has uploaded or is tagged in.\n  - name: user_posts\n    group: user\n    description: Posts on the app user's timeline.\n  - name: user_videos\n    group: user\n    description: Videos the app user has uploaded or is tagged in.\n  - name: gaming_profile\n    group: gaming\n    description: Gaming-scoped profile access.\n  - name: gaming_user_locale\n    group: gaming\n    description: Gaming-scoped locale access.\n  - name: developer_tools_mcp_app_read\n    group: mcp\n    description: >-\n      Read access for the Meta Devtools MCP server. Sourced from\n      https://mcp.facebook.com/.well-known/oauth-protected-resource/devtools,\
  \ not from the Permissions\n      Reference page.\n  - name: developer_tools_mcp_app_management\n    group: mcp\n    description: >-\n      Management access for the Meta Devtools MCP server. Sourced from\n      https://mcp.facebook.com/.well-known/oauth-protected-resource/devtools.\nscope_count: 82\ncompleteness_note: >-\n  Meta's Permissions Reference is paginated A-Z in a partly client-rendered layout. The list above is what\n  was legible in the served markup on 2026-08-13 plus the two MCP servers' machine-readable scope arrays.\n  It is a large and representative sample, not a guaranteed exhaustive enumeration; treat\n  https://developers.facebook.com/docs/permissions as canonical.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/scopes/facebook-business-manager-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Advertising
- Analytics
- Business Management
- Marketing
- Social Media
- Messaging
- Commerce
- Agents
- MCP
- Webhooks
token_urls: []
---
