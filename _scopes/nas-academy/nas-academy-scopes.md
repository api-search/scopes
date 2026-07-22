---
api_specs:
- filename: nas-academy-openapi-original.json
  format: json
  label: Nas.com Public Discovery API
  slug: nascom-public-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nas-academy/refs/heads/main/openapi/nas-academy-openapi-original.json
authorization_urls:
- https://auth.nas.com/oauth/authorize
description: ''
docs: https://nas.com/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nas Academy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nas.com (Nas Academy) publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nas.com (Nas Academy) API on a user''s behalf.


  Tokens are issued from https://auth.nas.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nas.com (Nas Academy)
provider_slug: nas-academy
schemes:
- flows:
  - authorizationUrl: https://auth.nas.com/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    registrationUrl: https://auth.nas.com/oauth/register
    revocationUrl: https://auth.nas.com/oauth/revoke
    tokenUrl: https://auth.nas.com/oauth/token
  issuer: https://auth.nas.com
  name: OAuth2
  source: https://auth.nas.io/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 6
scope_names:
- nas.communities.read
- nas.communities.write
- nas.members.read
- nas.products.read
- nas.products.write
- nas.orders.read
scopes:
- description: Read access to communities managed by the authenticated Nas user.
  flows: []
  scope: nas.communities.read
- description: Write access to communities managed by the authenticated Nas user.
  flows: []
  scope: nas.communities.write
- description: Read access to community members. Required by the list_members MCP tool.
  flows: []
  scope: nas.members.read
- description: Read access to products in a community.
  flows: []
  scope: nas.products.read
- description: Write access to products in a community.
  flows: []
  scope: nas.products.write
- description: Read access to physical product orders. Required by the list_physical_product_orders and get_physical_product_order MCP tools.
  flows: []
  scope: nas.orders.read
slug: nas-academy-scopes
source_filename: nas-academy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://auth.nas.io/.well-known/oauth-authorization-server\ndocs: https://nas.com/auth.md\nschemes:\n  - name: OAuth2\n    type: oauth2\n    source: https://auth.nas.io/.well-known/oauth-authorization-server\n    issuer: https://auth.nas.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.nas.com/oauth/authorize\n        tokenUrl: https://auth.nas.com/oauth/token\n        registrationUrl: https://auth.nas.com/oauth/register\n        revocationUrl: https://auth.nas.com/oauth/revoke\n        pkce: S256\n        grant_types: [authorization_code, refresh_token]\nscopes:\n  - scope: nas.communities.read\n    description: Read access to communities managed by the authenticated Nas user.\n  - scope: nas.communities.write\n    description: Write access to communities managed by the authenticated Nas user.\n  - scope: nas.members.read\n    description: Read access to community members. Required by\
  \ the list_members MCP tool.\n  - scope: nas.products.read\n    description: Read access to products in a community.\n  - scope: nas.products.write\n    description: Write access to products in a community.\n  - scope: nas.orders.read\n    description: Read access to physical product orders. Required by the list_physical_product_orders and get_physical_product_order MCP tools.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nas-academy/refs/heads/main/scopes/nas-academy-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Creator Economy
- Community
- E-commerce
- AI
- Agents
- MCP
- Online Courses
- Sellers
token_urls:
- https://auth.nas.com/oauth/token
---
