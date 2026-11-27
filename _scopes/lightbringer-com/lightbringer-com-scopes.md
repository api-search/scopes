---
api_specs:
- filename: lightbringer-com-oauth-api-openapi.yml
  format: yaml
  label: Lightbringer OAuth API
  slug: lightbringer-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lightbringer-com/openapi/lightbringer-com-oauth-api-openapi.yml
- filename: lightbringer-com-public-api-openapi.yml
  format: yaml
  label: Lightbringer Public API
  slug: lightbringer-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lightbringer-com/openapi/lightbringer-com-public-api-openapi.yml
- filename: lightbringer-com-well-known-api-openapi.yml
  format: yaml
  label: Lightbringer .well Known API
  slug: lightbringer-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lightbringer-com/openapi/lightbringer-com-well-known-api-openapi.yml
authorization_urls:
- https://app.lightbringer.com/api/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Lightbringer Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lightbringer publishes 31 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lightbringer API on a user''s behalf.


  Tokens are issued from https://app.lightbringer.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lightbringer
provider_slug: lightbringer-com
schemes:
- description: OAuth 2.1 authorization-code flow with PKCE (S256). Clients register dynamically (RFC 7591) or present a Client ID Metadata Document URL as client_id. Authorization requests must carry an RFC 8707 resource indicator. The mcp:* scopes are consentable directly; the granular scopes are minted through RFC 8693 token exchange against the token endpoint and enforced by the v1 API.
  flows:
  - authorizationUrl: https://app.lightbringer.com/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.lightbringer.com/api/oauth/token
  name: oauth2
  source: openapi/lightbringer-com-openapi.json
scope_count: 31
scope_names:
- delete:automated-tasks
- mcp:read
- mcp:write
- presence:token
- read:innovation-disclosures
- read:iprally-search
- read:organisation-settings
- read:prompts
- read:public-patents
- read:reviews
- read:strategies
- read:workflow-blueprints
- write:aurora-ticket
- write:comments
- write:document-collaboration
- write:image-generation
- write:innovation-disclosures
- write:knowledge-graph
- write:meeting-collaboration
- write:method-definition
- write:organisation-settings
- write:patent-draft
- write:patent-imports
- write:prosecution
- write:report-collaboration
- write:reviews
- write:skill-proposals
- write:strategies
- write:vault
- write:workflow-blueprints
- write:workflow-progress
scopes:
- description: Delete automated tasks resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: delete:automated-tasks
- description: Read your patent applications, documents, and prosecution data
  flows:
  - authorizationCode
  scope: mcp:read
- description: Create and edit patent applications, documents, and drafts
  flows:
  - authorizationCode
  scope: mcp:write
- description: Presence token resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: presence:token
- description: Read innovation disclosures resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: read:innovation-disclosures
- description: Read iprally search resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: read:iprally-search
- description: Read organisation settings resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: read:organisation-settings
- description: Read prompts resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: read:prompts
- description: Read public patents resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: read:public-patents
- description: Read reviews resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: read:reviews
- description: Read strategies resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: read:strategies
- description: Read workflow blueprints resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: read:workflow-blueprints
- description: Write aurora ticket resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:aurora-ticket
- description: Write comments resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:comments
- description: Write document collaboration resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:document-collaboration
- description: Write image generation resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:image-generation
- description: Write innovation disclosures resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:innovation-disclosures
- description: Write knowledge graph resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:knowledge-graph
- description: Write meeting collaboration resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:meeting-collaboration
- description: Write method definition resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:method-definition
- description: Write organisation settings resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:organisation-settings
- description: Write patent draft resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:patent-draft
- description: Write patent imports resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:patent-imports
- description: Write prosecution resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:prosecution
- description: Write report collaboration resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:report-collaboration
- description: Write reviews resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:reviews
- description: Write skill proposals resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:skill-proposals
- description: Write strategies resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:strategies
- description: Write vault resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:vault
- description: Write workflow blueprints resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:workflow-blueprints
- description: Write workflow progress resources (issued via RFC 8693 token exchange)
  flows:
  - authorizationCode
  scope: write:workflow-progress
slug: lightbringer-com-scopes
source_filename: lightbringer-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/lightbringer-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/lightbringer-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.lightbringer.com/api/oauth/authorize\n    tokenUrl: https://app.lightbringer.com/api/oauth/token\n  description: OAuth 2.1 authorization-code flow with PKCE (S256). Clients register dynamically\n    (RFC 7591) or present a Client ID Metadata Document URL as client_id. Authorization requests\n    must carry an RFC 8707 resource indicator. The mcp:* scopes are consentable directly; the\n    granular scopes are minted through RFC 8693 token exchange against the token endpoint and\n    enforced by the v1 API.\nscopes:\n- scope: delete:automated-tasks\n  description: Delete automated tasks resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: mcp:read\n  description:\
  \ Read your patent applications, documents, and prosecution data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: mcp:write\n  description: Create and edit patent applications, documents, and drafts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: presence:token\n  description: Presence token resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: read:innovation-disclosures\n  description: Read innovation disclosures resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: read:iprally-search\n  description: Read iprally search resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: read:organisation-settings\n  description: Read\
  \ organisation settings resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: read:prompts\n  description: Read prompts resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: read:public-patents\n  description: Read public patents resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: read:reviews\n  description: Read reviews resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: read:strategies\n  description: Read strategies resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: read:workflow-blueprints\n  description: Read workflow blueprints\
  \ resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:aurora-ticket\n  description: Write aurora ticket resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:comments\n  description: Write comments resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:document-collaboration\n  description: Write document collaboration resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:image-generation\n  description: Write image generation resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:innovation-disclosures\n  description:\
  \ Write innovation disclosures resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:knowledge-graph\n  description: Write knowledge graph resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:meeting-collaboration\n  description: Write meeting collaboration resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:method-definition\n  description: Write method definition resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:organisation-settings\n  description: Write organisation settings resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n\
  - scope: write:patent-draft\n  description: Write patent draft resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:patent-imports\n  description: Write patent imports resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:prosecution\n  description: Write prosecution resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:report-collaboration\n  description: Write report collaboration resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:reviews\n  description: Write reviews resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n\
  - scope: write:skill-proposals\n  description: Write skill proposals resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:strategies\n  description: Write strategies resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:vault\n  description: Write vault resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:workflow-blueprints\n  description: Write workflow blueprints resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n- scope: write:workflow-progress\n  description: Write workflow progress resources (issued via RFC 8693 token exchange)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightbringer-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lightbringer-com/scopes/lightbringer-com-scopes.yml
summary_line: 31 scopes · authorizationCode
tags:
- Artificial Intelligence
- Patents
- Deep Tech
- Startups
- Platform
token_bound: false
token_urls:
- https://app.lightbringer.com/api/oauth/token
---
