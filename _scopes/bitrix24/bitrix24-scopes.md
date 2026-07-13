---
api_specs:
- filename: bitrix24-openapi.json
  format: json
  label: Bitrix24 REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrix24/refs/heads/main/openapi/bitrix24-openapi.json
authorization_urls:
- https://oauth.bitrix.info/oauth/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bitrix24 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bitrix24 publishes 51 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bitrix24 API on a user''s behalf.


  Tokens are issued from https://oauth.bitrix.info/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bitrix24
provider_slug: bitrix24
schemes:
- description: OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://oauth.bitrix.info/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://oauth.bitrix.info/oauth/token/
  name: OAuth2
  source: openapi/bitrix24-openapi.json
scope_count: 51
scope_names:
- ai_admin
- basic
- biconnector
- bizproc
- booking
- calendar
- cashbox
- catalog
- crm
- delivery
- department
- depending on the embedding location
- depending on the integration point
- depending on the placement
- disk
- documentgenerator
- entity
- im
- imbot
- imconnector
- imopenlines
- intranet
- landing
- lists
- log
- mailservice
- main
- messageservice
- pay_system
- placement
- rpa
- sale
- sale, cashbox
- sale, delivery
- salescenter
- sign.b2e
- socialnetwork
- sonet
- sonet_group
- task
- tasks
- telephony
- timeman
- user
- user.userfield
- user_basic
- userconsent
- userfieldconfig
- userfieldconfig, module scope
- vote
- workgroups
scopes:
- description: CoPilot / AI
  flows:
  - authorizationCode
  scope: ai_admin
- description: Basic access
  flows:
  - authorizationCode
  scope: basic
- description: BIconnector — BI analytics
  flows:
  - authorizationCode
  scope: biconnector
- description: Business processes and robots
  flows:
  - authorizationCode
  scope: bizproc
- description: Online booking
  flows:
  - authorizationCode
  scope: booking
- description: Calendar
  flows:
  - authorizationCode
  scope: calendar
- description: Online cash registers
  flows:
  - authorizationCode
  scope: cashbox
- description: Trade Catalog — products, prices
  flows:
  - authorizationCode
  scope: catalog
- description: CRM — leads, deals, contacts, companies, smart processes
  flows:
  - authorizationCode
  scope: crm
- description: Delivery services
  flows:
  - authorizationCode
  scope: delivery
- description: Company structure
  flows:
  - authorizationCode
  scope: department
- description: ''
  flows: []
  scope: depending on the embedding location
- description: ''
  flows: []
  scope: depending on the integration point
- description: ''
  flows: []
  scope: depending on the placement
- description: Drive — files and folders
  flows:
  - authorizationCode
  scope: disk
- description: Document generator
  flows:
  - authorizationCode
  scope: documentgenerator
- description: Data storage
  flows:
  - authorizationCode
  scope: entity
- description: Chats and notifications
  flows:
  - authorizationCode
  scope: im
- description: Chatbots
  flows:
  - authorizationCode
  scope: imbot
- description: IM connector
  flows:
  - authorizationCode
  scope: imconnector
- description: Open Lines — messenger connectors
  flows:
  - authorizationCode
  scope: imopenlines
- description: Intranet
  flows:
  - authorizationCode
  scope: intranet
- description: Sites and landing pages
  flows:
  - authorizationCode
  scope: landing
- description: Universal lists
  flows:
  - authorizationCode
  scope: lists
- description: News feed
  flows:
  - authorizationCode
  scope: log
- description: Mail services
  flows:
  - authorizationCode
  scope: mailservice
- description: Main module
  flows:
  - authorizationCode
  scope: main
- description: Message providers (SMS)
  flows:
  - authorizationCode
  scope: messageservice
- description: Payment systems
  flows:
  - authorizationCode
  scope: pay_system
- description: Widget placements
  flows:
  - authorizationCode
  scope: placement
- description: Robots process automation
  flows:
  - authorizationCode
  scope: rpa
- description: E-Commerce — orders, shipments
  flows:
  - authorizationCode
  scope: sale
- description: ''
  flows: []
  scope: sale, cashbox
- description: ''
  flows: []
  scope: sale, delivery
- description: Sales center
  flows:
  - authorizationCode
  scope: salescenter
- description: Signature — e-document signing
  flows:
  - authorizationCode
  scope: sign.b2e
- description: Social network
  flows:
  - authorizationCode
  scope: socialnetwork
- description: Social network
  flows:
  - authorizationCode
  scope: sonet
- description: Workgroups and projects
  flows:
  - authorizationCode
  scope: sonet_group
- description: Tasks and projects
  flows:
  - authorizationCode
  scope: task
- description: ''
  flows: []
  scope: tasks
- description: Telephony
  flows:
  - authorizationCode
  scope: telephony
- description: Time tracking
  flows:
  - authorizationCode
  scope: timeman
- description: Users
  flows:
  - authorizationCode
  scope: user
- description: User custom fields
  flows:
  - authorizationCode
  scope: user.userfield
- description: Basic user access
  flows:
  - authorizationCode
  scope: user_basic
- description: User consent agreements
  flows:
  - authorizationCode
  scope: userconsent
- description: Custom field settings
  flows:
  - authorizationCode
  scope: userfieldconfig
- description: Custom field config
  flows:
  - authorizationCode
  scope: userfieldconfig, module scope
- description: Polls and voting
  flows:
  - authorizationCode
  scope: vote
- description: Workgroups
  flows:
  - authorizationCode
  scope: workgroups
slug: bitrix24-scopes
source_filename: bitrix24-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitrix24-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/bitrix24-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.bitrix.info/oauth/authorize/\n    tokenUrl: https://oauth.bitrix.info/oauth/token/\n  description: OAuth 2.0 authorization\nscopes:\n- scope: ai_admin\n  description: CoPilot / AI\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: basic\n  description: Basic access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: biconnector\n  description: BIconnector — BI analytics\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: bizproc\n  description: Business processes and robots\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: booking\n  description: Online booking\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/bitrix24-openapi.json\n- scope: calendar\n  description: Calendar\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: cashbox\n  description: Online cash registers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: catalog\n  description: Trade Catalog — products, prices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: crm\n  description: CRM — leads, deals, contacts, companies, smart processes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: delivery\n  description: Delivery services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: department\n  description: Company structure\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: depending on the embedding location\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: depending on the integration\
  \ point\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: depending on the placement\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: disk\n  description: Drive — files and folders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: documentgenerator\n  description: Document generator\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: entity\n  description: Data storage\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: im\n  description: Chats and notifications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: imbot\n  description: Chatbots\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: imconnector\n  description: IM connector\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: imopenlines\n  description: Open Lines — messenger connectors\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: intranet\n  description: Intranet\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: landing\n  description: Sites and landing pages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: lists\n  description: Universal lists\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: log\n  description: News feed\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: mailservice\n  description: Mail services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: main\n  description: Main module\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: messageservice\n  description: Message providers (SMS)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope:\
  \ pay_system\n  description: Payment systems\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: placement\n  description: Widget placements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: rpa\n  description: Robots process automation\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: sale\n  description: E-Commerce — orders, shipments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: sale, cashbox\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: sale, delivery\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: salescenter\n  description: Sales center\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: sign.b2e\n  description: Signature — e-document signing\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: socialnetwork\n  description: Social\
  \ network\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: sonet\n  description: Social network\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: sonet_group\n  description: Workgroups and projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: task\n  description: Tasks and projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: tasks\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: telephony\n  description: Telephony\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: timeman\n  description: Time tracking\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: user\n  description: Users\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: user.userfield\n  description: User custom fields\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/bitrix24-openapi.json\n- scope: user_basic\n  description: Basic user access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: userconsent\n  description: User consent agreements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: userfieldconfig\n  description: Custom field settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: userfieldconfig, module scope\n  description: Custom field config\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: vote\n  description: Polls and voting\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n- scope: workgroups\n  description: Workgroups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bitrix24-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitrix24/refs/heads/main/scopes/bitrix24-scopes.yml
summary_line: 51 scopes · authorizationCode
tags:
- CRM
- Collaboration
- Project Management
- Tasks
- Telephony
- Contact Center
- Document Management
- HR
- Business Suite
token_urls:
- https://oauth.bitrix.info/oauth/token/
---
