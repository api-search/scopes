---
authorization_urls:
- https://podio.com/oauth/authorize
description: ''
docs: https://developers.podio.com/authentication/scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Podio Scopes
name_suffix: OAuth Scopes
note: Podio scopes are parameterized as [scope]:[permission] pairs passed in the OAuth scope query parameter. Scope types are global, user, org_[id], space_[id], and app_[id]; permissions are read, write, delete, and all. Scopes are hierarchical (e.g. space access implies equivalent app access; user scope is decoupled). Omitting the scope parameter defaults to global:all.
overview: 'Podio publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Podio API on a user''s behalf.


  Tokens are issued from https://api.podio.com/oauth/token/v2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Podio
provider_slug: podio
schemes:
- flows:
  - authorizationUrl: https://podio.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.podio.com/oauth/token/v2
  name: oauth2Authorization
  source: openapi/podio-openapi.yml
scope_count: 5
scope_names:
- global:all
- user:[permission]
- org_[id]:[permission]
- space_[id]:[permission]
- app_[id]:[permission]
scopes:
- description: Full access to all accessible areas of Podio. This is the default scope granted when the scope parameter is omitted or empty.
  flows: []
  scope: global:all
- description: Access to areas related to the authenticated user, such as chat messages through the Conversations API or personal tasks. Decoupled from the other scopes and can be combined with them (space-separated). Permission is one of read, write, delete, or all.
  flows: []
  scope: user:[permission]
- description: Access to organizations; the user specifies which specific organizations are made accessible. Permission is one of read, write, delete, or all.
  flows: []
  scope: org_[id]:[permission]
- description: Access to spaces; the user specifies which specific spaces are made accessible. Granting Space scope also implicitly grants the App scope with identical permissions. Permission is one of read, write, delete, or all.
  flows: []
  scope: space_[id]:[permission]
- description: Access to apps; the user specifies which specific apps are made accessible. Permission is one of read, write, delete, or all.
  flows: []
  scope: app_[id]:[permission]
slug: podio-scopes
source_filename: podio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/podio-openapi.yml\ndocs: https://developers.podio.com/authentication/scopes\nnote: >-\n  Podio scopes are parameterized as [scope]:[permission] pairs passed in the\n  OAuth scope query parameter. Scope types are global, user, org_[id],\n  space_[id], and app_[id]; permissions are read, write, delete, and all.\n  Scopes are hierarchical (e.g. space access implies equivalent app access;\n  user scope is decoupled). Omitting the scope parameter defaults to\n  global:all.\nschemes:\n- name: oauth2Authorization\n  source: openapi/podio-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://podio.com/oauth/authorize\n    tokenUrl: https://api.podio.com/oauth/token/v2\nscopes:\n- scope: global:all\n  description: >-\n    Full access to all accessible areas of Podio. This is the default scope\n    granted when the scope parameter is omitted or empty.\n  sources:\n  - https://developers.podio.com/authentication/scopes\n\
  - scope: 'user:[permission]'\n  description: >-\n    Access to areas related to the authenticated user, such as chat messages\n    through the Conversations API or personal tasks. Decoupled from the other\n    scopes and can be combined with them (space-separated). Permission is one\n    of read, write, delete, or all.\n  sources:\n  - https://developers.podio.com/authentication/scopes\n- scope: 'org_[id]:[permission]'\n  description: >-\n    Access to organizations; the user specifies which specific organizations\n    are made accessible. Permission is one of read, write, delete, or all.\n  sources:\n  - https://developers.podio.com/authentication/scopes\n- scope: 'space_[id]:[permission]'\n  description: >-\n    Access to spaces; the user specifies which specific spaces are made\n    accessible. Granting Space scope also implicitly grants the App scope\n    with identical permissions. Permission is one of read, write, delete, or\n    all.\n  sources:\n  - https://developers.podio.com/authentication/scopes\n\
  - scope: 'app_[id]:[permission]'\n  description: >-\n    Access to apps; the user specifies which specific apps are made\n    accessible. Permission is one of read, write, delete, or all.\n  sources:\n  - https://developers.podio.com/authentication/scopes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podio/refs/heads/main/scopes/podio-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Work Management
- Collaboration
- Project Management
- CRM
- Workflow
- Custom Apps
token_urls:
- https://api.podio.com/oauth/token/v2
---
