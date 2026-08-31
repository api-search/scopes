---
api_specs:
- filename: instagram-comments-api-openapi.yml
  format: yaml
  label: Instagram Comments API
  slug: instagram-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-comments-api-openapi.yml
- filename: instagram-hashtags-api-openapi.yml
  format: yaml
  label: Instagram Hashtags API
  slug: instagram-hashtags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-hashtags-api-openapi.yml
- filename: instagram-insights-api-openapi.yml
  format: yaml
  label: Instagram Insights API
  slug: instagram-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-insights-api-openapi.yml
- filename: instagram-media-api-openapi.yml
  format: yaml
  label: Instagram Media API
  slug: instagram-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-media-api-openapi.yml
- filename: instagram-mentions-api-openapi.yml
  format: yaml
  label: Instagram Mentions API
  slug: instagram-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-mentions-api-openapi.yml
- filename: instagram-publishing-api-openapi.yml
  format: yaml
  label: Instagram Publishing API
  slug: instagram-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-publishing-api-openapi.yml
- filename: instagram-users-api-openapi.yml
  format: yaml
  label: Instagram Users API
  slug: instagram-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-users-api-openapi.yml
authorization_urls:
- https://www.facebook.com/dialog/oauth
- https://www.instagram.com/oauth/authorize
description: Meta calls these "permissions", not scopes, but they are requested as OAuth 2.0 scopes in the authorization request. Upgraded 2026-08-29 from a 7-scope derivation off the OpenAPI securitySchemes to the full published reference - 19 instagram_* permissions plus the Facebook Page permissions an Instagram-with-Facebook-Login app also needs. EVERY instagram_* permission requires App Review to be used against accounts the app does not own.
docs: https://developers.facebook.com/docs/permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Instagram Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Instagram publishes 19 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Instagram API on a user''s behalf.


  Tokens are issued from https://graph.facebook.com/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Instagram
provider_slug: instagram
schemes:
- description: OAuth 2.0 authorization code. Two parallel login models with two distinct permission families - picking the wrong family for the host is the most common integration failure on this platform.
  flows:
  - authorizationUrl: https://www.facebook.com/dialog/oauth
    base: https://graph.facebook.com
    flow: authorizationCode
    login_model: Instagram API with Facebook Login
    scope_family: instagram_*
    tokenUrl: https://graph.facebook.com/oauth/access_token
  - authorizationUrl: https://www.instagram.com/oauth/authorize
    base: https://graph.instagram.com
    flow: authorizationCode
    login_model: Instagram API with Instagram Login
    scope_family: instagram_business_*
    tokenUrl: https://api.instagram.com/oauth/access_token
  name: oauth2
  source:
  - openapi/
  - https://developers.facebook.com/docs/permissions
scope_count: 19
scope_names:
- instagram_basic
- instagram_content_publish
- instagram_manage_comments
- instagram_manage_insights
- instagram_manage_messages
- instagram_manage_contents
- instagram_manage_engagement
- instagram_manage_events
- instagram_manage_upcoming_events
- instagram_shopping_tag_products
- instagram_branded_content_ads_brand
- instagram_branded_content_brand
- instagram_branded_content_creator
- instagram_creator_marketplace_discovery
- instagram_creator_marketplace_messaging
- instagram_business_basic
- instagram_business_content_publish
- instagram_business_manage_comments
- instagram_business_manage_messages
scopes:
- description: Read an Instagram account profile's info and media.
  flows:
  - authorizationCode
  scope: instagram_basic
- description: Create organic feed photo and video posts on behalf of a business user.
  flows:
  - authorizationCode
  scope: instagram_content_publish
- description: Create, delete and hide comments on behalf of the Instagram account linked to a Page.
  flows:
  - authorizationCode
  scope: instagram_manage_comments
- description: Get access to insights for the Instagram account linked to a Facebook Page.
  flows:
  - authorizationCode
  scope: instagram_manage_insights
- description: Read and respond to Instagram Direct messages.
  flows:
  - authorizationCode
  scope: instagram_manage_messages
- description: Delete posts on behalf of an Instagram account linked to a Facebook Page.
  flows:
  - authorizationCode
  scope: instagram_manage_contents
- description: Publish or delete a Like on IG Media objects, Feed or Reels.
  flows:
  - authorizationCode
  scope: instagram_manage_engagement
- description: Log events on behalf of Instagram accounts.
  flows:
  - authorizationCode
  scope: instagram_manage_events
- description: Read, create and update upcoming events on behalf of Instagram accounts.
  flows:
  - authorizationCode
  scope: instagram_manage_upcoming_events
- description: Tag Instagram media with product tags and appeal product rejections.
  flows:
  - authorizationCode
  scope: instagram_shopping_tag_products
- description: Read Instagram posts where the app user's Instagram account is tagged as a paid partner.
  flows:
  - authorizationCode
  scope: instagram_branded_content_ads_brand
- description: Add, remove and view creators from a specific brand's approved creators list.
  flows:
  - authorizationCode
  scope: instagram_branded_content_brand
- description: Read and change the boost status of a creator's specific piece of content.
  flows:
  - authorizationCode
  scope: instagram_branded_content_creator
- description: Discover content creators on Instagram Creator Marketplace.
  flows:
  - authorizationCode
  scope: instagram_creator_marketplace_discovery
- description: Get a brand's partnership conversations and a creator's messaging ID.
  flows:
  - authorizationCode
  scope: instagram_creator_marketplace_messaging
- description: Read an Instagram Business account profile's info and media.
  flows:
  - authorizationCode
  scope: instagram_business_basic
- description: Create organic feed photo and video posts on behalf of a business user.
  flows:
  - authorizationCode
  scope: instagram_business_content_publish
- description: Create, update and delete comments on Instagram business accounts.
  flows:
  - authorizationCode
  scope: instagram_business_manage_comments
- description: Access messages on an Instagram professional account.
  flows:
  - authorizationCode
  scope: instagram_business_manage_messages
slug: instagram-scopes
source_filename: instagram-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://developers.facebook.com/docs/permissions\ndocs: https://developers.facebook.com/docs/permissions\ndescription: >-\n  Meta calls these \"permissions\", not scopes, but they are requested as OAuth 2.0 scopes in the\n  authorization request. Upgraded 2026-08-29 from a 7-scope derivation off the OpenAPI\n  securitySchemes to the full published reference - 19 instagram_* permissions plus the Facebook\n  Page permissions an Instagram-with-Facebook-Login app also needs. EVERY instagram_* permission\n  requires App Review to be used against accounts the app does not own.\nschemes:\n- name: oauth2\n  source:\n  - openapi/\n  - https://developers.facebook.com/docs/permissions\n  flows:\n  - flow: authorizationCode\n    login_model: Instagram API with Facebook Login\n    authorizationUrl: https://www.facebook.com/dialog/oauth\n    tokenUrl: https://graph.facebook.com/oauth/access_token\n    base: https://graph.facebook.com\n \
  \   scope_family: instagram_*\n  - flow: authorizationCode\n    login_model: Instagram API with Instagram Login\n    authorizationUrl: https://www.instagram.com/oauth/authorize\n    tokenUrl: https://api.instagram.com/oauth/access_token\n    base: https://graph.instagram.com\n    scope_family: instagram_business_*\n  description: >-\n    OAuth 2.0 authorization code. Two parallel login models with two distinct permission families -\n    picking the wrong family for the host is the most common integration failure on this platform.\naccess_levels:\n  standard: >-\n    Granted automatically on app creation. The permission may only be requested from users who hold\n    a role on the app (admin, developer, tester).\n  advanced: >-\n    Required to request the permission from any user. Needs App Review for the specific permission,\n    plus Business Verification.\n  source: https://developers.facebook.com/docs/graph-api/overview/access-levels\nscopes:\n- scope: instagram_basic\n  description:\
  \ Read an Instagram account profile's info and media.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_content_publish\n  description: Create organic feed photo and video posts on behalf of a business user.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_manage_comments\n  description: Create, delete and hide comments on behalf of the Instagram account linked to a Page.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_manage_insights\n  description: Get access to insights for the Instagram account linked to a Facebook Page.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_manage_messages\n  description: Read and respond to Instagram Direct messages.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_manage_contents\n  description: Delete posts on behalf of\
  \ an Instagram account linked to a Facebook Page.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n  note: This is the permission behind deleteMedia - the highest-consequence, irreversible operation in the catalog.\n- scope: instagram_manage_engagement\n  description: Publish or delete a Like on IG Media objects, Feed or Reels.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_manage_events\n  description: Log events on behalf of Instagram accounts.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_manage_upcoming_events\n  description: Read, create and update upcoming events on behalf of Instagram accounts.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_shopping_tag_products\n  description: Tag Instagram media with product tags and appeal product rejections.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n\
  - scope: instagram_branded_content_ads_brand\n  description: Read Instagram posts where the app user's Instagram account is tagged as a paid partner.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_branded_content_brand\n  description: Add, remove and view creators from a specific brand's approved creators list.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_branded_content_creator\n  description: Read and change the boost status of a creator's specific piece of content.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_creator_marketplace_discovery\n  description: Discover content creators on Instagram Creator Marketplace.\n  family: facebook-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_creator_marketplace_messaging\n  description: Get a brand's partnership conversations and a creator's messaging ID.\n  family: facebook-login\n\
  \  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_business_basic\n  description: Read an Instagram Business account profile's info and media.\n  family: instagram-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_business_content_publish\n  description: Create organic feed photo and video posts on behalf of a business user.\n  family: instagram-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_business_manage_comments\n  description: Create, update and delete comments on Instagram business accounts.\n  family: instagram-login\n  app_review: true\n  flows: [authorizationCode]\n- scope: instagram_business_manage_messages\n  description: Access messages on an Instagram professional account.\n  family: instagram-login\n  app_review: true\n  flows: [authorizationCode]\ncompanion_scopes:\n- scope: pages_show_list\n  description: List the Facebook Pages a user manages - needed to find the Page an Instagram account is linked\
  \ to.\n  family: facebook-login\n  required_for: Instagram API with Facebook Login\n- scope: pages_read_engagement\n  description: Read engagement data from Pages.\n  family: facebook-login\n  required_for: Instagram API with Facebook Login\n- scope: ads_management\n  description: Alternative to pages_read_engagement when Page access was granted through Business Manager.\n  family: facebook-login\n  required_for: IG Hashtag Search in some Business Manager configurations\n- scope: business_management\n  description: Alternative to pages_read_engagement when Page access was granted through Business Manager.\n  family: facebook-login\n  required_for: IG Hashtag Search in some Business Manager configurations\nfeatures:\n- name: Instagram Public Content Access\n  description: >-\n    A FEATURE, not a permission, and a separate App Review item. Required in addition to\n    instagram_basic for IG Hashtag Search.\n  applies_to:\n  - searchHashtag\n  - getHashtagTopMedia\n  - getHashtagRecentMedia\n\
  scope_count: 19\nobservations:\n- The two permission families are not interchangeable. instagram_business_* only works with\n  Instagram Login at graph.instagram.com; instagram_* only works with Facebook Login at\n  graph.facebook.com.\n- Hashtag search and business discovery are reachable ONLY through Facebook Login, and hashtag\n  search additionally needs the Instagram Public Content Access feature approved.\n- Every single instagram_* permission requires App Review. There is no read-only tier an app can\n  self-serve into for other people's accounts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/scopes/instagram-scopes.yml
summary_line: 19 scopes · authorizationCode
tags:
- Instagram
- Meta
- Photos
- Social-Media
- Videos
- Content Publishing
token_urls:
- https://graph.facebook.com/oauth/access_token
- https://api.instagram.com/oauth/access_token
---
