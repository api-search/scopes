---
api_specs:
- filename: reddit-data-api-openapi.yml
  format: yaml
  label: Reddit Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-data-api-openapi.yml
- filename: reddit-ads-api-openapi.yml
  format: yaml
  label: Reddit Ads API
  slug: ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-ads-api-openapi.yml
- filename: reddit-embeds-openapi.yml
  format: yaml
  label: Reddit Embeds (oEmbed)
  slug: embeds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-embeds-openapi.yml
authorization_urls:
- https://www.reddit.com/api/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Reddit Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Reddit publishes 20 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Reddit API on a user''s behalf.


  Tokens are issued from https://www.reddit.com/api/v1/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Reddit
provider_slug: reddit
schemes:
- description: Reddit Ads API uses OAuth 2.0 for authentication. Access tokens are obtained via the authorization code flow.
  flows:
  - authorizationUrl: https://www.reddit.com/api/v1/authorize
    flow: authorizationCode
    tokenUrl: https://www.reddit.com/api/v1/access_token
  name: oauth2
  source: openapi/reddit-ads-api-openapi.yml
- description: Reddit uses OAuth 2.0 for authentication. All API requests must include a valid access token obtained through one of the supported OAuth grant types.
  flows:
  - authorizationUrl: https://www.reddit.com/api/v1/authorize
    flow: authorizationCode
    tokenUrl: https://www.reddit.com/api/v1/access_token
  name: oauth2
  source: openapi/reddit-data-api-openapi.yml
scope_count: 20
scope_names:
- ads
- edit
- flair
- history
- identity
- modconfig
- modflair
- modlog
- modposts
- modwiki
- mysubreddits
- privatemessages
- read
- report
- save
- submit
- subscribe
- vote
- wikiedit
- wikiread
scopes:
- description: Access to ads management endpoints
  flows:
  - authorizationCode
  scope: ads
- description: Edit and delete content
  flows:
  - authorizationCode
  scope: edit
- description: Set user and link flair
  flows:
  - authorizationCode
  scope: flair
- description: Access voting history
  flows:
  - authorizationCode
  scope: history
- description: Access user identity
  flows:
  - authorizationCode
  scope: identity
- description: Manage subreddit configuration
  flows:
  - authorizationCode
  scope: modconfig
- description: Manage subreddit flair
  flows:
  - authorizationCode
  scope: modflair
- description: Access moderation log
  flows:
  - authorizationCode
  scope: modlog
- description: Approve and remove content
  flows:
  - authorizationCode
  scope: modposts
- description: Manage wiki pages
  flows:
  - authorizationCode
  scope: modwiki
- description: Access subscribed subreddits
  flows:
  - authorizationCode
  scope: mysubreddits
- description: Access private messages
  flows:
  - authorizationCode
  scope: privatemessages
- description: Read content
  flows:
  - authorizationCode
  scope: read
- description: Report content
  flows:
  - authorizationCode
  scope: report
- description: Save and unsave content
  flows:
  - authorizationCode
  scope: save
- description: Submit content
  flows:
  - authorizationCode
  scope: submit
- description: Manage subscriptions
  flows:
  - authorizationCode
  scope: subscribe
- description: Vote on content
  flows:
  - authorizationCode
  scope: vote
- description: Edit wiki pages
  flows:
  - authorizationCode
  scope: wikiedit
- description: Read wiki pages
  flows:
  - authorizationCode
  scope: wikiread
slug: reddit-scopes
source_filename: reddit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reddit-ads-api-openapi.yml, openapi/reddit-data-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/reddit-ads-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.reddit.com/api/v1/authorize\n    tokenUrl: https://www.reddit.com/api/v1/access_token\n  description: Reddit Ads API uses OAuth 2.0 for authentication. Access tokens are obtained\n    via the authorization code flow.\n- name: oauth2\n  source: openapi/reddit-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.reddit.com/api/v1/authorize\n    tokenUrl: https://www.reddit.com/api/v1/access_token\n  description: Reddit uses OAuth 2.0 for authentication. All API requests must include a valid\n    access token obtained through one of the supported OAuth grant types.\nscopes:\n- scope: ads\n  description: Access to ads management endpoints\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/reddit-ads-api-openapi.yml\n- scope: edit\n  description: Edit and delete content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: flair\n  description: Set user and link flair\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: history\n  description: Access voting history\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: identity\n  description: Access user identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: modconfig\n  description: Manage subreddit configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: modflair\n  description: Manage subreddit flair\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: modlog\n  description: Access moderation log\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: modposts\n  description: Approve and remove content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: modwiki\n  description: Manage wiki pages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: mysubreddits\n  description: Access subscribed subreddits\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: privatemessages\n  description: Access private messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: read\n  description: Read content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: report\n  description: Report content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: save\n  description: Save and unsave content\n  flows:\n  - authorizationCode\n \
  \ sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: submit\n  description: Submit content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: subscribe\n  description: Manage subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: vote\n  description: Vote on content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: wikiedit\n  description: Edit wiki pages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n- scope: wikiread\n  description: Read wiki pages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/reddit-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/scopes/reddit-scopes.yml
summary_line: 20 scopes · authorizationCode
tags:
- Advertising
- Communities
- Content
- Social Media
- Social News
token_urls:
- https://www.reddit.com/api/v1/access_token
---
