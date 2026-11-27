---
api_specs:
- filename: casatoo-pt-account-api-openapi.yml
  format: yaml
  label: Casatoo Account API
  slug: casatoo-pt-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casatoo-pt/openapi/casatoo-pt-account-api-openapi.yml
- filename: casatoo-pt-likes-api-openapi.yml
  format: yaml
  label: Casatoo Likes API
  slug: casatoo-pt-likes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casatoo-pt/openapi/casatoo-pt-likes-api-openapi.yml
- filename: casatoo-pt-listings-api-openapi.yml
  format: yaml
  label: Casatoo Listings API
  slug: casatoo-pt-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casatoo-pt/openapi/casatoo-pt-listings-api-openapi.yml
- filename: casatoo-pt-locations-api-openapi.yml
  format: yaml
  label: Casatoo Locations API
  slug: casatoo-pt-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casatoo-pt/openapi/casatoo-pt-locations-api-openapi.yml
- filename: casatoo-pt-saved-searches-api-openapi.yml
  format: yaml
  label: Casatoo Saved searches API
  slug: casatoo-pt-saved-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casatoo-pt/openapi/casatoo-pt-saved-searches-api-openapi.yml
authorization_urls:
- https://oauth.casatoo.pt/oauth2/auth
description: ''
docs: https://casatoo.pt/developers/agents#scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Casatoo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Casatoo publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Casatoo API on a user''s behalf.


  Tokens are issued from https://oauth.casatoo.pt/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Casatoo
provider_slug: casatoo-pt
schemes:
- description: Authorization code grants delegated human access.
  flows:
  - authorizationUrl: https://oauth.casatoo.pt/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth.casatoo.pt/oauth2/token
  name: casatooOAuth
  source: openapi/casatoo-pt-openapi.yml
scope_count: 8
scope_names:
- casatoo:read
- casatoo:write
- likes:read
- likes:write
- listings:read
- locations:read
- saved-searches:read
- saved-searches:write
scopes:
- description: Compatibility alias for all supported read scopes.
  flows:
  - authorizationCode
  scope: casatoo:read
- description: Compatibility alias for all supported write scopes.
  flows:
  - authorizationCode
  scope: casatoo:write
- description: Read listing likes owned by the principal.
  flows:
  - authorizationCode
  scope: likes:read
- description: Create or remove listing likes for the principal.
  flows:
  - authorizationCode
  scope: likes:write
- description: Read listing search results, detail, and comparisons.
  flows:
  - authorizationCode
  scope: listings:read
- description: Resolve supported Portuguese locations.
  flows:
  - authorizationCode
  scope: locations:read
- description: Read saved searches owned by the principal.
  flows:
  - authorizationCode
  scope: saved-searches:read
- description: Create, update, or delete saved searches for the principal.
  flows:
  - authorizationCode
  scope: saved-searches:write
slug: casatoo-pt-scopes
source_filename: casatoo-pt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://casatoo.pt/developers/agents\nschemes:\n- name: casatooOAuth\n  source: openapi/casatoo-pt-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.casatoo.pt/oauth2/auth\n    tokenUrl: https://oauth.casatoo.pt/oauth2/token\n  description: Authorization code grants delegated human access.\nscopes:\n- scope: casatoo:read\n  description: Compatibility alias for all supported read scopes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/casatoo-pt-openapi.yml\n- scope: casatoo:write\n  description: Compatibility alias for all supported write scopes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/casatoo-pt-openapi.yml\n- scope: likes:read\n  description: Read listing likes owned by the principal.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/casatoo-pt-openapi.yml\n- scope: likes:write\n  description: Create or remove listing likes for the principal.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/casatoo-pt-openapi.yml\n- scope: listings:read\n  description: Read listing search results, detail, and comparisons.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/casatoo-pt-openapi.yml\n- scope: locations:read\n  description: Resolve supported Portuguese locations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/casatoo-pt-openapi.yml\n- scope: saved-searches:read\n  description: Read saved searches owned by the principal.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/casatoo-pt-openapi.yml\n- scope: saved-searches:write\n  description: Create, update, or delete saved searches for the principal.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/casatoo-pt-openapi.yml\ndocs: https://casatoo.pt/developers/agents#scopes\nderived_from: openapi/casatoo-pt-openapi.yml\nnotes: casatoo:read / casatoo:write are compatibility aliases for supported read/write\n  scopes; new integrations should request granular\
  \ scopes instead. Public listing\n  and location reads require no scope at all. Authorization server also lists openid,\n  profile, email, offline_access.\n"
source_yaml_url: https://artifacts.apis.io/casatoo-pt/scopes/casatoo-pt-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Company
- Real Estate
- Property Search
- Portugal
- Price-Tracking
- Mortgage
- MCP
- AI Agents
token_bound: false
token_urls:
- https://oauth.casatoo.pt/oauth2/token
---
