---
api_specs:
- filename: revcontent-access-api-openapi.yml
  format: yaml
  label: RevContent Access API
  slug: revcontent-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-access-api-openapi.yml
- filename: revcontent-boosts-api-openapi.yml
  format: yaml
  label: RevContent Campaigns (Boosts) API
  slug: revcontent-boosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-boosts-api-openapi.yml
- filename: revcontent-ccpa-api-openapi.yml
  format: yaml
  label: RevContent CCPA API
  slug: revcontent-ccpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-ccpa-api-openapi.yml
- filename: revcontent-content-api-openapi.yml
  format: yaml
  label: RevContent Content API
  slug: revcontent-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-content-api-openapi.yml
- filename: revcontent-conversions-api-openapi.yml
  format: yaml
  label: RevContent Conversions API
  slug: revcontent-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-conversions-api-openapi.yml
- filename: revcontent-helpers-api-openapi.yml
  format: yaml
  label: RevContent Helpers API
  slug: revcontent-helpers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-helpers-api-openapi.yml
- filename: revcontent-sub-accounts-api-openapi.yml
  format: yaml
  label: RevContent Sub Accounts API
  slug: revcontent-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-sub-accounts-api-openapi.yml
- filename: revcontent-targeting-api-openapi.yml
  format: yaml
  label: RevContent Targeting API
  slug: revcontent-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-targeting-api-openapi.yml
- filename: revcontent-widgets-api-openapi.yml
  format: yaml
  label: RevContent Widgets API
  slug: revcontent-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widgets-api-openapi.yml
- filename: revcontent-widget-internal-content-api-openapi.yml
  format: yaml
  label: RevContent Widget Internal Content API
  slug: revcontent-widget-internal-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widget-internal-content-api-openapi.yml
- filename: revcontent-widget-optimizer-api-openapi.yml
  format: yaml
  label: RevContent Widget Optimizer API
  slug: revcontent-widget-optimizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widget-optimizer-api-openapi.yml
authorization_urls: []
description: 'RevContent''s OAuth 2.0 client-credentials token carries scopes, but they are NOT requestable and RevContent publishes no scopes reference page. The evidence is the token response the provider itself documents — `"scope": "advertiser publisher"` — cross-referenced against the per-operation `permission` marker on all 43 operations in the same contract. Two role scopes exist; a caller cannot narrow to one.'
docs: https://help.revcontent.com/knowledge/publisher-advertiser-api-requests
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Revcontent Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RevContent publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the RevContent API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RevContent
provider_slug: revcontent
schemes:
- evidence: 'Documented token response: {"access_token": "…", "expires_in": 86400, "token_type": "Bearer", "scope": "advertiser publisher"}. The token request accepts only grant_type, client_id and client_secret — there is no scope parameter to send.'
  flow: clientCredentials
  name: BearerAuth
  scope_parameter_supported: false
  source: https://api.revcontent.io/docs/stats/api_data.json#GetOauthAccess
  tokenUrl: https://api.revcontent.io/oauth/token
  type: oauth2
scope_count: 2
scope_names:
- advertiser
- publisher
scopes:
- description: The buy side. Campaigns (boosts), creative content, conversion pixels, widget targeting, widget blacklisting, and every Helpers reference lookup used to build a targeting request.
  flows:
  - clientCredentials
  scope: advertiser
- description: The sell side. Widget inventory, geo and Sub ID reporting, and publisher-owned internal content inside a widget.
  flows:
  - clientCredentials
  scope: publisher
slug: revcontent-scopes
source_filename: revcontent-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api.revcontent.io/docs/stats/api_data.json\ndocs: https://help.revcontent.com/knowledge/publisher-advertiser-api-requests\ndescription: >-\n  RevContent's OAuth 2.0 client-credentials token carries scopes, but they are NOT requestable and\n  RevContent publishes no scopes reference page. The evidence is the token response the provider\n  itself documents — `\"scope\": \"advertiser publisher\"` — cross-referenced against the per-operation\n  `permission` marker on all 43 operations in the same contract. Two role scopes exist; a caller\n  cannot narrow to one.\n\nschemes:\n  - name: BearerAuth\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://api.revcontent.io/oauth/token\n    scope_parameter_supported: false\n    source: https://api.revcontent.io/docs/stats/api_data.json#GetOauthAccess\n    evidence: >-\n      Documented token response: {\"access_token\": \"…\", \"expires_in\": 86400, \"token_type\"\
  : \"Bearer\",\n      \"scope\": \"advertiser publisher\"}. The token request accepts only grant_type, client_id and\n      client_secret — there is no scope parameter to send.\n\nscopes:\n  - scope: advertiser\n    description: >-\n      The buy side. Campaigns (boosts), creative content, conversion pixels, widget targeting,\n      widget blacklisting, and every Helpers reference lookup used to build a targeting request.\n    flows: [clientCredentials]\n    operation_count: 28\n    operations:\n      - getAllBoosts\n      - getBoostPerformance\n      - getWidgetStats\n      - postBoostAdd\n      - postBoostArchive\n      - postBoostSettings\n      - postBoostsStatus\n      - getAllBoostContent\n      - getBoostContent\n      - getContentWidgetStats\n      - postBoostContentAdd\n      - postBoostContentUpdate\n      - getConversions\n      - postConversionAdd\n      - postConversionDelete\n      - postConversionEdit\n      - getBrowsers\n      - getCountries\n      - getDevices\n      -\
  \ getDmas\n      - getLanguages\n      - getOperatingSystems\n      - getRegions\n      - getBoostWidgets\n      - postBoostWidgets\n      - getTargetsOptimizerWidgets\n      - postTargetsWidgetsOptimizerAdd\n      - postTargetsWidgetsOptimizerRemove\n  - scope: publisher\n    description: >-\n      The sell side. Widget inventory, geo and Sub ID reporting, and publisher-owned internal\n      content inside a widget.\n    flows: [clientCredentials]\n    operation_count: 6\n    operations:\n      - getAllWidgets\n      - getAllWidgetsGeo\n      - getSubIDStats\n      - getWidgetInternalContent\n      - postWidgetInternalContentAdd\n      - postWidgetInternalContentUpdate\n\nshared_operations:\n  description: Operations the contract marks as available to both roles.\n  advertiser_and_publisher:\n    - getOauthAccess\n    - getReactivateAccount\n    - addAccount\n    - editAccount\n    - listAccounts\n    - updateAccountStatus\n  unscoped:\n    description: >-\n      The three CCPA operations\
  \ declare no permission at all. postSubmitCCPARequest is documented\n      without a bearer token — it is issued from the consumer's browser with a `Cookie: __ID=…`\n      header — which makes it the one genuinely unauthenticated write in the API.\n    operations:\n      - postSubmitCCPARequest\n      - postUserData\n      - postUsersData\n\ngaps:\n  - No scopes or permissions reference page exists on revcontent.com or help.revcontent.com. The\n    scope values are only discoverable by reading the token response example inside the generated\n    API reference.\n  - Scopes cannot be narrowed. A credential entitled to both roles always receives both, so\n    least-privilege is not achievable through this API.\n  - >-\n    Sub-account access is not scoped at all. sub_account_id is a request parameter, so one token\n    reaches every child account of the parent.\n  - No /.well-known/oauth-authorization-server document (404), so neither the token endpoint nor the\n    supported scopes are programmatically\
  \ discoverable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/scopes/revcontent-scopes.yml
summary_line: 2 scopes
tags:
- Native Advertising
- Content Recommendation
- Ad Network
- Publisher Monetization
- Programmatic Advertising
- Advertising Technology
- Campaign Management
- Audience Targeting
- Conversion Tracking
- Marketing
token_urls: []
---
