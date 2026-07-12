---
authorization_urls:
- https://api.att.com/oauth/v4/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: At And T Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AT&T publishes 8 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AT&T API on a user''s behalf.


  Tokens are issued from https://api.att.com/oauth/v4/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AT&T
provider_slug: at-and-t
schemes:
- description: AT&T OAuth 2.0 with user consent via authorization code flow
  flows:
  - authorizationUrl: https://api.att.com/oauth/v4/authorize
    flow: authorizationCode
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  source: openapi/at-and-t-in-app-messaging-api.yaml
- description: AT&T OAuth 2.0 authentication using client credentials grant
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  source: openapi/at-and-t-sms-api.yaml
scope_count: 8
scope_names:
- ADS
- IMMN
- MIM
- MMS
- SMS
- SPEECH
- STTC
- TTS
scopes:
- description: Access to Advertising APIs
  flows:
  - clientCredentials
  scope: ADS
- description: Send Message - send MMS and SMS messages on behalf of user
  flows:
  - authorizationCode
  scope: IMMN
- description: Message Inbox Management - read, update, and delete messages
  flows:
  - authorizationCode
  scope: MIM
- description: Access to MMS messaging APIs
  flows:
  - clientCredentials
  scope: MMS
- description: Access to SMS messaging APIs
  flows:
  - clientCredentials
  scope: SMS
- description: Access to Speech to Text APIs
  flows:
  - clientCredentials
  scope: SPEECH
- description: Access to Speech to Text Custom APIs
  flows:
  - clientCredentials
  scope: STTC
- description: Access to Text to Speech APIs
  flows:
  - clientCredentials
  scope: TTS
slug: at-and-t-scopes
source_filename: at-and-t-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/at-and-t-in-app-messaging-api.yaml, openapi/at-and-t-sms-api.yaml\nschemes:\n- name: oauth2\n  source: openapi/at-and-t-in-app-messaging-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.att.com/oauth/v4/authorize\n    tokenUrl: https://api.att.com/oauth/v4/token\n  description: AT&T OAuth 2.0 with user consent via authorization code flow\n- name: oauth2\n  source: openapi/at-and-t-sms-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.att.com/oauth/v4/token\n  description: AT&T OAuth 2.0 authentication using client credentials grant\nscopes:\n- scope: ADS\n  description: Access to Advertising APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/at-and-t-sms-api.yaml\n- scope: IMMN\n  description: Send Message - send MMS and SMS messages on behalf of user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/at-and-t-in-app-messaging-api.yaml\n- scope:\
  \ MIM\n  description: Message Inbox Management - read, update, and delete messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/at-and-t-in-app-messaging-api.yaml\n- scope: MMS\n  description: Access to MMS messaging APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/at-and-t-sms-api.yaml\n- scope: SMS\n  description: Access to SMS messaging APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/at-and-t-sms-api.yaml\n- scope: SPEECH\n  description: Access to Speech to Text APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/at-and-t-sms-api.yaml\n- scope: STTC\n  description: Access to Speech to Text Custom APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/at-and-t-sms-api.yaml\n- scope: TTS\n  description: Access to Text to Speech APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/at-and-t-sms-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/scopes/at-and-t-scopes.yml
summary_line: 8 scopes · authorizationCode/clientCredentials
tags:
- Fortune 100
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
token_urls:
- https://api.att.com/oauth/v4/token
---
