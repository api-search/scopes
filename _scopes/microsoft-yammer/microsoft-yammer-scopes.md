---
authorization_urls:
- https://www.yammer.com/dialog/oauth
description: ''
docs: https://learn.microsoft.com/en-us/rest/api/yammer/app-registration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Yammer Scopes
name_suffix: OAuth Scopes
note: Legacy Yammer OAuth 2.0 tokens carry no granular scopes (a token grants full access as the authorizing user), and legacy app registrations are restricted as of July 1, 2025. Microsoft now directs developers to Entra applications, where the Yammer API exposes delegated permissions only — no application permissions are supported (https://learn.microsoft.com/en-us/rest/api/yammer/app-registration).
overview: 'Microsoft Yammer publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Yammer API on a user''s behalf.


  Tokens are issued from https://www.yammer.com/oauth2/access_token.json.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Yammer
provider_slug: microsoft-yammer
schemes:
- description: Yammer OAuth 2.0 legacy tokens or Microsoft Entra tokens. Delegated access only.
  flows:
  - authorizationUrl: https://www.yammer.com/dialog/oauth
    flow: authorizationCode
    tokenUrl: https://www.yammer.com/oauth2/access_token.json
  name: OAuth2
  source: openapi/microsoft-yammer-openapi.yml
scope_count: 2
scope_names:
- access_as_user
- user_impersonation
scopes:
- description: Delegated Entra permission for the Yammer API; allows the application to read and write to the Viva Engage (Yammer) platform on behalf of the signed-in user. The permission Microsoft's app-registration guide says to select for Entra applications calling the legacy Yammer REST APIs.
  flows: []
  scope: access_as_user
- description: Delegated Entra permission for the Yammer API used with AAD/Entra tokens; allows the application to access the Yammer platform as the signed-in user (used by the Yammer-API-with-AAD-tokens flow, requested as https://api.yammer.com/user_impersonation).
  flows: []
  scope: user_impersonation
slug: microsoft-yammer-scopes
source_filename: microsoft-yammer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/microsoft-yammer-openapi.yml\ndocs: https://learn.microsoft.com/en-us/rest/api/yammer/app-registration\nnote: Legacy Yammer OAuth 2.0 tokens carry no granular scopes (a token grants full\n  access as the authorizing user), and legacy app registrations are restricted as\n  of July 1, 2025. Microsoft now directs developers to Entra applications, where\n  the Yammer API exposes delegated permissions only — no application permissions\n  are supported (https://learn.microsoft.com/en-us/rest/api/yammer/app-registration).\nschemes:\n- name: OAuth2\n  source: openapi/microsoft-yammer-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.yammer.com/dialog/oauth\n    tokenUrl: https://www.yammer.com/oauth2/access_token.json\n  description: Yammer OAuth 2.0 legacy tokens or Microsoft Entra tokens. Delegated access only.\nscopes:\n- scope: access_as_user\n  description: Delegated Entra permission\
  \ for the Yammer API; allows the application\n    to read and write to the Viva Engage (Yammer) platform on behalf of the signed-in\n    user. The permission Microsoft's app-registration guide says to select for Entra\n    applications calling the legacy Yammer REST APIs.\n  sources:\n  - https://learn.microsoft.com/en-us/rest/api/yammer/app-registration\n- scope: user_impersonation\n  description: Delegated Entra permission for the Yammer API used with AAD/Entra\n    tokens; allows the application to access the Yammer platform as the signed-in\n    user (used by the Yammer-API-with-AAD-tokens flow, requested as\n    https://api.yammer.com/user_impersonation).\n  sources:\n  - https://techcommunity.microsoft.com/blog/viva_engage_blog/yammer-api-with-aad-tokens-postman-collection/857923\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-yammer/refs/heads/main/scopes/microsoft-yammer-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Enterprise Social
- Microsoft
- Social Networking
- Viva Engage
- Yammer
token_urls:
- https://www.yammer.com/oauth2/access_token.json
---
