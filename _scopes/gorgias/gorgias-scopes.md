---
api_specs:
- filename: gorgias-asyncapi.yml
  format: yaml
  label: Gorgias Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/asyncapi/gorgias-asyncapi.yml
- filename: gorgias-account-api-openapi.yml
  format: yaml
  label: Gorgias Account API
  slug: gorgias-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-account-api-openapi.yml
- filename: gorgias-customers-api-openapi.yml
  format: yaml
  label: Gorgias Customers API
  slug: gorgias-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-customers-api-openapi.yml
- filename: gorgias-integrations-api-openapi.yml
  format: yaml
  label: Gorgias Integrations API
  slug: gorgias-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-integrations-api-openapi.yml
- filename: gorgias-macros-api-openapi.yml
  format: yaml
  label: Gorgias Macros API
  slug: gorgias-macros-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-macros-api-openapi.yml
- filename: gorgias-messages-api-openapi.yml
  format: yaml
  label: Gorgias Messages API
  slug: gorgias-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-messages-api-openapi.yml
- filename: gorgias-rules-api-openapi.yml
  format: yaml
  label: Gorgias Rules API
  slug: gorgias-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-rules-api-openapi.yml
- filename: gorgias-surveys-api-openapi.yml
  format: yaml
  label: Gorgias Surveys API
  slug: gorgias-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-surveys-api-openapi.yml
- filename: gorgias-tags-api-openapi.yml
  format: yaml
  label: Gorgias Tags API
  slug: gorgias-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-tags-api-openapi.yml
- filename: gorgias-teams-api-openapi.yml
  format: yaml
  label: Gorgias Teams API
  slug: gorgias-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-teams-api-openapi.yml
- filename: gorgias-tickets-api-openapi.yml
  format: yaml
  label: Gorgias Tickets API
  slug: gorgias-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-tickets-api-openapi.yml
- filename: gorgias-users-api-openapi.yml
  format: yaml
  label: Gorgias Users API
  slug: gorgias-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-users-api-openapi.yml
- filename: gorgias-views-api-openapi.yml
  format: yaml
  label: Gorgias Views API
  slug: gorgias-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-views-api-openapi.yml
- filename: gorgias-widgets-api-openapi.yml
  format: yaml
  label: Gorgias Widgets API
  slug: gorgias-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-widgets-api-openapi.yml
authorization_urls:
- https://{account}.gorgias.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Gorgias Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Gorgias publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gorgias API on a user''s behalf.


  Tokens are issued from https://{account}.gorgias.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gorgias
provider_slug: gorgias
schemes:
- flows:
  - authorizationUrl: https://{account}.gorgias.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{account}.gorgias.com/oauth/token
  name: oauth2
  source: openapi/gorgias-openapi.yml
scope_count: 6
scope_names:
- accounts.read
- customers.read
- customers.write
- openid
- tickets.read
- tickets.write
scopes:
- description: Read account
  flows:
  - authorizationCode
  scope: accounts.read
- description: Read customers
  flows:
  - authorizationCode
  scope: customers.read
- description: Write customers
  flows:
  - authorizationCode
  scope: customers.write
- description: OpenID
  flows:
  - authorizationCode
  scope: openid
- description: Read tickets
  flows:
  - authorizationCode
  scope: tickets.read
- description: Write tickets
  flows:
  - authorizationCode
  scope: tickets.write
slug: gorgias-scopes
source_filename: gorgias-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gorgias-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/gorgias-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{account}.gorgias.com/oauth/authorize\n    tokenUrl: https://{account}.gorgias.com/oauth/token\nscopes:\n- scope: accounts.read\n  description: Read account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gorgias-openapi.yml\n- scope: customers.read\n  description: Read customers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gorgias-openapi.yml\n- scope: customers.write\n  description: Write customers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gorgias-openapi.yml\n- scope: openid\n  description: OpenID\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gorgias-openapi.yml\n- scope: tickets.read\n  description: Read tickets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gorgias-openapi.yml\n- scope: tickets.write\n\
  \  description: Write tickets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/gorgias-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/scopes/gorgias-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Customer-Support
- Help Desk
- E-Commerce
- Shopify
- Tickets
- Conversations
token_urls:
- https://{account}.gorgias.com/oauth/token
---
