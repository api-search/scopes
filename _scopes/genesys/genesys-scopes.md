---
api_specs:
- filename: genesys-platform-api-openapi-original.json
  format: json
  label: Genesys Cloud Platform API
  slug: genesys-cloud-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genesys/refs/heads/main/openapi/genesys-platform-api-openapi-original.json
authorization_urls:
- https://login.mypurecloud.com/authorize
description: ''
docs: https://developer.genesys.cloud/authorization/scopes/
flows:
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Genesys Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Genesys publishes 135 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Genesys API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Genesys
provider_slug: genesys
schemes:
- flows:
  - authorizationUrl: https://login.mypurecloud.com/authorize
    flow: implicit
  name: PureCloud OAuth
  source: openapi/genesys-platform-api-openapi-original.json
scope_count: 135
scope_names:
- ai-studio
- ai-studio:readonly
- alerting
- alerting:readonly
- all
- analytics
- analytics:readonly
- architect
- architect:readonly
- assistants
- assistants:readonly
- audits:readonly
- authorization
- authorization:readonly
- billing
- billing:readonly
- business-rules
- business-rules:readonly
- case-management
- case-management:readonly
- coaching
- coaching:readonly
- content-management
- content-management:readonly
- conversations
- conversations:readonly
- data-extensions
- data-privacy
- data-privacy:readonly
- devices
- devices:readonly
- dialog
- dialog:readonly
- employee-engagement
- employee-engagement:readonly
- employee-performance
- employee-performance:readonly
- external-contacts
- external-contacts:readonly
- fax
- fax:readonly
- gamification
- gamification:readonly
- gdpr
- gdpr:readonly
- geolocation
- geolocation:readonly
- greetings
- greetings:readonly
- groups
- groups:readonly
- identity-providers
- identity-providers:readonly
- infrastructureascode
- infrastructureascode:readonly
- integrations
- integrations:readonly
- journey
- journey:readonly
- knowledge
- knowledge:readonly
- language-understanding
- language-understanding:readonly
- learning
- learning:readonly
- license
- license:readonly
- locations
- locations:readonly
- logcapture
- logcapture:readonly
- messaging
- messaging-platform
- messaging-platform:readonly
- messaging:readonly
- notifications
- oauth
- oauth:readonly
- organization
- organization-authorization
- organization-authorization:readonly
- organization:readonly
- outbound
- outbound:readonly
- presence
- presence:readonly
- process-automation
- process-automation:readonly
- quality
- quality:readonly
- recordings
- recordings:readonly
- response-management
- response-management:readonly
- routing
- routing:readonly
- scim
- scim:readonly
- screen-monitoring
- screen-monitoring:readonly
- scripts
- scripts:readonly
- search:readonly
- social-media
- social-media:readonly
- speech-and-text-analytics
- speech-and-text-analytics:readonly
- stations
- stations:readonly
- telephony
- telephony:readonly
- textbots
- textbots:readonly
- upload
- usage
- usage:readonly
- user-basic-info
- user-recordings
- user-recordings:readonly
- users
- users-rules
- users-rules:readonly
- users:readonly
- voicemail
- voicemail:readonly
- web-chat
- web-chat:readonly
- webdeployments
- webdeployments:readonly
- widgets
- widgets:readonly
- workforce-management
- workforce-management:readonly
- workitems
- workitems:readonly
scopes:
- description: ''
  flows: []
  scope: ai-studio
- description: ''
  flows: []
  scope: ai-studio:readonly
- description: ''
  flows: []
  scope: alerting
- description: ''
  flows: []
  scope: alerting:readonly
- description: All the scopes
  flows:
  - implicit
  scope: all
- description: ''
  flows: []
  scope: analytics
- description: ''
  flows: []
  scope: analytics:readonly
- description: ''
  flows: []
  scope: architect
- description: ''
  flows: []
  scope: architect:readonly
- description: ''
  flows: []
  scope: assistants
- description: ''
  flows: []
  scope: assistants:readonly
- description: ''
  flows: []
  scope: audits:readonly
- description: ''
  flows: []
  scope: authorization
- description: ''
  flows: []
  scope: authorization:readonly
- description: ''
  flows: []
  scope: billing
- description: ''
  flows: []
  scope: billing:readonly
- description: ''
  flows: []
  scope: business-rules
- description: ''
  flows: []
  scope: business-rules:readonly
- description: ''
  flows: []
  scope: case-management
- description: ''
  flows: []
  scope: case-management:readonly
- description: ''
  flows: []
  scope: coaching
- description: ''
  flows: []
  scope: coaching:readonly
- description: ''
  flows: []
  scope: content-management
- description: ''
  flows: []
  scope: content-management:readonly
- description: ''
  flows: []
  scope: conversations
- description: ''
  flows: []
  scope: conversations:readonly
- description: ''
  flows: []
  scope: data-extensions
- description: ''
  flows: []
  scope: data-privacy
- description: ''
  flows: []
  scope: data-privacy:readonly
- description: ''
  flows: []
  scope: devices
- description: ''
  flows: []
  scope: devices:readonly
- description: ''
  flows: []
  scope: dialog
- description: ''
  flows: []
  scope: dialog:readonly
- description: ''
  flows: []
  scope: employee-engagement
- description: ''
  flows: []
  scope: employee-engagement:readonly
- description: ''
  flows: []
  scope: employee-performance
- description: ''
  flows: []
  scope: employee-performance:readonly
- description: ''
  flows: []
  scope: external-contacts
- description: ''
  flows: []
  scope: external-contacts:readonly
- description: ''
  flows: []
  scope: fax
- description: ''
  flows: []
  scope: fax:readonly
- description: ''
  flows: []
  scope: gamification
- description: ''
  flows: []
  scope: gamification:readonly
- description: ''
  flows: []
  scope: gdpr
- description: ''
  flows: []
  scope: gdpr:readonly
- description: ''
  flows: []
  scope: geolocation
- description: ''
  flows: []
  scope: geolocation:readonly
- description: ''
  flows: []
  scope: greetings
- description: ''
  flows: []
  scope: greetings:readonly
- description: ''
  flows: []
  scope: groups
- description: ''
  flows: []
  scope: groups:readonly
- description: ''
  flows: []
  scope: identity-providers
- description: ''
  flows: []
  scope: identity-providers:readonly
- description: ''
  flows: []
  scope: infrastructureascode
- description: ''
  flows: []
  scope: infrastructureascode:readonly
- description: ''
  flows: []
  scope: integrations
- description: ''
  flows: []
  scope: integrations:readonly
- description: ''
  flows: []
  scope: journey
- description: ''
  flows: []
  scope: journey:readonly
- description: ''
  flows: []
  scope: knowledge
- description: ''
  flows: []
  scope: knowledge:readonly
- description: ''
  flows: []
  scope: language-understanding
- description: ''
  flows: []
  scope: language-understanding:readonly
- description: ''
  flows: []
  scope: learning
- description: ''
  flows: []
  scope: learning:readonly
- description: ''
  flows: []
  scope: license
- description: ''
  flows: []
  scope: license:readonly
- description: ''
  flows: []
  scope: locations
- description: ''
  flows: []
  scope: locations:readonly
- description: ''
  flows: []
  scope: logcapture
- description: ''
  flows: []
  scope: logcapture:readonly
- description: ''
  flows: []
  scope: messaging
- description: ''
  flows: []
  scope: messaging-platform
- description: ''
  flows: []
  scope: messaging-platform:readonly
- description: ''
  flows: []
  scope: messaging:readonly
- description: ''
  flows: []
  scope: notifications
- description: ''
  flows: []
  scope: oauth
- description: ''
  flows: []
  scope: oauth:readonly
- description: ''
  flows: []
  scope: organization
- description: ''
  flows: []
  scope: organization-authorization
- description: ''
  flows: []
  scope: organization-authorization:readonly
- description: ''
  flows: []
  scope: organization:readonly
- description: ''
  flows: []
  scope: outbound
- description: ''
  flows: []
  scope: outbound:readonly
- description: ''
  flows: []
  scope: presence
- description: ''
  flows: []
  scope: presence:readonly
- description: ''
  flows: []
  scope: process-automation
- description: ''
  flows: []
  scope: process-automation:readonly
- description: ''
  flows: []
  scope: quality
- description: ''
  flows: []
  scope: quality:readonly
- description: ''
  flows: []
  scope: recordings
- description: ''
  flows: []
  scope: recordings:readonly
- description: ''
  flows: []
  scope: response-management
- description: ''
  flows: []
  scope: response-management:readonly
- description: ''
  flows: []
  scope: routing
- description: ''
  flows: []
  scope: routing:readonly
- description: ''
  flows: []
  scope: scim
- description: ''
  flows: []
  scope: scim:readonly
- description: ''
  flows: []
  scope: screen-monitoring
- description: ''
  flows: []
  scope: screen-monitoring:readonly
- description: ''
  flows: []
  scope: scripts
- description: ''
  flows: []
  scope: scripts:readonly
- description: ''
  flows: []
  scope: search:readonly
- description: ''
  flows: []
  scope: social-media
- description: ''
  flows: []
  scope: social-media:readonly
- description: ''
  flows: []
  scope: speech-and-text-analytics
- description: ''
  flows: []
  scope: speech-and-text-analytics:readonly
- description: ''
  flows: []
  scope: stations
- description: ''
  flows: []
  scope: stations:readonly
- description: ''
  flows: []
  scope: telephony
- description: ''
  flows: []
  scope: telephony:readonly
- description: ''
  flows: []
  scope: textbots
- description: ''
  flows: []
  scope: textbots:readonly
- description: ''
  flows: []
  scope: upload
- description: ''
  flows: []
  scope: usage
- description: ''
  flows: []
  scope: usage:readonly
- description: ''
  flows: []
  scope: user-basic-info
- description: ''
  flows: []
  scope: user-recordings
- description: ''
  flows: []
  scope: user-recordings:readonly
- description: ''
  flows: []
  scope: users
- description: ''
  flows: []
  scope: users-rules
- description: ''
  flows: []
  scope: users-rules:readonly
- description: ''
  flows: []
  scope: users:readonly
- description: ''
  flows: []
  scope: voicemail
- description: ''
  flows: []
  scope: voicemail:readonly
- description: ''
  flows: []
  scope: web-chat
- description: ''
  flows: []
  scope: web-chat:readonly
- description: ''
  flows: []
  scope: webdeployments
- description: ''
  flows: []
  scope: webdeployments:readonly
- description: ''
  flows: []
  scope: widgets
- description: ''
  flows: []
  scope: widgets:readonly
- description: ''
  flows: []
  scope: workforce-management
- description: ''
  flows: []
  scope: workforce-management:readonly
- description: ''
  flows: []
  scope: workitems
- description: ''
  flows: []
  scope: workitems:readonly
slug: genesys-scopes
source_filename: genesys-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/genesys-platform-api-openapi-original.json\ndocs: https://developer.genesys.cloud/authorization/scopes/\nnotes: >-\n  135 OAuth scopes derived from operation-level security requirements in the\n  Platform API OpenAPI. Scopes follow a <domain> / <domain>:readonly pattern\n  (e.g. analytics, analytics:readonly). Scope enforcement is disabled by default\n  per organization and must be explicitly enabled. The canonical reference is\n  the developer-center scopes page.\nschemes:\n- name: PureCloud OAuth\n  source: openapi/genesys-platform-api-openapi-original.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.mypurecloud.com/authorize\nscopes:\n- scope: ai-studio\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: ai-studio:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: alerting\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n\
  - scope: alerting:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: all\n  description: All the scopes\n  flows:\n  - implicit\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: analytics\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: analytics:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: architect\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: architect:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: assistants\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: assistants:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: audits:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: authorization\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: authorization:readonly\n\
  \  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: billing\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: billing:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: business-rules\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: business-rules:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: case-management\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: case-management:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: coaching\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: coaching:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: content-management\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: content-management:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n\
  - scope: conversations\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: conversations:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: data-extensions\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: data-privacy\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: data-privacy:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: devices\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: devices:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: dialog\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: dialog:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: employee-engagement\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: employee-engagement:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n\
  - scope: employee-performance\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: employee-performance:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: external-contacts\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: external-contacts:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: fax\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: fax:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: gamification\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: gamification:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: gdpr\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: gdpr:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: geolocation\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n\
  - scope: geolocation:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: greetings\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: greetings:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: groups\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: groups:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: identity-providers\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: identity-providers:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: infrastructureascode\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: infrastructureascode:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: integrations\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: integrations:readonly\n  sources:\n\
  \  - openapi/genesys-platform-api-openapi-original.json\n- scope: journey\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: journey:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: knowledge\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: knowledge:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: language-understanding\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: language-understanding:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: learning\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: learning:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: license\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: license:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n-\
  \ scope: locations\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: locations:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: logcapture\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: logcapture:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: messaging\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: messaging-platform\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: messaging-platform:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: messaging:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: notifications\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: oauth\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: oauth:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n\
  - scope: organization\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: organization-authorization\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: organization-authorization:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: organization:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: outbound\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: outbound:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: presence\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: presence:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: process-automation\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: process-automation:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: quality\n  sources:\n\
  \  - openapi/genesys-platform-api-openapi-original.json\n- scope: quality:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: recordings\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: recordings:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: response-management\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: response-management:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: routing\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: routing:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: scim\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: scim:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: screen-monitoring\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope:\
  \ screen-monitoring:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: scripts\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: scripts:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: search:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: social-media\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: social-media:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: speech-and-text-analytics\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: speech-and-text-analytics:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: stations\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: stations:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: telephony\n  sources:\n  -\
  \ openapi/genesys-platform-api-openapi-original.json\n- scope: telephony:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: textbots\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: textbots:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: upload\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: usage\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: usage:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: user-basic-info\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: user-recordings\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: user-recordings:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: users\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: users-rules\n  sources:\n\
  \  - openapi/genesys-platform-api-openapi-original.json\n- scope: users-rules:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: users:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: voicemail\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: voicemail:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: web-chat\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: web-chat:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: webdeployments\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: webdeployments:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: widgets\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: widgets:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope:\
  \ workforce-management\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: workforce-management:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: workitems\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n- scope: workitems:readonly\n  sources:\n  - openapi/genesys-platform-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genesys/refs/heads/main/scopes/genesys-scopes.yml
summary_line: 135 scopes · implicit
tags:
- Company
- Software
- Contact Center
- Customer Experience
- CCaaS
- Telephony
- Conversational AI
- Workforce Management
- Cloud Communications
- CPaaS
token_urls: []
---
