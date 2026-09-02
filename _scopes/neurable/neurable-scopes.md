---
api_specs:
- filename: neurable-core-api-openapi.yml
  format: yaml
  label: Neurable Core API
  slug: neurable-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-core-api-openapi.yml
- filename: neurable-oauth-api-openapi.yml
  format: yaml
  label: Neurable O Auth API
  slug: neurable-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-oauth-api-openapi.yml
- filename: neurable-oidc-api-openapi.yml
  format: yaml
  label: Neurable OIDC API
  slug: neurable-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-oidc-api-openapi.yml
- filename: neurable-open-api-openapi.yml
  format: yaml
  label: Neurable Open API
  slug: neurable-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-open-api-openapi.yml
- filename: neurable-protected-api-openapi.yml
  format: yaml
  label: Neurable Protected API
  slug: neurable-protected-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-protected-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Neurable Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Neurable publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Neurable API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Neurable
provider_slug: neurable
schemes: []
scope_count: 5
scope_names:
- openid
- email
- demos:all:read
- demos:prime:read
- session:stream:create
scopes:
- description: Standard OpenID Connect scope; requests an ID token from the pipe issuer.
  flows: []
  scope: openid
- description: Standard OpenID Connect scope; releases the `email` claim, which the discovery document lists in claims_supported and which the /oidc/userinfo response carries.
  flows: []
  scope: email
- description: Read access to the full set of Neurable demo experiences. A demos.neurable.com host is live and serves a single-page application, which is the surface this scope appears to govern.
  flows: []
  scope: demos:all:read
- description: Read access to a restricted "prime" subset of the demo experiences — a narrower grant than demos:all:read.
  flows: []
  scope: demos:prime:read
- description: Permission to open a streaming session against the real-time pipe service, which the service describes as "real-time data processing service for analyzing EEG sensor data from Neurable hardware". This is the only write/create scope advertised.
  flows: []
  scope: session:stream:create
slug: neurable-scopes
source_filename: neurable-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://pipe.neurable.com/.well-known/openid-configuration (HTTP 200, scopes_supported)\ndocs: null\nauthorization_server: https://pipe.neurable.com\nnotes: >-\n  Neurable publishes no scope reference page. These five scopes are the verbatim\n  `scopes_supported` array from the live OpenID Connect Discovery document served by the pipe\n  service. Descriptions below are read from the scope grammar and the service's own OpenAPI\n  description; Neurable does not document them, so the semantics are marked inferred where they\n  are not literally stated. The `scope` query parameter is REQUIRED on /oauth/authorize.\ngrammar:\n  pattern: '<resource>:<qualifier>:<action>'\n  note: >-\n    Three of the five scopes follow a colon-delimited resource:qualifier:action grammar; the\n    remaining two (openid, email) are the standard OIDC scopes.\nscopes:\n- scope: openid\n  standard: oidc-core\n  description: Standard OpenID Connect scope;\
  \ requests an ID token from the pipe issuer.\n  inferred: false\n- scope: email\n  standard: oidc-core\n  description: >-\n    Standard OpenID Connect scope; releases the `email` claim, which the discovery document\n    lists in claims_supported and which the /oidc/userinfo response carries.\n  inferred: false\n- scope: demos:all:read\n  resource: demos\n  qualifier: all\n  action: read\n  description: >-\n    Read access to the full set of Neurable demo experiences. A demos.neurable.com host is live\n    and serves a single-page application, which is the surface this scope appears to govern.\n  inferred: true\n- scope: demos:prime:read\n  resource: demos\n  qualifier: prime\n  action: read\n  description: >-\n    Read access to a restricted \"prime\" subset of the demo experiences — a narrower grant than\n    demos:all:read.\n  inferred: true\n- scope: session:stream:create\n  resource: session\n  qualifier: stream\n  action: create\n  description: >-\n    Permission to open a streaming\
  \ session against the real-time pipe service, which the service\n    describes as \"real-time data processing service for analyzing EEG sensor data from Neurable\n    hardware\". This is the only write/create scope advertised.\n  inferred: true\ncoverage_gap: >-\n  No scope is referenced anywhere in the three published OpenAPI documents — none of them declares\n  a securitySchemes block, so no operation maps to a scope in the contract. The mapping between\n  these scopes and the Analytics Service's \"protected\" operations is not published.\ncross_links:\n  authentication: authentication/neurable-authentication.yml\n  well_known: well-known/neurable-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/scopes/neurable-scopes.yml
summary_line: 5 scopes
tags:
- Neurotechnology
- Brain-Computer Interface
- EEG
- Neuroscience
- Wearables
- biosignals
- Hardware
- Consumer Electronics
- Research Tools
- cognitive-analytics
- Health Data
- Authentication
- OpenID Connect
token_urls: []
---
