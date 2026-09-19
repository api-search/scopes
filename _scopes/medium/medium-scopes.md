---
api_specs:
- filename: medium-authorization-api-openapi.yml
  format: yaml
  label: medium Authorization API
  slug: medium-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-authorization-api-openapi.yml
- filename: medium-images-api-openapi.yml
  format: yaml
  label: medium Images API
  slug: medium-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-images-api-openapi.yml
- filename: medium-posts-api-openapi.yml
  format: yaml
  label: medium Posts API
  slug: medium-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-posts-api-openapi.yml
- filename: medium-publications-api-openapi.yml
  format: yaml
  label: medium Publications API
  slug: medium-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-publications-api-openapi.yml
- filename: medium-tokens-api-openapi.yml
  format: yaml
  label: medium Tokens API
  slug: medium-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-tokens-api-openapi.yml
- filename: medium-users-api-openapi.yml
  format: yaml
  label: medium Users API
  slug: medium-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-users-api-openapi.yml
authorization_urls: []
description: 'OAuth2 scopes for Medium''s browser-based authorization flow, read from the scope table in section 2.2 of Medium''s own API documentation. Note that derive-oauth-scopes.py finds NOTHING in the repository''s OpenAPIs — none of the six refined specs declares an oauth2 securityScheme, so this artifact could only come from the docs. Scope grants are closed to new integrations: Medium states it does not allow new integrations, and the flow is "supported for existing integrations only".'
docs: https://github.com/Medium/medium-api-docs#22-browser-based-authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Medium Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Medium uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Medium
provider_slug: medium
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: medium-scopes
source_filename: medium-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://github.com/Medium/medium-api-docs#22-browser-based-authentication\ndocs: https://github.com/Medium/medium-api-docs#22-browser-based-authentication\ndescription: >-\n  OAuth2 scopes for Medium's browser-based authorization flow, read from the scope table in section\n  2.2 of Medium's own API documentation. Note that derive-oauth-scopes.py finds NOTHING in the\n  repository's OpenAPIs — none of the six refined specs declares an oauth2 securityScheme, so this\n  artifact could only come from the docs. Scope grants are closed to new integrations: Medium states\n  it does not allow new integrations, and the flow is \"supported for existing integrations only\".\nflow:\n  type: authorization_code\n  authorization_url: https://medium.com/m/oauth/authorize\n  token_url: https://api.medium.com/v1/tokens\n  refresh_url: https://api.medium.com/v1/tokens\n  scope_delimiter: ','\n  note: >-\n    Scopes are passed comma-separated\
  \ in the `scope` query parameter, not space-separated as RFC\n    6749 section 3.3 specifies. Access tokens are valid for 60 days; refresh tokens do not expire.\n    Self-issued integration tokens (the recommended path) carry no scope selection at all.\nsummary:\n  scope_count: 4\n  extended_count: 1\nscopes:\n- name: basicProfile\n  description: Grants basic access to a user's profile (not including their email).\n  extended: false\n  operations:\n  - getAuthenticatedUser\n- name: listPublications\n  description: Grants the ability to list publications related to the user.\n  extended: false\n  operations:\n  - listUserPublications\n- name: publishPost\n  description: Grants the ability to publish a post to the user's profile.\n  extended: false\n  operations:\n  - createUserPost\n  - createPublicationPost\n- name: uploadImage\n  description: Grants the ability to upload an image for use within a Medium post.\n  extended: true\n  operations:\n  - uploadImage\n  note: >-\n    Extended\
  \ scope. Medium's docs state integrations are not permitted to request extended scope\n    without explicit prior permission from Medium, and that requesting it through the standard flow\n    errors if the integration has not been authorized for it.\nrecommended_default:\n- basicProfile\n- publishPost\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/scopes/medium-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Publishing
- Content
- Blogging
- Media
- Social
- Writing
- Authentication
- Deprecated API
token_urls: []
---
