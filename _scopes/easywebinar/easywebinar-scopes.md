---
authorization_urls:
- https://app.easywebinar.com/oauth/authorize/
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- implicit
kind: oauth-scopes
layout: scope
method: probed
name: Easywebinar Scopes
name_suffix: OAuth Scopes
note: EasyWebinar publishes no scopes / permissions reference page. Every scope below is read verbatim from scopes_supported in the live discovery document. There is no OpenAPI to derive operation-level scope requirements from, so the mapping of scope to capability is unknown and deliberately left unstated rather than guessed.
overview: 'EasyWebinar publishes 4 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the EasyWebinar API on a user''s behalf.


  Tokens are issued from https://app.easywebinar.com/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EasyWebinar
provider_slug: easywebinar
schemes:
- flows:
  - authorizationUrl: https://app.easywebinar.com/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://app.easywebinar.com/oauth/token/
  - flow: clientCredentials
    tokenUrl: https://app.easywebinar.com/oauth/token/
  - authorizationUrl: https://app.easywebinar.com/oauth/authorize/
    flow: implicit
  issuer: https://app.easywebinar.com
  name: EasyWebinarOAuth2
  source: well-known/easywebinar-openid-configuration.json
scope_count: 4
scope_names:
- openid
- profile
- email
- basic
scopes:
- description: Standard OIDC scope requesting an id_token for the authenticated EasyWebinar user. Description is the OIDC Core definition; EasyWebinar publishes none of its own.
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: openid
- description: Standard OIDC scope for the end-user profile claims returned by /oauth/me/. Description is the OIDC Core definition; EasyWebinar publishes none of its own.
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: profile
- description: Standard OIDC scope for the email and email_verified claims. Description is the OIDC Core definition; EasyWebinar publishes none of its own.
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: email
- description: Vendor-specific scope advertised by the authorization server. EasyWebinar publishes no definition for it and there is no reference to resolve it against.
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: basic
slug: easywebinar-scopes
source_filename: easywebinar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://app.easywebinar.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  EasyWebinar publishes no scopes / permissions reference page. Every scope below is read\n  verbatim from scopes_supported in the live discovery document. There is no OpenAPI to\n  derive operation-level scope requirements from, so the mapping of scope to capability is\n  unknown and deliberately left unstated rather than guessed.\nschemes:\n  - name: EasyWebinarOAuth2\n    source: well-known/easywebinar-openid-configuration.json\n    issuer: https://app.easywebinar.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.easywebinar.com/oauth/authorize/\n        tokenUrl: https://app.easywebinar.com/oauth/token/\n      - flow: clientCredentials\n        tokenUrl: https://app.easywebinar.com/oauth/token/\n      - flow: implicit\n        authorizationUrl: https://app.easywebinar.com/oauth/authorize/\nscopes:\n  -\
  \ scope: openid\n    description: >-\n      Standard OIDC scope requesting an id_token for the authenticated EasyWebinar user.\n      Description is the OIDC Core definition; EasyWebinar publishes none of its own.\n    flows: [authorizationCode, clientCredentials, implicit]\n    sources: [well-known/easywebinar-openid-configuration.json]\n  - scope: profile\n    description: >-\n      Standard OIDC scope for the end-user profile claims returned by /oauth/me/.\n      Description is the OIDC Core definition; EasyWebinar publishes none of its own.\n    flows: [authorizationCode, clientCredentials, implicit]\n    sources: [well-known/easywebinar-openid-configuration.json]\n  - scope: email\n    description: >-\n      Standard OIDC scope for the email and email_verified claims. Description is the OIDC\n      Core definition; EasyWebinar publishes none of its own.\n    flows: [authorizationCode, clientCredentials, implicit]\n    sources: [well-known/easywebinar-openid-configuration.json]\n \
  \ - scope: basic\n    description: >-\n      Vendor-specific scope advertised by the authorization server. EasyWebinar publishes\n      no definition for it and there is no reference to resolve it against.\n    flows: [authorizationCode, clientCredentials, implicit]\n    sources: [well-known/easywebinar-openid-configuration.json]\nscope_count: 4\ngaps:\n  - >-\n    No resource-level scopes are advertised. The REST API EasyWebinar markets on its\n    enterprise page (registration, attendance, lead data, CRM sync, event lifecycle) has no\n    corresponding scope in the published metadata, so either it authenticates by another\n    mechanism or its scopes are not discoverable anonymously.\nx-evidence:\n  - url: https://app.easywebinar.com/.well-known/openid-configuration\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easywebinar/refs/heads/main/scopes/easywebinar-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials/implicit
tags:
- Company
- Webinars
- Video
- Live Streaming
- Marketing
- Events
- CRM
- Lead Generation
- Automation
- Identity
- OAuth
- SaaS
token_urls:
- https://app.easywebinar.com/oauth/token/
---
