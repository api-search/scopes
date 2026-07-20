---
api_specs:
- filename: socket-packages-api-openapi.yml
  format: yaml
  label: Socket Packages API
  slug: socket-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-packages-api-openapi.yml
- filename: socket-full-scans-api-openapi.yml
  format: yaml
  label: Socket Full Scans API
  slug: socket-full-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-full-scans-api-openapi.yml
- filename: socket-diff-scans-api-openapi.yml
  format: yaml
  label: Socket Diff Scans API
  slug: socket-diff-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-diff-scans-api-openapi.yml
- filename: socket-alerts-api-openapi.yml
  format: yaml
  label: Socket Alerts API
  slug: socket-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-alerts-api-openapi.yml
- filename: socket-triage-api-openapi.yml
  format: yaml
  label: Socket Triage API
  slug: socket-triage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-triage-api-openapi.yml
- filename: socket-repos-api-openapi.yml
  format: yaml
  label: Socket Repos API
  slug: socket-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-repos-api-openapi.yml
- filename: socket-org-settings-api-openapi.yml
  format: yaml
  label: Socket Organization Settings API
  slug: socket-org-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-org-settings-api-openapi.yml
- filename: socket-webhooks-api-openapi.yml
  format: yaml
  label: Socket Webhooks API
  slug: socket-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-webhooks-api-openapi.yml
- filename: socket-threat-feed-api-openapi.yml
  format: yaml
  label: Socket Threat Feed API
  slug: socket-threat-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-threat-feed-api-openapi.yml
- filename: socket-fixes-api-openapi.yml
  format: yaml
  label: Socket Fixes API
  slug: socket-fixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-fixes-api-openapi.yml
- filename: socket-dependencies-api-openapi.yml
  format: yaml
  label: Socket Dependencies API
  slug: socket-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dependencies-api-openapi.yml
- filename: socket-api-tokens-api-openapi.yml
  format: yaml
  label: Socket API Tokens API
  slug: socket-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-api-tokens-api-openapi.yml
- filename: socket-audit-log-api-openapi.yml
  format: yaml
  label: Socket Audit Log API
  slug: socket-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-audit-log-api-openapi.yml
- filename: socket-org-snapshots-api-openapi.yml
  format: yaml
  label: Socket Organization Snapshots API
  slug: socket-org-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-org-snapshots-api-openapi.yml
- filename: socket-metadata-api-openapi.yml
  format: yaml
  label: Socket Metadata API
  slug: socket-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-metadata-api-openapi.yml
authorization_urls:
- https://api.socket.dev/v1/oauth2/authorize
description: Socket operates a live OAuth 2.0 authorization server (RFC 8414 metadata at https://api.socket.dev/.well-known/oauth-authorization-server) alongside organization API tokens. Scopes below are captured verbatim from scopes_supported. Socket groups clients into three classes (internal_socket_app, customer_user_delegated, customer_machine_to_machine); customer M2M uses client_credentials, delegated uses authorization_code + refresh_token (PKCE S256).
docs: https://docs.socket.dev/reference/authentication-types
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Socket Dev Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Socket publishes 97 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Socket API on a user''s behalf.


  Tokens are issued from https://api.socket.dev/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Socket
provider_slug: socket-dev
schemes:
- flows:
  - authorizationUrl: https://api.socket.dev/v1/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.socket.dev/v1/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://api.socket.dev/v1/oauth2/token
  name: OAuth2
  source: well-known/socket-dev-oauth-authorization-server.json
scope_count: 97
scope_names:
- alerts
- alerts:list
- alerts:trend
- alert-resolution
- alert-resolution:list
- alert-resolution:create
- alert-resolution:read
- alert-resolution:delete
- threat-campaigns
- threat-campaigns:list
- api-tokens
- api-tokens:create
- api-tokens:update
- api-tokens:revoke
- api-tokens:rotate
- api-tokens:list
- audit-log
- audit-log:list
- dependencies
- dependencies:list
- dependencies:trend
- fixes
- fixes:list
- full-scans
- full-scans:list
- full-scans:create
- full-scans:delete
- diff-scans
- diff-scans:list
- diff-scans:create
- diff-scans:delete
- entitlements
- entitlements:list
- historical
- historical:snapshots-list
- historical:snapshots-start
- historical:alerts-list
- historical:alerts-trend
- historical:dependencies-list
- historical:dependencies-trend
- integration
- integration:list
- integration:create
- integration:update
- integration:delete
- access-policy
- access-policy:read
- access-policy:attach
- access-policy:update
- license-policy
- license-policy:update
- license-policy:read
- packages
- packages:list
- access-policy-definition
- access-policy-definition:attach
- access-policy-definition:read
- access-policy-definition:update
- report
- report:list
- report:read
- report:write
- repo
- repo:list
- repo:create
- repo:update
- repo:delete
- repo-label
- repo-label:list
- repo-label:create
- repo-label:update
- repo-label:delete
- security-policy
- security-policy:update
- security-policy:read
- socket-basics
- socket-basics:read
- telemetry-policy
- telemetry-policy:update
- telemetry-events
- telemetry-events:list
- threat-feed
- threat-feed:list
- triage
- triage:alerts-list
- triage:alerts-update
- uploaded-artifacts
- uploaded-artifacts:create
- uploaded-artifacts:list
- webhooks
- webhooks:create
- webhooks:list
- webhooks:update
- webhooks:delete
- openid
- profile
- email
scopes:
- description: ''
  flows: []
  scope: alerts
- description: ''
  flows: []
  scope: alerts:list
- description: ''
  flows: []
  scope: alerts:trend
- description: ''
  flows: []
  scope: alert-resolution
- description: ''
  flows: []
  scope: alert-resolution:list
- description: ''
  flows: []
  scope: alert-resolution:create
- description: ''
  flows: []
  scope: alert-resolution:read
- description: ''
  flows: []
  scope: alert-resolution:delete
- description: ''
  flows: []
  scope: threat-campaigns
- description: ''
  flows: []
  scope: threat-campaigns:list
- description: ''
  flows: []
  scope: api-tokens
- description: ''
  flows: []
  scope: api-tokens:create
- description: ''
  flows: []
  scope: api-tokens:update
- description: ''
  flows: []
  scope: api-tokens:revoke
- description: ''
  flows: []
  scope: api-tokens:rotate
- description: ''
  flows: []
  scope: api-tokens:list
- description: ''
  flows: []
  scope: audit-log
- description: ''
  flows: []
  scope: audit-log:list
- description: ''
  flows: []
  scope: dependencies
- description: ''
  flows: []
  scope: dependencies:list
- description: ''
  flows: []
  scope: dependencies:trend
- description: ''
  flows: []
  scope: fixes
- description: ''
  flows: []
  scope: fixes:list
- description: ''
  flows: []
  scope: full-scans
- description: ''
  flows: []
  scope: full-scans:list
- description: ''
  flows: []
  scope: full-scans:create
- description: ''
  flows: []
  scope: full-scans:delete
- description: ''
  flows: []
  scope: diff-scans
- description: ''
  flows: []
  scope: diff-scans:list
- description: ''
  flows: []
  scope: diff-scans:create
- description: ''
  flows: []
  scope: diff-scans:delete
- description: ''
  flows: []
  scope: entitlements
- description: ''
  flows: []
  scope: entitlements:list
- description: ''
  flows: []
  scope: historical
- description: ''
  flows: []
  scope: historical:snapshots-list
- description: ''
  flows: []
  scope: historical:snapshots-start
- description: ''
  flows: []
  scope: historical:alerts-list
- description: ''
  flows: []
  scope: historical:alerts-trend
- description: ''
  flows: []
  scope: historical:dependencies-list
- description: ''
  flows: []
  scope: historical:dependencies-trend
- description: ''
  flows: []
  scope: integration
- description: ''
  flows: []
  scope: integration:list
- description: ''
  flows: []
  scope: integration:create
- description: ''
  flows: []
  scope: integration:update
- description: ''
  flows: []
  scope: integration:delete
- description: ''
  flows: []
  scope: access-policy
- description: ''
  flows: []
  scope: access-policy:read
- description: ''
  flows: []
  scope: access-policy:attach
- description: ''
  flows: []
  scope: access-policy:update
- description: ''
  flows: []
  scope: license-policy
- description: ''
  flows: []
  scope: license-policy:update
- description: ''
  flows: []
  scope: license-policy:read
- description: ''
  flows: []
  scope: packages
- description: ''
  flows: []
  scope: packages:list
- description: ''
  flows: []
  scope: access-policy-definition
- description: ''
  flows: []
  scope: access-policy-definition:attach
- description: ''
  flows: []
  scope: access-policy-definition:read
- description: ''
  flows: []
  scope: access-policy-definition:update
- description: ''
  flows: []
  scope: report
- description: ''
  flows: []
  scope: report:list
- description: ''
  flows: []
  scope: report:read
- description: ''
  flows: []
  scope: report:write
- description: ''
  flows: []
  scope: repo
- description: ''
  flows: []
  scope: repo:list
- description: ''
  flows: []
  scope: repo:create
- description: ''
  flows: []
  scope: repo:update
- description: ''
  flows: []
  scope: repo:delete
- description: ''
  flows: []
  scope: repo-label
- description: ''
  flows: []
  scope: repo-label:list
- description: ''
  flows: []
  scope: repo-label:create
- description: ''
  flows: []
  scope: repo-label:update
- description: ''
  flows: []
  scope: repo-label:delete
- description: ''
  flows: []
  scope: security-policy
- description: ''
  flows: []
  scope: security-policy:update
- description: ''
  flows: []
  scope: security-policy:read
- description: ''
  flows: []
  scope: socket-basics
- description: ''
  flows: []
  scope: socket-basics:read
- description: ''
  flows: []
  scope: telemetry-policy
- description: ''
  flows: []
  scope: telemetry-policy:update
- description: ''
  flows: []
  scope: telemetry-events
- description: ''
  flows: []
  scope: telemetry-events:list
- description: ''
  flows: []
  scope: threat-feed
- description: ''
  flows: []
  scope: threat-feed:list
- description: ''
  flows: []
  scope: triage
- description: ''
  flows: []
  scope: triage:alerts-list
- description: ''
  flows: []
  scope: triage:alerts-update
- description: ''
  flows: []
  scope: uploaded-artifacts
- description: ''
  flows: []
  scope: uploaded-artifacts:create
- description: ''
  flows: []
  scope: uploaded-artifacts:list
- description: ''
  flows: []
  scope: webhooks
- description: ''
  flows: []
  scope: webhooks:create
- description: ''
  flows: []
  scope: webhooks:list
- description: ''
  flows: []
  scope: webhooks:update
- description: ''
  flows: []
  scope: webhooks:delete
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: email
slug: socket-dev-scopes
source_filename: socket-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: well-known/socket-dev-oauth-authorization-server.json\ndocs: https://docs.socket.dev/reference/authentication-types\ndescription: >-\n  Socket operates a live OAuth 2.0 authorization server (RFC 8414 metadata at\n  https://api.socket.dev/.well-known/oauth-authorization-server) alongside organization\n  API tokens. Scopes below are captured verbatim from scopes_supported. Socket groups\n  clients into three classes (internal_socket_app, customer_user_delegated,\n  customer_machine_to_machine); customer M2M uses client_credentials, delegated uses\n  authorization_code + refresh_token (PKCE S256).\nschemes:\n  - name: OAuth2\n    source: well-known/socket-dev-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.socket.dev/v1/oauth2/authorize\n        tokenUrl: https://api.socket.dev/v1/oauth2/token\n      - flow: clientCredentials\n        tokenUrl: https://api.socket.dev/v1/oauth2/token\n\
  client_classes: [\"internal_socket_app\", \"customer_user_delegated\", \"customer_machine_to_machine\"]\ngrant_types: [\"authorization_code\", \"refresh_token\"]\ncode_challenge_methods: [\"S256\"]\nscopes:\n  - scope: alerts\n  - scope: alerts:list\n  - scope: alerts:trend\n  - scope: alert-resolution\n  - scope: alert-resolution:list\n  - scope: alert-resolution:create\n  - scope: alert-resolution:read\n  - scope: alert-resolution:delete\n  - scope: threat-campaigns\n  - scope: threat-campaigns:list\n  - scope: api-tokens\n  - scope: api-tokens:create\n  - scope: api-tokens:update\n  - scope: api-tokens:revoke\n  - scope: api-tokens:rotate\n  - scope: api-tokens:list\n  - scope: audit-log\n  - scope: audit-log:list\n  - scope: dependencies\n  - scope: dependencies:list\n  - scope: dependencies:trend\n  - scope: fixes\n  - scope: fixes:list\n  - scope: full-scans\n  - scope: full-scans:list\n  - scope: full-scans:create\n  - scope: full-scans:delete\n  - scope: diff-scans\n  - scope:\
  \ diff-scans:list\n  - scope: diff-scans:create\n  - scope: diff-scans:delete\n  - scope: entitlements\n  - scope: entitlements:list\n  - scope: historical\n  - scope: historical:snapshots-list\n  - scope: historical:snapshots-start\n  - scope: historical:alerts-list\n  - scope: historical:alerts-trend\n  - scope: historical:dependencies-list\n  - scope: historical:dependencies-trend\n  - scope: integration\n  - scope: integration:list\n  - scope: integration:create\n  - scope: integration:update\n  - scope: integration:delete\n  - scope: access-policy\n  - scope: access-policy:read\n  - scope: access-policy:attach\n  - scope: access-policy:update\n  - scope: license-policy\n  - scope: license-policy:update\n  - scope: license-policy:read\n  - scope: packages\n  - scope: packages:list\n  - scope: access-policy-definition\n  - scope: access-policy-definition:attach\n  - scope: access-policy-definition:read\n  - scope: access-policy-definition:update\n  - scope: report\n  - scope: report:list\n\
  \  - scope: report:read\n  - scope: report:write\n  - scope: repo\n  - scope: repo:list\n  - scope: repo:create\n  - scope: repo:update\n  - scope: repo:delete\n  - scope: repo-label\n  - scope: repo-label:list\n  - scope: repo-label:create\n  - scope: repo-label:update\n  - scope: repo-label:delete\n  - scope: security-policy\n  - scope: security-policy:update\n  - scope: security-policy:read\n  - scope: socket-basics\n  - scope: socket-basics:read\n  - scope: telemetry-policy\n  - scope: telemetry-policy:update\n  - scope: telemetry-events\n  - scope: telemetry-events:list\n  - scope: threat-feed\n  - scope: threat-feed:list\n  - scope: triage\n  - scope: triage:alerts-list\n  - scope: triage:alerts-update\n  - scope: uploaded-artifacts\n  - scope: uploaded-artifacts:create\n  - scope: uploaded-artifacts:list\n  - scope: webhooks\n  - scope: webhooks:create\n  - scope: webhooks:list\n  - scope: webhooks:update\n  - scope: webhooks:delete\n  - scope: openid\n  - scope: profile\n  - scope:\
  \ email\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/scopes/socket-dev-scopes.yml
summary_line: 97 scopes · authorizationCode/clientCredentials
tags:
- Supply Chain Security
- Open Source Security
- Software Composition Analysis
- SCA
- Malware Detection
- Dependency Scanning
- SBOM
- npm
- PyPI
- Go
- Maven
- Cargo
- NuGet
- RubyGems
- Developer Security
token_urls:
- https://api.socket.dev/v1/oauth2/token
---
