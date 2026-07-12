---
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Peertube Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PeerTube publishes 3 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PeerTube API on a user''s behalf.


  Tokens are issued from /api/v1/users/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PeerTube
provider_slug: peertube
schemes:
- description: 'Authenticating via OAuth requires the following steps:

    - Have an activated account

    - [Generate] an access token for that account at `/api/v1/users/token`.

    - Make requests with the *Authorization: Bearer <token\>* header

    - Profit, depending on the role assigned to the account


    Note that the __access token is valid for 1 day__ and is given

    along with a __refresh token valid for 2 weeks__.


    [Generate]: https://docs.joinpeertube.org/api/rest-getting-started'
  flows:
  - flow: password
    tokenUrl: /api/v1/users/token
  name: OAuth2
  source: openapi/openapi.json
- description: 'Authenticating via OAuth requires the following steps:

    - Have an activated account

    - [Generate] an access token for that account at `/api/v1/users/token`.

    - Make requests with the *Authorization: Bearer <token\>* header

    - Profit, depending on the role assigned to the account


    Note that the __access token is valid for 1 day__ and is given

    along with a __refresh token valid for 2 weeks__.


    [Generate]: https://docs.joinpeertube.org/api/rest-getting-started'
  flows:
  - flow: password
    tokenUrl: /api/v1/users/token
  name: OAuth2
  source: openapi/openapi.yaml
scope_count: 3
scope_names:
- admin
- moderator
- user
scopes:
- description: Admin scope
  flows:
  - password
  scope: admin
- description: Moderator scope
  flows:
  - password
  scope: moderator
- description: User scope
  flows:
  - password
  scope: user
slug: peertube-scopes
source_filename: peertube-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json, openapi/openapi.yaml\nschemes:\n- name: OAuth2\n  source: openapi/openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /api/v1/users/token\n  description: |-\n    Authenticating via OAuth requires the following steps:\n    - Have an activated account\n    - [Generate] an access token for that account at `/api/v1/users/token`.\n    - Make requests with the *Authorization: Bearer <token\\>* header\n    - Profit, depending on the role assigned to the account\n\n    Note that the __access token is valid for 1 day__ and is given\n    along with a __refresh token valid for 2 weeks__.\n\n    [Generate]: https://docs.joinpeertube.org/api/rest-getting-started\n- name: OAuth2\n  source: openapi/openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: /api/v1/users/token\n  description: |-\n    Authenticating via OAuth requires the following steps:\n    - Have an activated account\n    - [Generate] an access\
  \ token for that account at `/api/v1/users/token`.\n    - Make requests with the *Authorization: Bearer <token\\>* header\n    - Profit, depending on the role assigned to the account\n\n    Note that the __access token is valid for 1 day__ and is given\n    along with a __refresh token valid for 2 weeks__.\n\n    [Generate]: https://docs.joinpeertube.org/api/rest-getting-started\nscopes:\n- scope: admin\n  description: Admin scope\n  flows:\n  - password\n  sources:\n  - openapi/openapi.json\n  - openapi/openapi.yaml\n- scope: moderator\n  description: Moderator scope\n  flows:\n  - password\n  sources:\n  - openapi/openapi.json\n  - openapi/openapi.yaml\n- scope: user\n  description: User scope\n  flows:\n  - password\n  sources:\n  - openapi/openapi.json\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peertube/refs/heads/main/scopes/peertube-scopes.yml
summary_line: 3 scopes · password
tags:
- Video
- Decentralized
- Federation
- Open Source
- ActivityPub
- Self-Hosted
- Streaming
token_urls:
- /api/v1/users/token
---
