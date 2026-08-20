---
api_specs:
- filename: appsmax-rest-api-v1-access-api-openapi.yml
  format: yaml
  label: AppsMax Access API
  slug: appsmax-rest-api-v1-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-access-api-openapi.yml
- filename: appsmax-rest-api-v1-applications-api-openapi.yml
  format: yaml
  label: AppsMax Applications API
  slug: appsmax-rest-api-v1-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-applications-api-openapi.yml
- filename: appsmax-rest-api-v1-bots-api-openapi.yml
  format: yaml
  label: AppsMax Bots API
  slug: appsmax-rest-api-v1-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-bots-api-openapi.yml
- filename: appsmax-rest-api-v1-campaigns-api-openapi.yml
  format: yaml
  label: AppsMax Campaigns API
  slug: appsmax-rest-api-v1-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-campaigns-api-openapi.yml
- filename: appsmax-rest-api-v1-funnels-api-openapi.yml
  format: yaml
  label: AppsMax Funnels API
  slug: appsmax-rest-api-v1-funnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-funnels-api-openapi.yml
- filename: appsmax-rest-api-v1-interactive-menu-api-openapi.yml
  format: yaml
  label: AppsMax Interactive menu API
  slug: appsmax-rest-api-v1-interactive-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-interactive-menu-api-openapi.yml
- filename: appsmax-rest-api-v1-miniapps-api-openapi.yml
  format: yaml
  label: AppsMax Miniapps API
  slug: appsmax-rest-api-v1-miniapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-miniapps-api-openapi.yml
- filename: appsmax-rest-api-v1-organizations-api-openapi.yml
  format: yaml
  label: AppsMax Organizations API
  slug: appsmax-rest-api-v1-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-organizations-api-openapi.yml
- filename: appsmax-rest-api-v1-subscribers-api-openapi.yml
  format: yaml
  label: AppsMax Subscribers API
  slug: appsmax-rest-api-v1-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-subscribers-api-openapi.yml
authorization_urls: []
description: ''
docs: https://appsmax.ru/developers/#scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Appsmax Rest Api V1 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AppsMax publishes 12 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the AppsMax API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AppsMax
provider_slug: appsmax-rest-api-v1
schemes: []
scope_count: 12
scope_names:
- organizations:read
- bots:read
- connections:read
- miniapps:read
- funnels:read
- interactive_menu:read
- applications:read
- applications:write
- campaigns:read
- campaigns:write
- subscribers:read
- subscribers:write
scopes:
- description: Read the current organization.
  flows: []
  scope: organizations:read
- description: Read the bot list and individual bot records.
  flows: []
  scope: bots:read
- description: Read the state of a bot's channel connection.
  flows: []
  scope: connections:read
- description: Read mini apps.
  flows: []
  scope: miniapps:read
- description: Read funnels and scenarios.
  flows: []
  scope: funnels:read
- description: Read interactive menu items.
  flows: []
  scope: interactive_menu:read
- description: Read customer requests (applications).
  flows: []
  scope: applications:read
- description: Create customer requests and sync their tags.
  flows: []
  scope: applications:write
- description: Read campaigns.
  flows: []
  scope: campaigns:read
- description: Create campaigns and separately launch them.
  flows: []
  scope: campaigns:write
- description: Read subscribers.
  flows: []
  scope: subscribers:read
- description: Create or update subscribers.
  flows: []
  scope: subscribers:write
slug: appsmax-rest-api-v1-scopes
source_filename: appsmax-rest-api-v1-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://appsmax.ru/developers/#scopes\ndocs: https://appsmax.ru/developers/#scopes\nvocabulary_url: https://appsmax.ru/developers/#scopes\ncorroborated_by: openapi/appsmax-rest-api-v1-openapi-original.json  # per-operation x-required-scope\n\nmodel:\n  type: api-token scope strings\n  oauth2: false\n  note: >-\n    AppsMax does NOT run OAuth 2.0. Scopes are selected by a signed-in human when creating an\n    organization-owned API token in the AppsMax cabinet (Data -> Integrations -> API). There is\n    no authorization endpoint, no token endpoint and no dynamic client registration.\n  default_when_empty: >-\n    A token created with no scope list technically receives full access within its organization.\n    AppsMax explicitly discourages this for new integrations — select the minimum required scopes.\n  tenancy: Every token is confined to its own AppsMax organization.\n  visibility: 'The scopes granted to the current token\
  \ are readable at GET /me.'\n\nscopes:\n  - scope: organizations:read\n    description: Read the current organization.\n    description_ru: Читать текущую организацию.\n    operations: [listOrganizations]\n  - scope: bots:read\n    description: Read the bot list and individual bot records.\n    description_ru: Читать список и карточки ботов.\n    operations: [listBots, getBot]\n  - scope: connections:read\n    description: Read the state of a bot's channel connection.\n    description_ru: Читать состояние подключения бота к каналу.\n    operations: [listBotConnections]\n  - scope: miniapps:read\n    description: Read mini apps.\n    description_ru: Читать мини-приложения.\n    operations: [listMiniapps]\n  - scope: funnels:read\n    description: Read funnels and scenarios.\n    description_ru: Читать сценарии и воронки.\n    operations: [listFunnels]\n  - scope: interactive_menu:read\n    description: Read interactive menu items.\n    description_ru: Читать элементы интерактивного меню.\n\
  \    operations: [listInteractiveMenuItems]\n  - scope: applications:read\n    description: Read customer requests (applications).\n    description_ru: Читать заявки.\n    operations: [listApplications, getApplication]\n  - scope: applications:write\n    description: Create customer requests and sync their tags.\n    description_ru: Создавать заявки и синхронизировать их теги.\n    operations: [createApplication, syncApplicationTags]\n  - scope: campaigns:read\n    description: Read campaigns.\n    description_ru: Читать кампании.\n    operations: [listCampaigns, getCampaign]\n  - scope: campaigns:write\n    description: Create campaigns and separately launch them.\n    description_ru: Создавать и отдельно запускать кампании.\n    operations: [createCampaign, runCampaign]\n  - scope: subscribers:read\n    description: Read subscribers.\n    description_ru: Читать подписчиков.\n    operations: [listSubscribers, getSubscriber]\n  - scope: subscribers:write\n    description: Create or update\
  \ subscribers.\n    description_ru: Создавать или обновлять подписчиков.\n    operations: [upsertSubscriber, updateSubscriber]\n\nunscoped_operations:\n  - operationId: ping\n    note: Requires a valid token but no scope.\n  - operationId: getCurrentApiContext\n    note: Requires a valid token but no scope; returns the token's own scopes and rate limit.\n\nsummary:\n  scope_count: 12\n  read_scopes: 8\n  write_scopes: 4\n  operations_covered: 19\n  operations_unscoped: 2\n\nx-evidence:\n  fetched: '2026-08-09'\n  urls:\n    - url: https://appsmax.ru/developers/\n      http_status: 200\n    - url: https://appsmax.ru/.well-known/api-onboarding\n      http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/scopes/appsmax-rest-api-v1-scopes.yml
summary_line: 12 scopes
tags:
- Company
- Software-as-a-Service
- Messaging
- Business Automation
- Chatbots
- Mini Apps
- Customer Requests
- Workflow-Automation
- MAX
- Telegram
- Russian Language
token_urls: []
---
