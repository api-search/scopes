---
api_specs:
- filename: butterflymx-access-groups-api-openapi.yml
  format: yaml
  label: ButterflyMX Access groups API
  slug: butterflymx-access-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-groups-api-openapi.yml
- filename: butterflymx-access-logs-api-openapi.yml
  format: yaml
  label: ButterflyMX Access Logs API
  slug: butterflymx-access-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-logs-api-openapi.yml
- filename: butterflymx-access-points-api-openapi.yml
  format: yaml
  label: ButterflyMX Access Points API
  slug: butterflymx-access-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-points-api-openapi.yml
- filename: butterflymx-access-tools-api-openapi.yml
  format: yaml
  label: ButterflyMX Access Tools API
  slug: butterflymx-access-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-access-tools-api-openapi.yml
- filename: butterflymx-building-integrations-api-openapi.yml
  format: yaml
  label: ButterflyMX Building Integrations API
  slug: butterflymx-building-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-building-integrations-api-openapi.yml
- filename: butterflymx-buildings-api-openapi.yml
  format: yaml
  label: ButterflyMX Buildings API
  slug: butterflymx-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-buildings-api-openapi.yml
- filename: butterflymx-calls-api-openapi.yml
  format: yaml
  label: ButterflyMX Calls API
  slug: butterflymx-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-calls-api-openapi.yml
- filename: butterflymx-devices-api-openapi.yml
  format: yaml
  label: ButterflyMX Devices API
  slug: butterflymx-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-devices-api-openapi.yml
- filename: butterflymx-door-release-requests-api-openapi.yml
  format: yaml
  label: ButterflyMX Door Release Requests API
  slug: butterflymx-door-release-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-door-release-requests-api-openapi.yml
- filename: butterflymx-keychains-api-openapi.yml
  format: yaml
  label: ButterflyMX Keychains API
  slug: butterflymx-keychains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-keychains-api-openapi.yml
- filename: butterflymx-tenant-integrations-api-openapi.yml
  format: yaml
  label: ButterflyMX Tenant Integrations API
  slug: butterflymx-tenant-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-tenant-integrations-api-openapi.yml
- filename: butterflymx-tenants-api-openapi.yml
  format: yaml
  label: ButterflyMX Tenants API
  slug: butterflymx-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-tenants-api-openapi.yml
- filename: butterflymx-units-api-openapi.yml
  format: yaml
  label: ButterflyMX Units API
  slug: butterflymx-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-units-api-openapi.yml
- filename: butterflymx-virtual-keys-api-openapi.yml
  format: yaml
  label: ButterflyMX Virtual Keys API
  slug: butterflymx-virtual-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/openapi/butterflymx-virtual-keys-api-openapi.yml
authorization_urls:
- https://accounts.butterflymx.com/oauth/authorize
description: ''
docs: https://apidocs.butterflymx.com/docs/authorization
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Butterflymx Scopes
name_suffix: OAuth Scopes
note: 'The published OpenAPI declares no oauth2 securityScheme, so no scopes are derivable from the spec. These scopes come from the live OAuth 2.0 / OpenID Connect discovery documents the ButterflyMX authorization server serves anonymously. ButterflyMX publishes no scope-reference page in its developer docs, so the descriptions below are marked `undocumented` where the provider does not explain the scope — they are NOT guessed. The sample token response in the authorization guide shows `"scope": "public"`, confirming `public` is the default scope granted to a developer application.'
overview: 'ButterflyMX publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the ButterflyMX API on a user''s behalf.


  Tokens are issued from https://accounts.butterflymx.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ButterflyMX
provider_slug: butterflymx
schemes:
- flows:
  - authorizationUrl: https://accounts.butterflymx.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://accounts.butterflymx.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://accounts.butterflymx.com/oauth/token
  name: OAuth2
  source: https://accounts.butterflymx.com/.well-known/oauth-authorization-server
scope_count: 6
scope_names:
- public
- openid
- profile
- email
- os
- caterpillar
scopes:
- description: Default scope returned in the documented sample token response; grants access to the public ButterflyMX API v4 surface for the authenticated tenant or admin.
  flows: []
  scope: public
- description: Standard OpenID Connect scope; requests an ID token.
  flows: []
  scope: openid
- description: Standard OpenID Connect scope for basic profile claims.
  flows: []
  scope: profile
- description: Standard OpenID Connect scope for the `email` and `email_verified` claims.
  flows: []
  scope: email
- description: undocumented — advertised by the authorization server but not explained in the public docs.
  flows: []
  scope: os
- description: undocumented — advertised by the authorization server but not explained in the public docs.
  flows: []
  scope: caterpillar
slug: butterflymx-scopes
source_filename: butterflymx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: https://accounts.butterflymx.com/.well-known/openid-configuration\ndocs: https://apidocs.butterflymx.com/docs/authorization\nnote: >-\n  The published OpenAPI declares no oauth2 securityScheme, so no scopes are derivable from the spec. These\n  scopes come from the live OAuth 2.0 / OpenID Connect discovery documents the ButterflyMX authorization\n  server serves anonymously. ButterflyMX publishes no scope-reference page in its developer docs, so the\n  descriptions below are marked `undocumented` where the provider does not explain the scope — they are NOT\n  guessed. The sample token response in the authorization guide shows `\"scope\": \"public\"`, confirming\n  `public` is the default scope granted to a developer application.\nschemes:\n- name: OAuth2\n  source: https://accounts.butterflymx.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.butterflymx.com/oauth/authorize\n\
  \    tokenUrl: https://accounts.butterflymx.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://accounts.butterflymx.com/oauth/token\nscopes:\n- scope: public\n  description: >-\n    Default scope returned in the documented sample token response; grants access to the public ButterflyMX\n    API v4 surface for the authenticated tenant or admin.\n  documented: true\n  sources:\n  - https://apidocs.butterflymx.com/docs/authorization\n  - https://accounts.butterflymx.com/.well-known/openid-configuration\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token.\n  documented: false\n  standard: openid-connect-core\n  sources:\n  - https://accounts.butterflymx.com/.well-known/openid-configuration\n- scope: profile\n  description: Standard OpenID Connect scope for basic profile claims.\n  documented: false\n  standard: openid-connect-core\n  sources:\n  - https://accounts.butterflymx.com/.well-known/openid-configuration\n- scope: email\n  description:\
  \ Standard OpenID Connect scope for the `email` and `email_verified` claims.\n  documented: false\n  standard: openid-connect-core\n  sources:\n  - https://accounts.butterflymx.com/.well-known/openid-configuration\n- scope: os\n  description: undocumented — advertised by the authorization server but not explained in the public docs.\n  documented: false\n  sources:\n  - https://accounts.butterflymx.com/.well-known/openid-configuration\n- scope: caterpillar\n  description: undocumented — advertised by the authorization server but not explained in the public docs.\n  documented: false\n  sources:\n  - https://accounts.butterflymx.com/.well-known/openid-configuration\nclaims_supported:\n- iss\n- sub\n- aud\n- exp\n- iat\n- email\n- email_verified\ngaps:\n- >-\n  There is no published scopes/permissions reference. Two of the six advertised scopes (`os`, `caterpillar`)\n  are undocumented, and the OpenAPI does not bind any operation to a scope, so an integrator cannot\n  determine least-privilege\
  \ access from the contract.\nx-evidence:\n- url: https://accounts.butterflymx.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-08'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butterflymx/refs/heads/main/scopes/butterflymx-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Access Control
- physical-access
- smart-intercom
- PropTech
- Property Management
- Multifamily
- Building Automation
- Visitor Management
- IoT
- smart-locks
- Authentication
- Webhook
token_urls:
- https://accounts.butterflymx.com/oauth/token
---
