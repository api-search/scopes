---
api_specs:
- filename: blackbird-flynet-openapi-original.yml
  format: yaml
  label: Flynet API
  slug: flynet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-flynet-openapi-original.yml
authorization_urls: []
description: 'OAuth 2.0 scopes for the Flynet API. Flynet''s OAuth implementation follows the Token-Mediating Backend variant of OAuth 2.0 + PKCE (S256). Member routes are gated per-scope: a valid bearer that lacks the scope a route requires returns HTTP 403 insufficient_scope (in the WWW-Authenticate header for member routes, a JSON body for API-key Discovery routes). Scope names are exact-match; a token is granted exactly the scopes it requests. The scope-to-operation map below is derived from the per-operation 403 response descriptions in the OpenAPI and enriched from the docs OAuth reference. The spec models the bearer as an http/JWT scheme (oauthBearer), so this scope surface is documented rather than declared as an OpenAPI oauth2 flow object.'
docs: https://docs.flynet.org/concepts/oauth
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Blackbird Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Blackbird publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Blackbird API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blackbird
provider_slug: blackbird
schemes: []
scope_count: 9
scope_names:
- read:profile
- read:wallets
- read:user_checkins
- read:checkins
- read:balance
- read:app
- read:restaurant_challenges
- read:restaurant_specials
- write:rewards
scopes:
- description: Read the authenticated member's profile and status.
  flows: []
  scope: read:profile
- description: Read the authenticated member's wallets (MEMBERSHIP and SPENDING).
  flows: []
  scope: read:wallets
- description: Read the authenticated member's own check-in history.
  flows: []
  scope: read:user_checkins
- description: Read the anonymized venue check-in feed (also minted on API keys for the /check_ins feed).
  flows: []
  scope: read:checkins
- description: Read the calling app's FLY wallet balance.
  flows: []
  scope: read:balance
- description: Read the calling app (DeveloperApp) context.
  flows: []
  scope: read:app
- description: List restaurant challenges.
  flows: []
  scope: read:restaurant_challenges
- description: List restaurant specials.
  flows: []
  scope: read:restaurant_specials
- description: Issue a FLY reward to a user.
  flows: []
  scope: write:rewards
slug: blackbird-scopes
source_filename: blackbird-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/blackbird-flynet-openapi-original.yml\ndocs: https://docs.flynet.org/concepts/oauth\ndescription: >-\n  OAuth 2.0 scopes for the Flynet API. Flynet's OAuth implementation follows the\n  Token-Mediating Backend variant of OAuth 2.0 + PKCE (S256). Member routes are\n  gated per-scope: a valid bearer that lacks the scope a route requires returns\n  HTTP 403 insufficient_scope (in the WWW-Authenticate header for member routes,\n  a JSON body for API-key Discovery routes). Scope names are exact-match; a token\n  is granted exactly the scopes it requests. The scope-to-operation map below is\n  derived from the per-operation 403 response descriptions in the OpenAPI and\n  enriched from the docs OAuth reference. The spec models the bearer as an\n  http/JWT scheme (oauthBearer), so this scope surface is documented rather than\n  declared as an OpenAPI oauth2 flow object.\noauth:\n  variant: OAuth 2.0 + PKCE (Token-Mediating\
  \ Backend)\n  authorize_url: https://api.blackbird.xyz/oauth/authorize\n  token_url: https://api.blackbird.xyz/oauth/token\n  authorize_url_staging: https://api.staging.blackbird.xyz/oauth/authorize\n  token_url_staging: https://api.staging.blackbird.xyz/oauth/token\n  consent_host: https://passport.flynet.org\n  pkce_required: true\n  code_challenge_method: S256\n  access_token_ttl: 60 minutes\n  refresh_token_ttl: up to 30 days, rotated on each use\nscopes:\n  - scope: read:profile\n    description: Read the authenticated member's profile and status.\n    operations: [getMe, getMyStatus]\n  - scope: read:wallets\n    description: Read the authenticated member's wallets (MEMBERSHIP and SPENDING).\n    operations: [listMyWallets]\n  - scope: read:user_checkins\n    description: Read the authenticated member's own check-in history.\n    operations: [listMyCheckIns]\n  - scope: read:checkins\n    description: Read the anonymized venue check-in feed (also minted on API keys for the /check_ins\
  \ feed).\n    operations: [getCheckIn, listCheckIns]\n  - scope: read:balance\n    description: Read the calling app's FLY wallet balance.\n    operations: [getBalance]\n  - scope: read:app\n    description: Read the calling app (DeveloperApp) context.\n    operations: [getApp]\n  - scope: read:restaurant_challenges\n    description: List restaurant challenges.\n    operations: [listChallenges]\n  - scope: read:restaurant_specials\n    description: List restaurant specials.\n    operations: [listSpecials]\n  - scope: write:rewards\n    description: Issue a FLY reward to a user.\n    operations: [issueReward]\nnotes: >-\n  Payment Intent routes require an OAuth access token (API keys are not accepted)\n  but are not gated by a payments-specific scope in the published spec; access is\n  gated by partner approval and the flynet_merchant_id credential instead. On a\n  member's first successful OAuth completion two wallets are minted automatically\n  (MEMBERSHIP + SPENDING).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/scopes/blackbird-scopes.yml
summary_line: 9 scopes
tags:
- Company
- Restaurants
- Loyalty
- Payments
- Dining
- Membership
- Crypto
- Blockchain
- Web3
token_urls: []
---
