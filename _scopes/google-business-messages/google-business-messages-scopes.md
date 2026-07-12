---
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: https://developers.google.com/business-communications/business-messages/guides/how-to/integrate/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Business Messages Scopes
name_suffix: OAuth Scopes
note: Google Business Messages was sunset on July 31, 2024; the API used a single OAuth scope, documented in the OAuth guide and official client libraries.
overview: 'Google Business Messages publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Business Messages API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Business Messages
provider_slug: google-business-messages
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/businessmessages
scopes:
- description: Access the Business Messages API to send and receive messages and manage conversations as an agent.
  flows: []
  scope: https://www.googleapis.com/auth/businessmessages
slug: google-business-messages-scopes
source_filename: google-business-messages-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/openapi.yml\ndocs: https://developers.google.com/business-communications/business-messages/guides/how-to/integrate/oauth\nnote: Google Business Messages was sunset on July 31, 2024; the API used a single\n  OAuth scope, documented in the OAuth guide and official client libraries.\nschemes:\n- name: OAuth2\n  source: openapi/openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/businessmessages\n  description: Access the Business Messages API to send and receive messages and\n    manage conversations as an agent.\n  sources:\n  - https://developers.google.com/business-communications/business-messages/guides/how-to/integrate/oauth\n  - https://github.com/google-business-communications/nodejs-businessmessages\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-business-messages/refs/heads/main/scopes/google-business-messages-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Business Communications
- Conversations
- Customer Support
- Google
- Messaging
token_urls:
- https://oauth2.googleapis.com/token
---
