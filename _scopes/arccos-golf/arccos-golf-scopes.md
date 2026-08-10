---
api_specs:
- filename: arccos-golf-clubs-api-openapi.yml
  format: yaml
  label: Arccos Golf Clubs API
  slug: arccos-golf-clubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-clubs-api-openapi.yml
- filename: arccos-golf-courses-api-openapi.yml
  format: yaml
  label: Arccos Golf Courses API
  slug: arccos-golf-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-courses-api-openapi.yml
- filename: arccos-golf-rounds-api-openapi.yml
  format: yaml
  label: Arccos Golf Rounds API
  slug: arccos-golf-rounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-rounds-api-openapi.yml
- filename: arccos-golf-users-api-openapi.yml
  format: yaml
  label: Arccos Golf Users API
  slug: arccos-golf-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-users-api-openapi.yml
- filename: arccos-golf-webhooks-api-openapi.yml
  format: yaml
  label: Arccos Golf Webhooks API
  slug: arccos-golf-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/openapi/arccos-golf-webhooks-api-openapi.yml
authorization_urls:
- https://signin.arccosgolf.com/login
description: ''
docs: https://api.arccosgolf.com/swagger
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Arccos Golf Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Arccos Golf publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Arccos Golf API on a user''s behalf.


  Tokens are issued from https://api.arccosgolf.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Arccos Golf
provider_slug: arccos-golf
schemes:
- flows:
  - authorizationUrl: https://signin.arccosgolf.com/login
    flow: authorizationCode
    tokenUrl: https://api.arccosgolf.com/oauth2/token
  name: AccessCodeAuth
  source: openapi/arccos-golf-on-course-data-api-openapi.yml
scope_count: 4
scope_names:
- openid
- arccos/read:users
- arccos/read:rounds
- arccos/read:clubs
scopes:
- description: Required for all endpoints that have userId in the path
  flows:
  - authorizationCode
  scope: openid
- description: Grants read users access
  flows:
  - authorizationCode
  scope: arccos/read:users
- description: Grants read rounds access
  flows:
  - authorizationCode
  scope: arccos/read:rounds
- description: Grants read clubs access
  flows:
  - authorizationCode
  scope: arccos/read:clubs
slug: arccos-golf-scopes
source_filename: arccos-golf-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: >-\n  https://api.arccosgolf.com/swagger.json — securityDefinitions.AccessCodeAuth.scopes plus the published\n  \"Scopes\" section of info.description\ndocs: https://api.arccosgolf.com/swagger\nmodel: >-\n  Scopes gate access to endpoints. A scope that was not requested in the initial authorization request cannot be\n  added retroactively — the user must re-authorize the client. Arccos controls which scopes a given client is\n  permitted to request at all. Every scope except openid is namespaced as `arccos/<operation>:<resource>`.\nschemes:\n- name: AccessCodeAuth\n  source: openapi/arccos-golf-on-course-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://signin.arccosgolf.com/login\n    tokenUrl: https://api.arccosgolf.com/oauth2/token\nscopes:\n- scope: openid\n  description: Required for all endpoints that have userId in the path\n  flows:\n  - authorizationCode\n  required_for:\n \
  \ - handle_get_one_user.get./v5/users/{userId}\n  - handle_search_rounds.get./v5/users/{userId}/rounds\n  - handle_get_one_round.get./v5/users/{userId}/rounds/{roundId}\n  - handle_get_round_stats.get./v5/users/{userId}/rounds/{roundId}/stats\n  - handle_search_clubs.get./v5/users/{userId}/clubs\n  - handle_get_one_club.get./v5/users/{userId}/clubs/{clubId}\n  note: >-\n    Also the scope that causes an id_token to be issued; its custom:arccosUserId claim is the {userId} path value.\n  sources:\n  - openapi/arccos-golf-on-course-data-api-openapi.yml\n  - https://api.arccosgolf.com/swagger.json\n- scope: arccos/read:users\n  description: Grants read users access\n  flows:\n  - authorizationCode\n  operations:\n  - handle_get_one_user.get./v5/users/{userId}\n  sources:\n  - openapi/arccos-golf-on-course-data-api-openapi.yml\n- scope: arccos/read:rounds\n  description: Grants read rounds access\n  flows:\n  - authorizationCode\n  operations:\n  - handle_search_rounds.get./v5/users/{userId}/rounds\n\
  \  - handle_get_one_round.get./v5/users/{userId}/rounds/{roundId}\n  - handle_get_round_stats.get./v5/users/{userId}/rounds/{roundId}/stats\n  sources:\n  - openapi/arccos-golf-on-course-data-api-openapi.yml\n- scope: arccos/read:clubs\n  description: Grants read clubs access\n  flows:\n  - authorizationCode\n  operations:\n  - handle_search_clubs.get./v5/users/{userId}/clubs\n  - handle_get_one_club.get./v5/users/{userId}/clubs/{clubId}\n  sources:\n  - openapi/arccos-golf-on-course-data-api-openapi.yml\nunscoped_operations:\n- operations:\n  - handle_search_courses.get./v5/courses\n  - handle_get_one_course.get./v5/courses/{courseId}\n  - handle_get_one_course_version.get./v5/courses/{courseId}/versions/{courseVersion}\n  note: Course-catalog reads declare no security requirement and were verified callable anonymously on 2026-08-06.\n- operations:\n  - handle_get_webhooks.get./v5/webhooks\n  - handle_create_webhook.post./v5/webhooks\n  - handle_delete_webhook.delete./v5/webhooks/{webhookId}\n\
  \  note: >-\n    Webhook registration uses HTTP Basic client credentials (BasicAuth), not the OAuth scope model — these are\n    client-level, not user-delegated, operations.\ngaps:\n- No write scopes are published; the delegated surface is read-only.\n- >-\n  There is no public scope-reference page separate from the Swagger UI; the scope list is only discoverable from\n  the spec's securityDefinitions and the \"Authorize\" dialog.\ncross_links:\n  authentication: authentication/arccos-golf-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arccos-golf/refs/heads/main/scopes/arccos-golf-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- golf
- sports-technology
- wearables
- iot
- shot-tracking
- sports-analytics
- performance-analytics
- geospatial
- consumer-hardware
- webhooks
- oauth2
- mcp
- ecommerce
token_urls:
- https://api.arccosgolf.com/oauth2/token
---
