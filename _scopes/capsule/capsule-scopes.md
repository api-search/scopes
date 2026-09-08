---
api_specs:
- filename: capsule-opportunities-api-openapi.yml
  format: yaml
  label: Capsule Opportunities API
  slug: capsule-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-opportunities-api-openapi.yml
- filename: capsule-parties-api-openapi.yml
  format: yaml
  label: Capsule Parties API
  slug: capsule-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-parties-api-openapi.yml
- filename: capsule-projects-api-openapi.yml
  format: yaml
  label: Capsule Projects API
  slug: capsule-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-projects-api-openapi.yml
- filename: capsule-tasks-api-openapi.yml
  format: yaml
  label: Capsule Tasks API
  slug: capsule-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/openapi/capsule-tasks-api-openapi.yml
authorization_urls: []
description: OAuth 2.0 scopes Capsule advertises. The authoritative list is scopes_supported in the served OAuth Authorization Server Metadata document (RFC 8414) on the API host; the authentication docs page documents only the three combinations an application is expected to request. Both are recorded, and where they disagree the discovery document wins.
docs: https://developer.capsulecrm.com/v2/overview/authentication
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Capsule Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Capsule uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Capsule
provider_slug: capsule
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: capsule-scopes
source_filename: capsule-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://api.capsulecrm.com/.well-known/oauth-authorization-server\ndocs: https://developer.capsulecrm.com/v2/overview/authentication\ndescription: >-\n  OAuth 2.0 scopes Capsule advertises. The authoritative list is\n  scopes_supported in the served OAuth Authorization Server Metadata document\n  (RFC 8414) on the API host; the authentication docs page documents only the\n  three combinations an application is expected to request. Both are recorded,\n  and where they disagree the discovery document wins.\nauthorization_server: https://api.capsulecrm.com\nauthorization_endpoint: https://api.capsulecrm.com/oauth/authorise\ntoken_endpoint: https://api.capsulecrm.com/oauth/token\nflows:\n- authorization_code\nscope_delimiter: space\nscopes:\n- {name: read, description: 'Read-only access to Capsule data.', source: discovery+docs}\n- {name: write, description: 'Create, update and delete Capsule data. Requested alongside read.', source:\
  \ discovery+docs}\n- {name: user_preference, description: 'Access to the authenticated user''s preferences.', source: discovery+docs}\n- {name: openid, description: 'OpenID Connect - request an ID token.', source: discovery}\n- {name: profile, description: 'OIDC profile claims (name, given_name, family_name, locale, updated_at).', source: discovery}\n- {name: email, description: 'OIDC email claim.', source: discovery}\n- {name: tenant, description: 'Capsule tenant/subdomain claim identifying which Capsule account the token belongs to.', source: discovery}\nscope_count: 7\ndocumented_combinations:\n- {value: 'read', meaning: Read-only access}\n- {value: 'read write', meaning: Full read and write. The default an application receives.}\n- {value: 'read write user_preference', meaning: Read, write and user preferences.}\nnotes:\n- >-\n  The docs page presents scopes as three fixed combinations rather than a\n  composable set; the discovery document exposes seven individual values,\n  including\
  \ the four OIDC ones the docs never mention.\n- >-\n  Capsule publishes no per-operation scope mapping. Which endpoints require\n  write versus user_preference is not documented, so an agent cannot compute\n  least-privilege from the contract.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capsule/refs/heads/main/scopes/capsule-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Contact Management
- CRM
- Custom Fields
- Opportunities
- Pipelines
- Project Management
- REST
- Sales
- Task
- Webhook
token_urls: []
---
