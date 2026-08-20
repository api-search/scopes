---
api_specs:
- filename: jebbit-auth-api-openapi.yml
  format: yaml
  label: Jebbit Auth API
  slug: jebbit-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-auth-api-openapi.yml
- filename: jebbit-businesses-api-openapi.yml
  format: yaml
  label: Jebbit Businesses API
  slug: jebbit-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-businesses-api-openapi.yml
- filename: jebbit-campaigns-api-openapi.yml
  format: yaml
  label: Jebbit Campaigns API
  slug: jebbit-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-campaigns-api-openapi.yml
- filename: jebbit-feed-columns-api-openapi.yml
  format: yaml
  label: Jebbit Feed Columns API
  slug: jebbit-feed-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-feed-columns-api-openapi.yml
- filename: jebbit-feed-rows-api-openapi.yml
  format: yaml
  label: Jebbit Feed Rows API
  slug: jebbit-feed-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-feed-rows-api-openapi.yml
- filename: jebbit-feeds-api-openapi.yml
  format: yaml
  label: Jebbit Feeds API
  slug: jebbit-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-feeds-api-openapi.yml
- filename: jebbit-integration-historic-backfills-api-openapi.yml
  format: yaml
  label: Jebbit Integration Historic Backfills API
  slug: jebbit-integration-historic-backfills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-integration-historic-backfills-api-openapi.yml
- filename: jebbit-integration-mappings-api-openapi.yml
  format: yaml
  label: Jebbit Integration Mappings API
  slug: jebbit-integration-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-integration-mappings-api-openapi.yml
- filename: jebbit-integrations-api-openapi.yml
  format: yaml
  label: Jebbit Integrations API
  slug: jebbit-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-integrations-api-openapi.yml
- filename: jebbit-launch-links-api-openapi.yml
  format: yaml
  label: Jebbit Launch Links API
  slug: jebbit-launch-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-launch-links-api-openapi.yml
authorization_urls: []
description: ''
docs: https://support-experiences.blueconic.com/en/articles/246971-api-overview
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Jebbit Scopes
name_suffix: OAuth Scopes
note: Tokens are minted by an Auth0 tenant (auth.jebbit.com) via the OAuth 2.0 client_credentials grant with audience "public-api". The OpenAPI models the bearer scheme as http/bearer but declares read/write/delete scopes; the docs token example returns finer-grained resource scopes.
overview: 'Jebbit publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jebbit API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jebbit
provider_slug: jebbit
schemes:
- audience: public-api
  flow: clientCredentials
  name: JWT (Auth0 client_credentials)
  source: openapi/jebbit-openapi-original.json
  tokenUrl: https://auth.jebbit.com/oauth/token
  type: oauth2
scope_count: 6
scope_names:
- read
- write
- delete
- read:business:{business_id}
- read:integration
- write:integration
scopes:
- description: Grants read access
  flows: []
  scope: read
- description: Grants write access
  flows: []
  scope: write
- description: Grants delete access
  flows: []
  scope: delete
- description: Read access scoped to a specific Jebbit business/account (observed in the docs token response).
  flows: []
  scope: read:business:{business_id}
- description: Read access to integrations (webhooks).
  flows: []
  scope: read:integration
- description: Create/update integrations (webhooks).
  flows: []
  scope: write:integration
slug: jebbit-scopes
source_filename: jebbit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/jebbit-openapi-original.json\ndocs: https://support-experiences.blueconic.com/en/articles/246971-api-overview\nnote: Tokens are minted by an Auth0 tenant (auth.jebbit.com) via the OAuth 2.0 client_credentials grant\n  with audience \"public-api\". The OpenAPI models the bearer scheme as http/bearer but declares read/write/delete\n  scopes; the docs token example returns finer-grained resource scopes.\nschemes:\n- name: JWT (Auth0 client_credentials)\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://auth.jebbit.com/oauth/token\n  audience: public-api\n  source: openapi/jebbit-openapi-original.json\nscopes:\n- scope: read\n  description: Grants read access\n  sources:\n  - openapi/jebbit-openapi-original.json\n- scope: write\n  description: Grants write access\n  sources:\n  - openapi/jebbit-openapi-original.json\n- scope: delete\n  description: Grants delete access\n  sources:\n  - openapi/jebbit-openapi-original.json\n\
  - scope: read:business:{business_id}\n  description: Read access scoped to a specific Jebbit business/account (observed in the docs token response).\n  sources:\n  - docs\n- scope: read:integration\n  description: Read access to integrations (webhooks).\n  sources:\n  - docs\n- scope: write:integration\n  description: Create/update integrations (webhooks).\n  sources:\n  - docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/scopes/jebbit-scopes.yml
summary_line: 6 scopes
tags:
- Company
- Interactive Experiences
- Zero-Party Data
- First-Party Data
- Marketing
- Quizzes
- Product Feeds
- Webhook
- Customer Data
- JSON:API
token_urls: []
---
