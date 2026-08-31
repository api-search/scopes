---
api_specs:
- filename: playable-campaigns-api-openapi.yml
  format: yaml
  label: Playable Campaigns API
  slug: playable-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-campaigns-api-openapi.yml
- filename: playable-media-api-openapi.yml
  format: yaml
  label: Playable Media API
  slug: playable-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-media-api-openapi.yml
- filename: playable-oauth-api-openapi.yml
  format: yaml
  label: Playable OAUTH API
  slug: playable-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-oauth-api-openapi.yml
- filename: playable-user-api-openapi.yml
  format: yaml
  label: Playable User API
  slug: playable-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-user-api-openapi.yml
authorization_urls: []
description: ''
docs: https://api.playable.com/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Playable Scopes
name_suffix: OAuth Scopes
note: 'All 37 scopes come from the OAuth2 clientCredentials flow declared in the provider OpenAPI. Playable publishes NO separate scopes/permissions reference page — the spec is the only source, and every scope description it carries is the placeholder string "Grant right to" with no object and no semantics (preserved verbatim as provider_description). The description field on each entry below is DERIVED by API Evangelist from the summary of the operation(s) that require that scope, and each entry lists those operations by METHOD + path because the spec declares no operationId. Nothing is invented: a scope with no operation gets a null description. Scope granularity itself is genuinely good — 37 scopes across list/view/modify/delete verbs — so publishing real scope descriptions would be a cheap, high-value fix for Playable.'
overview: 'Playable publishes 37 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Playable API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Playable
provider_slug: playable
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: clientCredentials
  source: openapi/playable-api-openapi.yml
scope_count: 37
scope_names:
- campaigns.activate
- campaigns.bulk-prizes-items.send-email
- campaigns.bulk-prizes.list
- campaigns.bulk-prizes.modify
- campaigns.bulk-prizes.view
- campaigns.clear-cache
- campaigns.copy
- campaigns.delete
- campaigns.email-log.list
- campaigns.email-log.view
- campaigns.game-data-statistics
- campaigns.game-settings.modify
- campaigns.game-settings.view
- campaigns.integrations.list
- campaigns.list
- campaigns.modify
- campaigns.pause
- campaigns.prizes.list
- campaigns.prizes.view
- campaigns.registrations.delete
- campaigns.registrations.list
- campaigns.registrations.view
- campaigns.resume
- campaigns.sections.form-fields.list
- campaigns.sections.form-fields.view
- campaigns.sections.list
- campaigns.sections.view
- campaigns.sms-log.list
- campaigns.sms-log.view
- campaigns.types.list
- campaigns.types.view
- campaigns.view
- campaigns.voucher.delete
- campaigns.voucher.list
- campaigns.voucher.view
- media.upload
- user.create-login-token
scopes:
- description: Activate Campaign
  flows:
  - clientCredentials
  scope: campaigns.activate
- description: Send email to winner
  flows:
  - clientCredentials
  scope: campaigns.bulk-prizes-items.send-email
- description: Campaign Bulk Prizes
  flows:
  - clientCredentials
  scope: campaigns.bulk-prizes.list
- description: Campaign Bulk Prize
  flows:
  - clientCredentials
  scope: campaigns.bulk-prizes.modify
- description: Get a single campaign bulk prize resource
  flows:
  - clientCredentials
  scope: campaigns.bulk-prizes.view
- description: Campaign Clear Cache
  flows:
  - clientCredentials
  scope: campaigns.clear-cache
- description: Campaign copy
  flows:
  - clientCredentials
  scope: campaigns.copy
- description: Delete Campaign
  flows:
  - clientCredentials
  scope: campaigns.delete
- description: Campaign email logs
  flows:
  - clientCredentials
  scope: campaigns.email-log.list
- description: Campaign email log
  flows:
  - clientCredentials
  scope: campaigns.email-log.view
- description: Campaign game data statistic
  flows:
  - clientCredentials
  scope: campaigns.game-data-statistics
- description: Update campaign game settings
  flows:
  - clientCredentials
  scope: campaigns.game-settings.modify
- description: View campaign game settings
  flows:
  - clientCredentials
  scope: campaigns.game-settings.view
- description: Campaign Integrations
  flows:
  - clientCredentials
  scope: campaigns.integrations.list
- description: Campaigns list
  flows:
  - clientCredentials
  scope: campaigns.list
- description: Update Campaign
  flows:
  - clientCredentials
  scope: campaigns.modify
- description: Pause Campaign
  flows:
  - clientCredentials
  scope: campaigns.pause
- description: Campaign prizes
  flows:
  - clientCredentials
  scope: campaigns.prizes.list
- description: Campaign prize
  flows:
  - clientCredentials
  scope: campaigns.prizes.view
- description: Delete campaign registration
  flows:
  - clientCredentials
  scope: campaigns.registrations.delete
- description: Campaign registrations
  flows:
  - clientCredentials
  scope: campaigns.registrations.list
- description: Campaign registration
  flows:
  - clientCredentials
  scope: campaigns.registrations.view
- description: Resume campaign
  flows:
  - clientCredentials
  scope: campaigns.resume
- description: Campaign Section Form Fields
  flows:
  - clientCredentials
  scope: campaigns.sections.form-fields.list
- description: Campaign Section Form Field
  flows:
  - clientCredentials
  scope: campaigns.sections.form-fields.view
- description: Campaign Sections
  flows:
  - clientCredentials
  scope: campaigns.sections.list
- description: Campaign Section
  flows:
  - clientCredentials
  scope: campaigns.sections.view
- description: Campaign sms logs
  flows:
  - clientCredentials
  scope: campaigns.sms-log.list
- description: Campaign sms log
  flows:
  - clientCredentials
  scope: campaigns.sms-log.view
- description: Campaign types
  flows:
  - clientCredentials
  scope: campaigns.types.list
- description: This API responds with a single campaign type resource.
  flows:
  - clientCredentials
  scope: campaigns.types.view
- description: Campaign Statistics Registrations; Campaign Statistics Sessions; Campaign statistics; Show a single campaign
  flows:
  - clientCredentials
  scope: campaigns.view
- description: Delete Campaign vouchers
  flows:
  - clientCredentials
  scope: campaigns.voucher.delete
- description: Campaign vouchers
  flows:
  - clientCredentials
  scope: campaigns.voucher.list
- description: Campaign voucher
  flows:
  - clientCredentials
  scope: campaigns.voucher.view
- description: Upload media
  flows:
  - clientCredentials
  scope: media.upload
- description: Create login user token
  flows:
  - clientCredentials
  scope: user.create-login-token
slug: playable-scopes
source_filename: playable-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/playable-api-openapi.yml\ndocs: https://api.playable.com/\nreference: https://help.playable.com/en/articles/10384051-developer\ngrant: client_credentials\nscope_count: 37\nnote: 'All 37 scopes come from the OAuth2 clientCredentials flow declared in the provider OpenAPI. Playable\n  publishes NO separate scopes/permissions reference page — the spec is the only source, and every scope\n  description it carries is the placeholder string \"Grant right to\" with no object and no semantics (preserved\n  verbatim as provider_description). The description field on each entry below is DERIVED by API Evangelist\n  from the summary of the operation(s) that require that scope, and each entry lists those operations\n  by METHOD + path because the spec declares no operationId. Nothing is invented: a scope with no operation\n  gets a null description. Scope granularity itself is genuinely good — 37 scopes across list/view/modify/delete\n\
  \  verbs — so publishing real scope descriptions would be a cheap, high-value fix for Playable.'\norphan_scopes: []\nschemes:\n- name: clientCredentials\n  source: openapi/playable-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\nscopes:\n- scope: campaigns.activate\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Activate Campaign\n  operations:\n  - POST /v1/campaign/{campaign}/activate\n  description_method: derived-from-operation-summary\n- scope: campaigns.bulk-prizes-items.send-email\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Send email to winner\n  operations:\n  - POST /v1/campaign/{campaign}/bulk-prize/{bulkPrize}/item/{bulkPrizeItem}/send/email\n  description_method: derived-from-operation-summary\n- scope: campaigns.bulk-prizes.list\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign Bulk Prizes\n  operations:\n  - GET /v1/campaign/{campaign}/bulk-prizes\n  description_method: derived-from-operation-summary\n- scope: campaigns.bulk-prizes.modify\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign Bulk Prize\n  operations:\n  - PATCH /v1/campaign/{campaign}/bulk-prize/{bulkPrize}\n  description_method: derived-from-operation-summary\n- scope: campaigns.bulk-prizes.view\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Get a single campaign bulk prize resource\n  operations:\n  - GET /v1/campaign/{campaign}/bulk-prize/{bulkPrize}\n  description_method: derived-from-operation-summary\n- scope: campaigns.clear-cache\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n\
  \  provider_description: Grant right to\n  description: Campaign Clear Cache\n  operations:\n  - POST /v1/campaign/{campaign}/clear-cache\n  description_method: derived-from-operation-summary\n- scope: campaigns.copy\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign copy\n  operations:\n  - POST /v1/campaign/copy/{campaign}\n  description_method: derived-from-operation-summary\n- scope: campaigns.delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Delete Campaign\n  operations:\n  - DELETE /v1/campaign/{campaign}\n  description_method: derived-from-operation-summary\n- scope: campaigns.email-log.list\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign email logs\n  operations:\n  - GET /v1/campaign/{campaign}/email-log\n\
  \  description_method: derived-from-operation-summary\n- scope: campaigns.email-log.view\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign email log\n  operations:\n  - GET /v1/campaign/{campaign}/email-log/{emailLog}\n  description_method: derived-from-operation-summary\n- scope: campaigns.game-data-statistics\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign game data statistic\n  operations:\n  - GET /v1/campaign/{campaign}/game-data-statistics\n  description_method: derived-from-operation-summary\n- scope: campaigns.game-settings.modify\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Update campaign game settings\n  operations:\n  - PATCH /v1/campaign/{campaign}/game-settings\n  description_method: derived-from-operation-summary\n\
  - scope: campaigns.game-settings.view\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: View campaign game settings\n  operations:\n  - GET /v1/campaign/{campaign}/game-settings\n  description_method: derived-from-operation-summary\n- scope: campaigns.integrations.list\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign Integrations\n  operations:\n  - GET /v1/campaign/{campaign}/integrations\n  description_method: derived-from-operation-summary\n- scope: campaigns.list\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaigns list\n  operations:\n  - GET /v1/campaigns\n  description_method: derived-from-operation-summary\n- scope: campaigns.modify\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n\
  \  provider_description: Grant right to\n  description: Update Campaign\n  operations:\n  - POST /v1/campaign/{campaign}\n  description_method: derived-from-operation-summary\n- scope: campaigns.pause\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Pause Campaign\n  operations:\n  - POST /v1/campaign/{campaign}/pause\n  description_method: derived-from-operation-summary\n- scope: campaigns.prizes.list\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign prizes\n  operations:\n  - GET /v1/campaign/{campaign}/prizes\n  description_method: derived-from-operation-summary\n- scope: campaigns.prizes.view\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign prize\n  operations:\n  - GET /v1/campaign/{campaign}/prize/{prize}\n\
  \  description_method: derived-from-operation-summary\n- scope: campaigns.registrations.delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Delete campaign registration\n  operations:\n  - DELETE /v1/campaign/{campaign}/registration/{registration}\n  description_method: derived-from-operation-summary\n- scope: campaigns.registrations.list\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign registrations\n  operations:\n  - GET /v1/campaign/{campaign}/registrations\n  description_method: derived-from-operation-summary\n- scope: campaigns.registrations.view\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign registration\n  operations:\n  - GET /v1/campaign/{campaign}/registration/{registration}\n  description_method:\
  \ derived-from-operation-summary\n- scope: campaigns.resume\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Resume campaign\n  operations:\n  - POST /v1/campaign/{campaign}/resume\n  description_method: derived-from-operation-summary\n- scope: campaigns.sections.form-fields.list\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign Section Form Fields\n  operations:\n  - GET /v1/campaign/{campaign}/section/{section}/form-fields\n  description_method: derived-from-operation-summary\n- scope: campaigns.sections.form-fields.view\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign Section Form Field\n  operations:\n  - GET /v1/campaign/{campaign}/section/{section}/form-field/{formField}\n  description_method: derived-from-operation-summary\n\
  - scope: campaigns.sections.list\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign Sections\n  operations:\n  - GET /v1/campaign/{campaign}/sections\n  description_method: derived-from-operation-summary\n- scope: campaigns.sections.view\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign Section\n  operations:\n  - GET /v1/campaign/{campaign}/section/{section}\n  description_method: derived-from-operation-summary\n- scope: campaigns.sms-log.list\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign sms logs\n  operations:\n  - GET /v1/campaign/{campaign}/sms-log\n  description_method: derived-from-operation-summary\n- scope: campaigns.sms-log.view\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n\
  \  provider_description: Grant right to\n  description: Campaign sms log\n  operations:\n  - GET /v1/campaign/{campaign}/sms-log/{smsLog}\n  description_method: derived-from-operation-summary\n- scope: campaigns.types.list\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign types\n  operations:\n  - GET /v1/campaign-types\n  description_method: derived-from-operation-summary\n- scope: campaigns.types.view\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: This API responds with a single campaign type resource.\n  operations:\n  - GET /v1/campaign-type/{campaignType}\n  description_method: derived-from-operation-summary\n- scope: campaigns.view\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign Statistics Registrations;\
  \ Campaign Statistics Sessions; Campaign statistics; Show\n    a single campaign\n  operations:\n  - GET /v1/campaign/{campaign}\n  - GET /v1/campaign/{campaign}/statistics\n  - GET /v1/campaign/{campaign}/statistics/sessions\n  - GET /v1/campaign/{campaign}/statistics/registrations\n  description_method: derived-from-operation-summary\n- scope: campaigns.voucher.delete\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Delete Campaign vouchers\n  operations:\n  - DELETE /v1/campaign/voucher\n  description_method: derived-from-operation-summary\n- scope: campaigns.voucher.list\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign vouchers\n  operations:\n  - GET /v1/campaign/{campaign}/vouchers\n  description_method: derived-from-operation-summary\n- scope: campaigns.voucher.view\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Campaign voucher\n  operations:\n  - GET /v1/campaign/{campaign}/voucher/{voucher}\n  description_method: derived-from-operation-summary\n- scope: media.upload\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Upload media\n  operations:\n  - POST /v1/media/upload\n  description_method: derived-from-operation-summary\n- scope: user.create-login-token\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/playable-api-openapi.yml\n  provider_description: Grant right to\n  description: Create login user token\n  operations:\n  - POST /v1/user/create-login-token\n  description_method: derived-from-operation-summary\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/scopes/playable-scopes.yml
summary_line: 37 scopes · clientCredentials
tags:
- Company
- marketing-gamification
- interactive-marketing
- Campaign Management
- Zero-Party Data
- Lead Generation
- Loyalty
- MarTech
- Webhook
- Authentication
token_urls:
- /oauth/token
---
