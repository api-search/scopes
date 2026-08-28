---
api_specs:
- filename: newscred-cmp-open-api-openapi.json
  format: json
  label: Optimizely CMP Open API v3
  slug: optimizely-cmp-open-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-cmp-open-api-openapi.json
- filename: newscred-welcome-open-api-openapi.yml
  format: yaml
  label: Welcome Open API v3 (legacy)
  slug: welcome-open-api-v3-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-welcome-open-api-openapi.yml
authorization_urls:
- https://accounts.cmp.optimizely.com/o/oauth2/v1/auth
description: ''
docs: https://docs.developers.optimizely.com/content-marketing-platform/docs/authentication-1
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Newscred Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Newscred publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Newscred API on a user''s behalf.


  Tokens are issued from https://accounts.cmp.optimizely.com/o/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Newscred
provider_slug: newscred
schemes:
- flows:
  - authorizationUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/auth
    flow: authorizationCode
    tokenUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/token
  - flow: clientCredentials
    tokenUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/token
  name: OAuth2
  source: openapi/newscred-cmp-open-api-openapi.json
scope_count: 3
scope_names:
- offline_access
- openid
- profile
scopes:
- description: Grants the ability to refresh access_token using the refresh token even when user is not present (not logged in).
  flows:
  - authorizationCode
  scope: offline_access
- description: Grants the ability to receive a unique identifier for the user.
  flows:
  - authorizationCode
  scope: openid
- description: Grants access to user profile information.
  flows:
  - authorizationCode
  scope: profile
slug: newscred-scopes
source_filename: newscred-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.developers.optimizely.com/content-marketing-platform/docs/authentication-1\nschemes:\n- name: OAuth2\n  source: openapi/newscred-cmp-open-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/auth\n    tokenUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://accounts.cmp.optimizely.com/o/oauth2/v1/token\nscopes:\n- scope: offline_access\n  description: Grants the ability to refresh access_token using the refresh token even when user is not present\n    (not logged in).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/newscred-cmp-open-api-openapi.json\n- scope: openid\n  description: Grants the ability to receive a unique identifier for the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/newscred-cmp-open-api-openapi.json\n- scope: profile\n  description: Grants\
  \ access to user profile information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/newscred-cmp-open-api-openapi.json\ndocs: https://docs.developers.optimizely.com/content-marketing-platform/docs/authentication-1\nderived_from: openapi/newscred-cmp-open-api-openapi.json\nscope_model:\n  granularity: coarse — identity scopes only\n  note: 'CMP publishes exactly three scopes and they are the OIDC identity trio: openid, profile and offline_access.\n    NONE of them scopes API capability. There is no read vs write scope, no per-resource scope (library, tasks,\n    campaigns, settings), and the clientCredentials flow declares an EMPTY scopes map. Authorization is therefore\n    decided entirely by the CMP organization permissions of the user or app, not by the token scope — which means\n    a consent screen cannot tell a user what an app will be able to do, and an agent cannot request least privilege.\n    The docs confirm all three must be sent, space-delimited, to the authorization\
  \ endpoint.'\n  documented_requirement: All three scopes must be passed to the authorization endpoint, delimited by a single space.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/scopes/newscred-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Company
- Content Marketing
- Content Management
- Digital Asset Management
- Marketing
- Marketing Resource Management
- Workflow
- Publishing
- Webhooks
- Acquired
token_urls:
- https://accounts.cmp.optimizely.com/o/oauth2/v1/token
---
