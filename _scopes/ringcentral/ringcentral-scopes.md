---
api_specs:
- filename: ringcentral-platform-openapi.yml
  format: yaml
  label: RingCentral Voice API
  slug: ringcentral-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/openapi/ringcentral-platform-openapi.yml
- filename: ringcentral-subscriptions-asyncapi.yaml
  format: yaml
  label: RingCentral Webhooks and Subscriptions API
  slug: ringcentral-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/asyncapi/ringcentral-subscriptions-asyncapi.yaml
authorization_urls:
- https://platform.ringcentral.com/restapi/oauth/authorize
description: ''
docs: https://developers.ringcentral.com/guide/basics/permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ringcentral Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RingCentral publishes 38 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the RingCentral API on a user''s behalf.


  Tokens are issued from https://platform.ringcentral.com/restapi/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RingCentral
provider_slug: ringcentral
schemes:
- flows:
  - authorizationUrl: https://platform.ringcentral.com/restapi/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.ringcentral.com/restapi/oauth/token
  name: OAuth2
  source: openapi/ringcentral-platform-openapi.yml
scope_count: 38
scope_names:
- A2P SMS
- Accounts
- EditAccounts
- AI
- Analytics
- CallControl
- Contacts
- ControlWebinars
- DirectRingOut
- EditCallLog
- EditCustomData
- EditExtensions
- EditMessages
- EditPaymentInfo
- EditPresence
- EditReportingSettings
- EditUserCredentials
- EditWebinars
- Faxes
- Glip
- InternalMessages
- Meetings
- ReadAccounts
- ReadCallLog
- ReadCallRecording
- ReadClientInfo
- ReadContacts
- ReadMessages
- ReadPresence
- ReadWebinars
- RingOut
- RoleManagement
- SMS
- SubscriptionWebhook
- TeamMessaging
- Video
- Voicemail
- VoipCalling
scopes:
- description: Sending SMS messages in large numbers (high-volume / A2P).
  flows: []
  scope: A2P SMS
- description: Managing accounts - creating, viewing, updating, and deleting account information.
  flows: []
  scope: Accounts
- description: Viewing and updating user account info (name, business name, address, phone/account number).
  flows: []
  scope: EditAccounts
- description: Analyze audio and text; view and update analysis info including speaker samples.
  flows: []
  scope: AI
- description: Access call analytics data via the Analytics product.
  flows: []
  scope: Analytics
- description: Manipulate and control calls in progress.
  flows: []
  scope: CallControl
- description: Creating, viewing, editing and deleting user personal contacts.
  flows: []
  scope: Contacts
- description: Control webinar sessions.
  flows: []
  scope: ControlWebinars
- description: Performing direct (one-legged) ring-out phone calls. Available on request.
  flows: []
  scope: DirectRingOut
- description: Viewing and updating user call logs.
  flows: []
  scope: EditCallLog
- description: Viewing and updating client custom data (key-value).
  flows: []
  scope: EditCustomData
- description: Viewing and updating user extension info.
  flows: []
  scope: EditExtensions
- description: Viewing and updating user messages.
  flows: []
  scope: EditMessages
- description: Viewing and updating account billing settings.
  flows: []
  scope: EditPaymentInfo
- description: Getting and modifying user presence information.
  flows: []
  scope: EditPresence
- description: Viewing and updating call reporting settings. Available on request.
  flows: []
  scope: EditReportingSettings
- description: Editing and managing a user's login credentials including their password. Available on request.
  flows: []
  scope: EditUserCredentials
- description: Viewing and updating webinars and webinar sessions.
  flows: []
  scope: EditWebinars
- description: Sending and receiving faxes.
  flows: []
  scope: Faxes
- description: Read and post messages, read and manage chats (Team Messaging / Glip).
  flows: []
  scope: Glip
- description: Sending and receiving intra-company text messages (pager messages).
  flows: []
  scope: InternalMessages
- description: Creating, viewing, editing and deleting meetings via RingCentral Meetings.
  flows: []
  scope: Meetings
- description: Viewing user account info (name, business name, address, phone/account number).
  flows: []
  scope: ReadAccounts
- description: Viewing user call logs.
  flows: []
  scope: ReadCallLog
- description: Downloading call recording content.
  flows: []
  scope: ReadCallRecording
- description: Viewing client application registered attributes and helper information.
  flows: []
  scope: ReadClientInfo
- description: Viewing user personal contacts.
  flows: []
  scope: ReadContacts
- description: Viewing user messages.
  flows: []
  scope: ReadMessages
- description: Getting user presence information.
  flows: []
  scope: ReadPresence
- description: Viewing webinars and webinar sessions.
  flows: []
  scope: ReadWebinars
- description: Performing two-legged ring-out phone calls.
  flows: []
  scope: RingOut
- description: Editing and assignment of user roles. Available on request.
  flows: []
  scope: RoleManagement
- description: Sending and receiving SMS text messages.
  flows: []
  scope: SMS
- description: Subscribing to and managing webhook notification preferences.
  flows: []
  scope: SubscriptionWebhook
- description: Post messages and view, edit and delete Team Messaging related data.
  flows: []
  scope: TeamMessaging
- description: Creating, viewing, editing and deleting meetings via RingCentral Video.
  flows: []
  scope: Video
- description: Delivering voicemail messages to multiple internal recipients.
  flows: []
  scope: Voicemail
- description: Registering as a VoIP device and making VoIP calls.
  flows: []
  scope: VoipCalling
slug: ringcentral-scopes
source_filename: ringcentral-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/ringcentral-platform-openapi.yml\ndocs: https://developers.ringcentral.com/guide/basics/permissions\nnotes: >-\n  The OpenAPI declares a single OAuth2 authorizationCode scheme but publishes an\n  empty scopes map; the scope list below is captured from the RingCentral\n  \"Application permissions and scopes\" reference. Scopes marked requires_permission\n  are restricted and available on request / gated by an account role.\nschemes:\n  - name: OAuth2\n    source: openapi/ringcentral-platform-openapi.yml\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://platform.ringcentral.com/restapi/oauth/authorize\n        tokenUrl: https://platform.ringcentral.com/restapi/oauth/token\nscopes:\n  - scope: A2P SMS\n    description: Sending SMS messages in large numbers (high-volume / A2P).\n  - scope: Accounts\n    description: Managing accounts - creating, viewing, updating, and deleting account information.\n\
  \  - scope: EditAccounts\n    description: Viewing and updating user account info (name, business name, address, phone/account number).\n  - scope: AI\n    description: Analyze audio and text; view and update analysis info including speaker samples.\n  - scope: Analytics\n    description: Access call analytics data via the Analytics product.\n  - scope: CallControl\n    description: Manipulate and control calls in progress.\n  - scope: Contacts\n    description: Creating, viewing, editing and deleting user personal contacts.\n  - scope: ControlWebinars\n    description: Control webinar sessions.\n  - scope: DirectRingOut\n    description: Performing direct (one-legged) ring-out phone calls. Available on request.\n    requires_permission: true\n  - scope: EditCallLog\n    description: Viewing and updating user call logs.\n  - scope: EditCustomData\n    description: Viewing and updating client custom data (key-value).\n  - scope: EditExtensions\n    description: Viewing and updating user\
  \ extension info.\n  - scope: EditMessages\n    description: Viewing and updating user messages.\n  - scope: EditPaymentInfo\n    description: Viewing and updating account billing settings.\n  - scope: EditPresence\n    description: Getting and modifying user presence information.\n  - scope: EditReportingSettings\n    description: Viewing and updating call reporting settings. Available on request.\n    requires_permission: true\n  - scope: EditUserCredentials\n    description: Editing and managing a user's login credentials including their password. Available on request.\n    requires_permission: true\n  - scope: EditWebinars\n    description: Viewing and updating webinars and webinar sessions.\n  - scope: Faxes\n    description: Sending and receiving faxes.\n  - scope: Glip\n    description: Read and post messages, read and manage chats (Team Messaging / Glip).\n  - scope: InternalMessages\n    description: Sending and receiving intra-company text messages (pager messages).\n  - scope:\
  \ Meetings\n    description: Creating, viewing, editing and deleting meetings via RingCentral Meetings.\n  - scope: ReadAccounts\n    description: Viewing user account info (name, business name, address, phone/account number).\n  - scope: ReadCallLog\n    description: Viewing user call logs.\n  - scope: ReadCallRecording\n    description: Downloading call recording content.\n  - scope: ReadClientInfo\n    description: Viewing client application registered attributes and helper information.\n  - scope: ReadContacts\n    description: Viewing user personal contacts.\n  - scope: ReadMessages\n    description: Viewing user messages.\n  - scope: ReadPresence\n    description: Getting user presence information.\n  - scope: ReadWebinars\n    description: Viewing webinars and webinar sessions.\n  - scope: RingOut\n    description: Performing two-legged ring-out phone calls.\n  - scope: RoleManagement\n    description: Editing and assignment of user roles. Available on request.\n    requires_permission:\
  \ true\n  - scope: SMS\n    description: Sending and receiving SMS text messages.\n  - scope: SubscriptionWebhook\n    description: Subscribing to and managing webhook notification preferences.\n  - scope: TeamMessaging\n    description: Post messages and view, edit and delete Team Messaging related data.\n  - scope: Video\n    description: Creating, viewing, editing and deleting meetings via RingCentral Video.\n  - scope: Voicemail\n    description: Delivering voicemail messages to multiple internal recipients.\n  - scope: VoipCalling\n    description: Registering as a VoIP device and making VoIP calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/scopes/ringcentral-scopes.yml
summary_line: 38 scopes · authorizationCode
tags:
- Communications
- UCaaS
- Voice
- Video
- Contact Center
- SMS
- Messaging
- Fax
token_urls:
- https://platform.ringcentral.com/restapi/oauth/token
---
