---
api_specs:
- filename: hubris-pw-audio-api-openapi.yml
  format: yaml
  label: Hubris Audio API
  slug: hubris-pw-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-audio-api-openapi.yml
- filename: hubris-pw-decisions-api-openapi.yml
  format: yaml
  label: Hubris Decisions API
  slug: hubris-pw-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-decisions-api-openapi.yml
- filename: hubris-pw-embeddings-api-openapi.yml
  format: yaml
  label: Hubris Embeddings API
  slug: hubris-pw-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-embeddings-api-openapi.yml
- filename: hubris-pw-images-api-openapi.yml
  format: yaml
  label: Hubris Images API
  slug: hubris-pw-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-images-api-openapi.yml
- filename: hubris-pw-integrations-api-openapi.yml
  format: yaml
  label: Hubris Integrations API
  slug: hubris-pw-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-integrations-api-openapi.yml
- filename: hubris-pw-management-api-openapi.yml
  format: yaml
  label: Hubris Management API
  slug: hubris-pw-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-management-api-openapi.yml
- filename: hubris-pw-messages-api-openapi.yml
  format: yaml
  label: Hubris Messages API
  slug: hubris-pw-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-messages-api-openapi.yml
- filename: hubris-pw-metrics-api-openapi.yml
  format: yaml
  label: Hubris Metrics API
  slug: hubris-pw-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-metrics-api-openapi.yml
- filename: hubris-pw-models-api-openapi.yml
  format: yaml
  label: Hubris Models API
  slug: hubris-pw-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-models-api-openapi.yml
- filename: hubris-pw-rerank-api-openapi.yml
  format: yaml
  label: Hubris Rerank API
  slug: hubris-pw-rerank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-rerank-api-openapi.yml
- filename: hubris-pw-responses-api-openapi.yml
  format: yaml
  label: Hubris Responses API
  slug: hubris-pw-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-responses-api-openapi.yml
- filename: hubris-pw-usage-api-openapi.yml
  format: yaml
  label: Hubris Usage API
  slug: hubris-pw-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-usage-api-openapi.yml
- filename: hubris-pw-videos-api-openapi.yml
  format: yaml
  label: Hubris Videos API
  slug: hubris-pw-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-videos-api-openapi.yml
- filename: hubris-pw-chat-completions-api-openapi.yml
  format: yaml
  label: Hubris Chat Completions API
  slug: hubris-pw-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-chat-completions-api-openapi.yml
authorization_urls:
- https://api.hubris.pw/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Hubris Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hubris publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hubris API on a user''s behalf.


  Tokens are issued from https://api.hubris.pw/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hubris
provider_slug: hubris-pw
schemes:
- description: 'OAuth-токен приложения с ограниченными правами. Регистрация клиента — `POST /oauth/clients` (RFC 7591), PKCE S256 обязателен. Метаданные: `/.well-known/oauth-authorization-server`, `/.well-known/oauth-protected-resource`.'
  flows:
  - authorizationUrl: https://api.hubris.pw/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.hubris.pw/oauth/token
  name: oauth2
  source: openapi/hubris-pw-openapi.json
scope_count: 6
scope_names:
- balance:read
- chat:write
- models:read
- offline_access
- videos:read
- videos:write
scopes:
- description: Видеть остаток баланса пользователя.
  flows:
  - authorizationCode
  scope: balance:read
- description: 'Запросы к моделям от имени пользователя (списывают баланс): чат, Responses, Messages, эмбеддинги, реранкеры, модели решений, изображения, распознавание и озвучка речи, расшифровка видео; коннекторы Битрикс24.'
  flows:
  - authorizationCode
  scope: chat:write
- description: Видеть цепочки резервных моделей пользователя в `GET /v1/models`.
  flows:
  - authorizationCode
  scope: models:read
- description: Выдать refresh-токен, чтобы подключение жило 90 дней без повторного входа.
  flows:
  - authorizationCode
  scope: offline_access
- description: Узнавать статус и скачивать видео пользователя (`GET /v1/videos/{id}`, `GET /v1/videos/{id}/content`).
  flows:
  - authorizationCode
  scope: videos:read
- description: Создавать видео от имени пользователя (`POST /v1/videos`, резервирует и списывает баланс).
  flows:
  - authorizationCode
  scope: videos:write
slug: hubris-pw-scopes
source_filename: hubris-pw-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hubris-pw-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/hubris-pw-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.hubris.pw/oauth/authorize\n    tokenUrl: https://api.hubris.pw/oauth/token\n  description: 'OAuth-токен приложения с ограниченными правами. Регистрация клиента — `POST\n    /oauth/clients` (RFC 7591), PKCE S256 обязателен. Метаданные: `/.well-known/oauth-authorization-server`,\n    `/.well-known/oauth-protected-resource`.'\nscopes:\n- scope: balance:read\n  description: Видеть остаток баланса пользователя.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubris-pw-openapi.json\n- scope: chat:write\n  description: 'Запросы к моделям от имени пользователя (списывают баланс): чат, Responses,\n    Messages, эмбеддинги, реранкеры, модели решений, изображения, распознавание и озвучка речи,\n    расшифровка видео; коннекторы Битрикс24.'\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/hubris-pw-openapi.json\n- scope: models:read\n  description: Видеть цепочки резервных моделей пользователя в `GET /v1/models`.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubris-pw-openapi.json\n- scope: offline_access\n  description: Выдать refresh-токен, чтобы подключение жило 90 дней без повторного входа.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubris-pw-openapi.json\n- scope: videos:read\n  description: Узнавать статус и скачивать видео пользователя (`GET /v1/videos/{id}`, `GET /v1/videos/{id}/content`).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubris-pw-openapi.json\n- scope: videos:write\n  description: Создавать видео от имени пользователя (`POST /v1/videos`, резервирует и списывает\n    баланс).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hubris-pw-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hubris-pw/scopes/hubris-pw-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Artificial Intelligence
- Gateways
- Models
- OpenAI-Compatible
- Russian
token_bound: false
token_urls:
- https://api.hubris.pw/oauth/token
---
