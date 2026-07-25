---
api_specs:
- filename: typeface-audiences-api-openapi.yml
  format: yaml
  label: Typeface Audiences API
  slug: typeface-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-audiences-api-openapi.yml
- filename: typeface-authentication-api-openapi.yml
  format: yaml
  label: Typeface Authentication API
  slug: typeface-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-authentication-api-openapi.yml
- filename: typeface-basic-services-api-openapi.yml
  format: yaml
  label: Typeface Basic Services API
  slug: typeface-basic-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-basic-services-api-openapi.yml
- filename: typeface-brand-kits-api-openapi.yml
  format: yaml
  label: Typeface Brand Kits API
  slug: typeface-brand-kits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-brand-kits-api-openapi.yml
- filename: typeface-content-generation-api-openapi.yml
  format: yaml
  label: Typeface Content Generation API
  slug: typeface-content-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-content-generation-api-openapi.yml
- filename: typeface-content-service-api-openapi.yml
  format: yaml
  label: Typeface Content Service API
  slug: typeface-content-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-content-service-api-openapi.yml
- filename: typeface-digital-assets-api-openapi.yml
  format: yaml
  label: Typeface Digital Assets API
  slug: typeface-digital-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-digital-assets-api-openapi.yml
- filename: typeface-discovery-api-openapi.yml
  format: yaml
  label: Typeface Discovery API
  slug: typeface-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-discovery-api-openapi.yml
- filename: typeface-feeds-api-openapi.yml
  format: yaml
  label: Typeface Feeds API
  slug: typeface-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-feeds-api-openapi.yml
- filename: typeface-profile-service-api-openapi.yml
  format: yaml
  label: Typeface Profile Service API
  slug: typeface-profile-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-profile-service-api-openapi.yml
- filename: typeface-projects-api-openapi.yml
  format: yaml
  label: Typeface Projects API
  slug: typeface-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-projects-api-openapi.yml
- filename: typeface-provisioning-api-openapi.yml
  format: yaml
  label: Typeface Provisioning API
  slug: typeface-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-provisioning-api-openapi.yml
- filename: typeface-provisioning-service-api-openapi.yml
  format: yaml
  label: Typeface Provisioning Service API
  slug: typeface-provisioning-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-provisioning-service-api-openapi.yml
- filename: typeface-search-service-api-openapi.yml
  format: yaml
  label: Typeface Search Service API
  slug: typeface-search-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-search-service-api-openapi.yml
- filename: typeface-tag-library-api-openapi.yml
  format: yaml
  label: Typeface Tag Library API
  slug: typeface-tag-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-tag-library-api-openapi.yml
authorization_urls:
- https://auth-us.typeface.ai/authorize
description: ''
docs: https://developers.typeface.ai/docs/oauth-21-authorization-code-flow-for-typeface-mcp-apis
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Typeface Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Typeface publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Typeface API on a user''s behalf.


  Tokens are issued from https://api-us.typeface.ai/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Typeface
provider_slug: typeface
schemes:
- flows:
  - authorizationUrl: https://auth-us.typeface.ai/authorize
    flow: authorizationCode
    tokenUrl: https://api-us.typeface.ai/mcp/oauth/token
  name: mcpOAuth
  source: https://developers.typeface.ai/docs/oauth-21-authorization-code-flow-for-typeface-mcp-apis
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email claim.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
slug: typeface-scopes
source_filename: typeface-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.typeface.ai/docs/oauth-21-authorization-code-flow-for-typeface-mcp-apis\ndocs: https://developers.typeface.ai/docs/oauth-21-authorization-code-flow-for-typeface-mcp-apis\nnotes: The core REST API uses bearer JWTs from application credentials (no\n  scope surface documented). The documented scope set below applies to the\n  OAuth 2.1 authorization-code flow (with PKCE) for the Typeface MCP server and\n  MCP APIs; the discovery document at\n  https://api-us.typeface.ai/.well-known/oauth-authorization-server lists\n  supported scopes and grant types.\nschemes:\n  - name: mcpOAuth\n    source: https://developers.typeface.ai/docs/oauth-21-authorization-code-flow-for-typeface-mcp-apis\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth-us.typeface.ai/authorize\n        tokenUrl: https://api-us.typeface.ai/mcp/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect\
  \ authentication.\n    flows: [authorizationCode]\n  - scope: profile\n    description: Access to the user's profile claims.\n    flows: [authorizationCode]\n  - scope: email\n    description: Access to the user's email claim.\n    flows: [authorizationCode]\n  - scope: offline_access\n    description: Issue a refresh token for long-lived access.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/scopes/typeface-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Ai
- Artificial Intelligence
- Content Generation
- Marketing
- Agents
- Generative AI
- Brand Management
- Enterprise
token_urls:
- https://api-us.typeface.ai/mcp/oauth/token
---
