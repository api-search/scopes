---
api_specs:
- filename: justidea-agency-agents-api-openapi.yml
  format: yaml
  label: JustIdea Agents API
  slug: justidea-agency-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-agents-api-openapi.yml
- filename: justidea-agency-contact-api-openapi.yml
  format: yaml
  label: JustIdea Contact API
  slug: justidea-agency-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-contact-api-openapi.yml
- filename: justidea-agency-content-api-openapi.yml
  format: yaml
  label: JustIdea Content API
  slug: justidea-agency-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-content-api-openapi.yml
- filename: justidea-agency-meta-api-openapi.yml
  format: yaml
  label: JustIdea Meta API
  slug: justidea-agency-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-meta-api-openapi.yml
- filename: justidea-agency-offer-api-openapi.yml
  format: yaml
  label: JustIdea Offer API
  slug: justidea-agency-offer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-offer-api-openapi.yml
authorization_urls:
- https://justidea.agency/oauth/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: JustIdea Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'JustIdea publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the JustIdea API on a user''s behalf.


  Tokens are issued from https://justidea.agency/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: JustIdea
provider_slug: justidea-agency
schemes:
- description: Optional. Identifies the agent and raises the rate limit to 600 requests per minute. Dynamic client registration and anonymous agent registration are described at https://justidea.agency/auth.md.
  flows:
  - authorizationUrl: https://justidea.agency/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://justidea.agency/oauth/token/
  name: agentOAuth
  source: openapi/justidea-agency-openapi.json
- description: Optional. Identifies the agent and raises the rate limit to 600 requests per minute. Dynamic client registration and anonymous agent registration are described at https://justidea.agency/auth.md.
  flows:
  - authorizationUrl: https://justidea.agency/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://justidea.agency/oauth/token/
  name: agentOAuth
  source: openapi/justidea-agency-openapi.yml
scope_count: 1
scope_names:
- site:read
scopes:
- description: Read public content of justidea.agency (REST API and MCP server).
  flows:
  - authorizationCode
  scope: site:read
slug: justidea-agency-scopes
source_filename: justidea-agency-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/justidea-agency-openapi.json, openapi/justidea-agency-openapi.yml\nschemes:\n- name: agentOAuth\n  source: openapi/justidea-agency-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://justidea.agency/oauth/authorize/\n    tokenUrl: https://justidea.agency/oauth/token/\n  description: Optional. Identifies the agent and raises the rate limit to 600 requests per\n    minute. Dynamic client registration and anonymous agent registration are described at https://justidea.agency/auth.md.\n- name: agentOAuth\n  source: openapi/justidea-agency-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://justidea.agency/oauth/authorize/\n    tokenUrl: https://justidea.agency/oauth/token/\n  description: Optional. Identifies the agent and raises the rate limit to 600 requests per\n    minute. Dynamic client registration and anonymous agent registration are described at https://justidea.agency/auth.md.\n\
  scopes:\n- scope: site:read\n  description: Read public content of justidea.agency (REST API and MCP server).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justidea-agency-openapi.json\n  - openapi/justidea-agency-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/justidea-agency/scopes/justidea-agency-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- E-Commerce
- Agency
- Poland
- PrestaShop
- WooCommerce
token_bound: false
token_urls:
- https://justidea.agency/oauth/token/
---
