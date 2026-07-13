---
api_specs:
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Profiles API
  slug: memberclicks-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Profile Search API
  slug: memberclicks-profile-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Attributes API
  slug: memberclicks-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Member Types and Statuses API
  slug: memberclicks-member-types-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Groups API
  slug: memberclicks-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Events API
  slug: memberclicks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
- filename: memberclicks-openapi.yml
  format: yaml
  label: MemberClicks Continuing Education API
  slug: memberclicks-continuing-education-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/openapi/memberclicks-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Memberclicks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MemberClicks publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MemberClicks API on a user''s behalf.


  Tokens are issued from https://{orgId}.memberclicks.net/oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MemberClicks
provider_slug: memberclicks
schemes:
- description: OAuth 2.0. Obtain a bearer token from /oauth/v1/token using HTTP Basic client credentials (Base64 clientId:clientSecret) with scope read, write, or read write.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{orgId}.memberclicks.net/oauth/v1/token
  name: oauth2
  source: openapi/memberclicks-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to resources.
  flows:
  - clientCredentials
  scope: read
- description: Write access to resources.
  flows:
  - clientCredentials
  scope: write
slug: memberclicks-scopes
source_filename: memberclicks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/memberclicks-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/memberclicks-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{orgId}.memberclicks.net/oauth/v1/token\n  description: OAuth 2.0. Obtain a bearer token from /oauth/v1/token using HTTP Basic client\n    credentials (Base64 clientId:clientSecret) with scope read, write, or read write.\nscopes:\n- scope: read\n  description: Read access to resources.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/memberclicks-openapi.yml\n- scope: write\n  description: Write access to resources.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/memberclicks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memberclicks/refs/heads/main/scopes/memberclicks-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Membership Management
- Association Management
- AMS
- Nonprofit
- Events
- CRM
- Personify
token_urls:
- https://{orgId}.memberclicks.net/oauth/v1/token
---
