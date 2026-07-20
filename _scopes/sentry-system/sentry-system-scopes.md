---
api_specs:
- filename: openapi-derefed.json
  format: json
  label: Sentry API
  slug: sentry-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Events and Issues API
  slug: sentry-events-and-issues-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Organizations API
  slug: sentry-organizations-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Projects API
  slug: sentry-projects-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Teams API
  slug: sentry-teams-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Releases API
  slug: sentry-releases-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Alerts API
  slug: sentry-alerts-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Crons API
  slug: sentry-crons-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Dashboards API
  slug: sentry-dashboards-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Discover API
  slug: sentry-discover-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Environments API
  slug: sentry-environments-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Explore API
  slug: sentry-explore-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Integration Platform API
  slug: sentry-integration-platform-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Integrations API
  slug: sentry-integrations-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Mobile Builds API
  slug: sentry-mobile-builds-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Monitors API
  slug: sentry-monitors-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Prevent API
  slug: sentry-prevent-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Replays API
  slug: sentry-replays-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry SCIM API
  slug: sentry-scim-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Seer API
  slug: sentry-seer-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
- filename: openapi-derefed.json
  format: json
  label: Sentry Users API
  slug: sentry-users-api
  spec_type: OpenAPI
  url: https://github.com/getsentry/sentry-api-schema/blob/main/openapi-derefed.json
authorization_urls:
- https://sentry.io/oauth/authorize/
description: ''
docs: https://docs.sentry.io/api/permissions/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sentry System Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sentry publishes 26 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sentry API on a user''s behalf.


  Tokens are issued from https://sentry.io/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sentry
provider_slug: sentry-system
schemes:
- flows:
  - authorizationUrl: https://sentry.io/oauth/authorize/
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    tokenUrl: https://sentry.io/oauth/token/
  name: OAuth2
  source: https://sentry.io/.well-known/oauth-authorization-server
scope_count: 26
scope_names:
- openid
- email
- profile
- org:read
- org:write
- org:admin
- org:billing
- org:ci
- org:integrations
- project:read
- project:write
- project:admin
- project:releases
- project:distribution
- team:read
- team:write
- team:admin
- member:read
- member:invite
- member:write
- member:admin
- event:read
- event:write
- event:admin
- alerts:read
- alerts:write
scopes:
- description: OpenID Connect authentication
  flows: []
  scope: openid
- description: Access the user's email address
  flows: []
  scope: email
- description: Access the user's basic profile
  flows: []
  scope: profile
- description: Read organization details (GET organization endpoints)
  flows: []
  scope: org:read
- description: Create/update organizations (PUT/POST organization endpoints)
  flows: []
  scope: org:write
- description: Delete organizations and full admin (DELETE organization endpoints)
  flows: []
  scope: org:admin
- description: Access organization billing information
  flows: []
  scope: org:billing
- description: CI and deployment workflows — upload source maps
  flows: []
  scope: org:ci
- description: Manage organization integrations
  flows: []
  scope: org:integrations
- description: Read project details (GET project endpoints)
  flows: []
  scope: project:read
- description: Create/update projects (PUT/POST project endpoints)
  flows: []
  scope: project:write
- description: Delete projects and full admin (DELETE project endpoints)
  flows: []
  scope: project:admin
- description: Access project and organization release endpoints
  flows: []
  scope: project:releases
- description: Access project distribution/artifact endpoints
  flows: []
  scope: project:distribution
- description: Read team details (GET team endpoints)
  flows: []
  scope: team:read
- description: Create/update teams (PUT/POST team endpoints)
  flows: []
  scope: team:write
- description: Delete teams and full admin (DELETE team endpoints)
  flows: []
  scope: team:admin
- description: Read organization members (GET member endpoints)
  flows: []
  scope: member:read
- description: Invite members to the organization
  flows: []
  scope: member:invite
- description: Create/update members (PUT/POST member endpoints)
  flows: []
  scope: member:write
- description: Remove members and full admin (DELETE member endpoints)
  flows: []
  scope: member:admin
- description: Read issues and events (GET event endpoints)
  flows: []
  scope: event:read
- description: Update issues and events (PUT event endpoints)
  flows: []
  scope: event:write
- description: Delete issues and events (DELETE event endpoints)
  flows: []
  scope: event:admin
- description: Read alert rules
  flows: []
  scope: alerts:read
- description: Create/update/delete alert rules
  flows: []
  scope: alerts:write
slug: sentry-system-scopes
source_filename: sentry-system-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://sentry.io/.well-known/oauth-authorization-server\ndocs: https://docs.sentry.io/api/permissions/\nnotes: >-\n  Sentry auth tokens (user, organization, and internal/public integration tokens) are scope-bearing.\n  The authoritative scope list is published in Sentry's RFC 8414 OAuth authorization-server document;\n  descriptions and the GET/PUT-POST/DELETE permission-level mapping come from the API permissions docs.\n  OpenAPI specs in this repo declare only bearer/DSN security schemes, so the scope surface is not\n  derivable from them and is captured here from the provider's own OAuth metadata.\nschemes:\n  - name: OAuth2\n    source: https://sentry.io/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://sentry.io/oauth/authorize/\n        tokenUrl: https://sentry.io/oauth/token/\n        pkce: S256\n        grant_types: [authorization_code, refresh_token]\n\
  scopes:\n  - {scope: openid, description: OpenID Connect authentication}\n  - {scope: email, description: Access the user's email address}\n  - {scope: profile, description: Access the user's basic profile}\n  - {scope: org:read, description: Read organization details (GET organization endpoints)}\n  - {scope: org:write, description: Create/update organizations (PUT/POST organization endpoints)}\n  - {scope: org:admin, description: Delete organizations and full admin (DELETE organization endpoints)}\n  - {scope: org:billing, description: Access organization billing information}\n  - {scope: org:ci, description: CI and deployment workflows — upload source maps, create releases, manage code mappings}\n  - {scope: org:integrations, description: Manage organization integrations}\n  - {scope: project:read, description: Read project details (GET project endpoints)}\n  - {scope: project:write, description: Create/update projects (PUT/POST project endpoints)}\n  - {scope: project:admin, description:\
  \ Delete projects and full admin (DELETE project endpoints)}\n  - {scope: project:releases, description: Access project and organization release endpoints}\n  - {scope: project:distribution, description: Access project distribution/artifact endpoints}\n  - {scope: team:read, description: Read team details (GET team endpoints)}\n  - {scope: team:write, description: Create/update teams (PUT/POST team endpoints)}\n  - {scope: team:admin, description: Delete teams and full admin (DELETE team endpoints)}\n  - {scope: member:read, description: Read organization members (GET member endpoints)}\n  - {scope: member:invite, description: Invite members to the organization}\n  - {scope: member:write, description: Create/update members (PUT/POST member endpoints)}\n  - {scope: member:admin, description: Remove members and full admin (DELETE member endpoints)}\n  - {scope: event:read, description: Read issues and events (GET event endpoints)}\n  - {scope: event:write, description: Update issues and\
  \ events (PUT event endpoints)}\n  - {scope: event:admin, description: Delete issues and events (DELETE event endpoints)}\n  - {scope: alerts:read, description: Read alert rules}\n  - {scope: alerts:write, description: Create/update/delete alert rules}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentry-system/refs/heads/main/scopes/sentry-system-scopes.yml
summary_line: 26 scopes · authorizationCode
tags:
- APM
- Application Monitoring
- Bug Tracking
- Developer Tools
- Error Tracking
- Observability
- Performance Monitoring
- Real-Time Monitoring
token_urls:
- https://sentry.io/oauth/token/
---
