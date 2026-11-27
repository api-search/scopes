---
api_specs:
- filename: eztexting-com-blocks-api-openapi.yml
  format: yaml
  label: EZ Texting Blocks API
  slug: eztexting-com-blocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-blocks-api-openapi.yml
- filename: eztexting-com-contact-fields-api-openapi.yml
  format: yaml
  label: EZ Texting Contact Fields API
  slug: eztexting-com-contact-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-contact-fields-api-openapi.yml
- filename: eztexting-com-contact-groups-api-openapi.yml
  format: yaml
  label: EZ Texting Contact Groups API
  slug: eztexting-com-contact-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-contact-groups-api-openapi.yml
- filename: eztexting-com-contacts-api-openapi.yml
  format: yaml
  label: EZ Texting Contacts API
  slug: eztexting-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-contacts-api-openapi.yml
- filename: eztexting-com-conversations-api-openapi.yml
  format: yaml
  label: EZ Texting Conversations API
  slug: eztexting-com-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-conversations-api-openapi.yml
- filename: eztexting-com-credits-api-openapi.yml
  format: yaml
  label: EZ Texting Credits API
  slug: eztexting-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-credits-api-openapi.yml
- filename: eztexting-com-keywords-api-openapi.yml
  format: yaml
  label: EZ Texting Keywords API
  slug: eztexting-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-keywords-api-openapi.yml
- filename: eztexting-com-media-files-api-openapi.yml
  format: yaml
  label: EZ Texting Media Files API
  slug: eztexting-com-media-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-media-files-api-openapi.yml
- filename: eztexting-com-message-reports-api-openapi.yml
  format: yaml
  label: EZ Texting Message Reports API
  slug: eztexting-com-message-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-message-reports-api-openapi.yml
- filename: eztexting-com-message-templates-api-openapi.yml
  format: yaml
  label: EZ Texting Message Templates API
  slug: eztexting-com-message-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-message-templates-api-openapi.yml
- filename: eztexting-com-messages-api-openapi.yml
  format: yaml
  label: EZ Texting Messages API
  slug: eztexting-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-messages-api-openapi.yml
- filename: eztexting-com-tokens-api-openapi.yml
  format: yaml
  label: EZ Texting Tokens API
  slug: eztexting-com-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-tokens-api-openapi.yml
- filename: eztexting-com-webhooks-api-openapi.yml
  format: yaml
  label: EZ Texting Webhooks API
  slug: eztexting-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: EZ Texting Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EZ Texting publishes 2 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the EZ Texting API on a user''s behalf.


  Tokens are issued from http://nova-app.stg0.cf.wtf/oauth_token/generate/swagger.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EZ Texting
provider_slug: eztexting-com
schemes:
- flows:
  - flow: password
    tokenUrl: http://nova-app.stg0.cf.wtf/oauth_token/generate/swagger
  name: oauth_auth
  source: openapi/eztexting-com-api-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: ''
  flows:
  - password
  scope: read
- description: ''
  flows:
  - password
  scope: write
slug: eztexting-com-scopes
source_filename: eztexting-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/eztexting-com-api-openapi.yml\nschemes:\n- name: oauth_auth\n  source: openapi/eztexting-com-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: http://nova-app.stg0.cf.wtf/oauth_token/generate/swagger\nscopes:\n- scope: read\n  flows:\n  - password\n  sources:\n  - openapi/eztexting-com-api-openapi.yml\n- scope: write\n  flows:\n  - password\n  sources:\n  - openapi/eztexting-com-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/eztexting-com/scopes/eztexting-com-scopes.yml
summary_line: 2 scopes · password
tags:
- SMS
- Marketing
- Communications
- Text Messaging
token_bound: false
token_urls:
- http://nova-app.stg0.cf.wtf/oauth_token/generate/swagger
---
