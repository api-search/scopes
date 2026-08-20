---
api_specs:
- filename: zeplin-authorization-api-openapi.yml
  format: yaml
  label: Zeplin Authorization API
  slug: zeplin-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-authorization-api-openapi.yml
- filename: zeplin-colors-api-openapi.yml
  format: yaml
  label: Zeplin Colors API
  slug: zeplin-colors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-colors-api-openapi.yml
- filename: zeplin-components-api-openapi.yml
  format: yaml
  label: Zeplin Components API
  slug: zeplin-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-components-api-openapi.yml
- filename: zeplin-connected-components-api-openapi.yml
  format: yaml
  label: Zeplin Connected Components API
  slug: zeplin-connected-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-connected-components-api-openapi.yml
- filename: zeplin-design-tokens-api-openapi.yml
  format: yaml
  label: Zeplin Design Tokens API
  slug: zeplin-design-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-design-tokens-api-openapi.yml
- filename: zeplin-flows-api-openapi.yml
  format: yaml
  label: Zeplin Flows API
  slug: zeplin-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-flows-api-openapi.yml
- filename: zeplin-notifications-api-openapi.yml
  format: yaml
  label: Zeplin Notifications API
  slug: zeplin-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-notifications-api-openapi.yml
- filename: zeplin-organizations-api-openapi.yml
  format: yaml
  label: Zeplin Organizations API
  slug: zeplin-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-organizations-api-openapi.yml
- filename: zeplin-projects-api-openapi.yml
  format: yaml
  label: Zeplin Projects API
  slug: zeplin-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-projects-api-openapi.yml
- filename: zeplin-screens-api-openapi.yml
  format: yaml
  label: Zeplin Screens API
  slug: zeplin-screens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-screens-api-openapi.yml
- filename: zeplin-spacing-api-openapi.yml
  format: yaml
  label: Zeplin Spacing API
  slug: zeplin-spacing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-spacing-api-openapi.yml
- filename: zeplin-styleguides-api-openapi.yml
  format: yaml
  label: Zeplin Styleguides API
  slug: zeplin-styleguides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-styleguides-api-openapi.yml
- filename: zeplin-textstyles-api-openapi.yml
  format: yaml
  label: Zeplin TextStyles API
  slug: zeplin-textstyles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-textstyles-api-openapi.yml
- filename: zeplin-users-api-openapi.yml
  format: yaml
  label: Zeplin Users API
  slug: zeplin-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-users-api-openapi.yml
- filename: zeplin-variable-collections-api-openapi.yml
  format: yaml
  label: Zeplin Variable Collections API
  slug: zeplin-variable-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-variable-collections-api-openapi.yml
- filename: zeplin-webhooks-api-openapi.yml
  format: yaml
  label: Zeplin Webhooks API
  slug: zeplin-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/openapi/zeplin-webhooks-api-openapi.yml
authorization_urls:
- /v1/oauth/authorize
description: ''
docs: https://docs.zeplin.dev/reference/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zeplin Scopes
name_suffix: OAuth Scopes
note: Zeplin's OAuth 2.0 (authorization code with PKCE) does not use or document granular scopes; the authorize endpoint accepts no scope parameter and authorized apps get broad read/write access on behalf of the user (https://docs.zeplin.dev/reference/authentication).
overview: 'Zeplin uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zeplin
provider_slug: zeplin
schemes:
- flows:
  - authorizationUrl: /v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: /v1/oauth/token
  name: OAuth2
  source: openapi/zeplin-zeplin-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: zeplin-scopes
source_filename: zeplin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zeplin-zeplin-api-openapi.yml\ndocs: https://docs.zeplin.dev/reference/authentication\nnote: Zeplin's OAuth 2.0 (authorization code with PKCE) does not use or document\n  granular scopes; the authorize endpoint accepts no scope parameter and authorized\n  apps get broad read/write access on behalf of the user\n  (https://docs.zeplin.dev/reference/authentication).\nschemes:\n- name: OAuth2\n  source: openapi/zeplin-zeplin-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/oauth/authorize\n    tokenUrl: /v1/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/scopes/zeplin-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Design
- Design Handoff
- Developer Tools
- Figma
- Sketch
- Adobe XD
- Style Guides
- Components
- Assets
- Webhook
token_urls:
- /v1/oauth/token
---
