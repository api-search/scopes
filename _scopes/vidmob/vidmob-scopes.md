---
api_specs:
- filename: vidmob-media-api-openapi.yml
  format: yaml
  label: VidMob Media API
  slug: vidmob-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-media-api-openapi.yml
- filename: vidmob-organization-api-openapi.yml
  format: yaml
  label: VidMob Organization API
  slug: vidmob-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-organization-api-openapi.yml
- filename: vidmob-scoring-api-openapi.yml
  format: yaml
  label: VidMob Scoring API
  slug: vidmob-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-scoring-api-openapi.yml
- filename: vidmob-workspaces-api-openapi.yml
  format: yaml
  label: VidMob Workspaces API
  slug: vidmob-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-workspaces-api-openapi.yml
authorization_urls:
- https://acs.vidmob.com/oauth/authorize
description: ''
docs:
- https://vidmob-api-docs.readme.io/docs/authentication
- https://help.vidmob.com/en/articles/15461399-vidmob-mcp-security-compliance-overview
flows:
- authorizationCode
- refreshToken
- jwtBearer
kind: oauth-scopes
layout: scope
method: searched
name: Vidmob Scopes
name_suffix: OAuth Scopes
note: Vidmob runs two distinct scope vocabularies. The REST API keys carry capability-domain scopes (organization / scoring / aperture / analytics with read or read_write access) that are documented in the developer portal but are NOT declared in the published OpenAPI — the specs only declare a single apiKey scheme, so 0-working/derive-oauth-scopes.py finds nothing. The MCP authorization server publishes a separate OIDC-style scope set in its RFC 8414 / OIDC discovery documents. Both are recorded below with their real source.
overview: 'VidMob publishes 12 OAuth 2.0 scopes via the authorizationCode, refreshToken, and jwtBearer flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the VidMob API on a user''s behalf.


  Tokens are issued from https://mcp-auth.vidmob.com/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: VidMob
provider_slug: vidmob
schemes:
- in: header
  issued_per: organization
  management_url: https://acs.vidmob.com/api-key-management
  name: vidmob-api-key
  parameter: Authorization
  scheme: Bearer
  source: https://vidmob-api-docs.readme.io/docs/authentication
  type: apiKey
- flows:
  - authorizationUrl: https://acs.vidmob.com/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    registrationUrl: https://mcp-auth.vidmob.com/v1/oauth2/register
    tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token
  - flow: refreshToken
    tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token
  - flow: jwtBearer
    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token
  name: vidmob-mcp-oauth
  source: https://mcp-auth.vidmob.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 12
scope_names:
- scoring:read
- scoring:read_write
- aperture:read
- aperture:read_write
- organization:read
- analytics:read
- openid
- profile
- email
- phone
- offline_access
- full_access
scopes:
- description: View guidelines, criteria, scorecards and scores. Covers GET /v1/scoring/workspace/{workspaceId}/scorecards, GET /v1/scoring/scorecard/{scorecardId}/media-metadata, GET /v1/scoring/media/{mediaId}/scores, GET /v1/media/{mediaId}/status, POST /v1/scoring/criteria/metadata and GET /v1/media/updated-scores.
  flows: []
  scope: scoring:read
- description: Submit media for scoring (POST /v1/media, and upload reservation on the MCP surface) plus everything scoring:read grants.
  flows: []
  scope: scoring:read_write
- description: Retrieve Creative Tags job status and results — GET /v1/media/aperture/{jobId}.
  flows: []
  scope: aperture:read
- description: Submit assets for tagging — POST /v1/media/aperture — plus everything aperture:read grants.
  flows: []
  scope: aperture:read_write
- description: Workspace and ad-account reference data. A valid key with no specific scope already reaches GET /v1/organization, GET /v1/permission and GET /v1/workspaces.
  flows: []
  scope: organization:read
- description: Media performance and KPI discovery. Exposed on the MCP surface only; no public REST operation.
  flows: []
  scope: analytics:read
- description: OIDC subject identity on the MCP authorization server.
  flows:
  - authorizationCode
  scope: openid
- description: ''
  flows:
  - authorizationCode
  scope: profile
- description: ''
  flows:
  - authorizationCode
  scope: email
- description: ''
  flows:
  - authorizationCode
  scope: phone
- description: Issues a refresh token so an agent stays connected after the one-time interactive sign-in.
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
- description: Advertised in the OIDC discovery document's scopes_supported but absent from the RFC 8414 oauth-authorization-server document and undocumented in the help center.
  flows:
  - authorizationCode
  scope: full_access
slug: vidmob-scopes
source_filename: vidmob-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://vidmob-api-docs.readme.io/docs/authentication\ndocs:\n  - https://vidmob-api-docs.readme.io/docs/authentication\n  - https://help.vidmob.com/en/articles/15461399-vidmob-mcp-security-compliance-overview\nnote: >-\n  Vidmob runs two distinct scope vocabularies. The REST API keys carry capability-domain scopes (organization / scoring\n  / aperture / analytics with read or read_write access) that are documented in the developer portal but are NOT\n  declared in the published OpenAPI — the specs only declare a single apiKey scheme, so 0-working/derive-oauth-scopes.py\n  finds nothing. The MCP authorization server publishes a separate OIDC-style scope set in its RFC 8414 / OIDC discovery\n  documents. Both are recorded below with their real source.\nschemes:\n  - name: vidmob-api-key\n    type: apiKey\n    in: header\n    parameter: Authorization\n    scheme: Bearer\n    issued_per: organization\n    management_url: https://acs.vidmob.com/api-key-management\n\
  \    source: https://vidmob-api-docs.readme.io/docs/authentication\n  - name: vidmob-mcp-oauth\n    type: oauth2\n    source: https://mcp-auth.vidmob.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://acs.vidmob.com/oauth/authorize\n        tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token\n        registrationUrl: https://mcp-auth.vidmob.com/v1/oauth2/register\n        code_challenge_methods: [S256]\n      - flow: refreshToken\n        tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token\n      - flow: jwtBearer\n        grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n        tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token\nscopes:\n  - scope: scoring:read\n    description: >-\n      View guidelines, criteria, scorecards and scores. Covers GET /v1/scoring/workspace/{workspaceId}/scorecards,\n      GET /v1/scoring/scorecard/{scorecardId}/media-metadata, GET /v1/scoring/media/{mediaId}/scores,\n\
  \      GET /v1/media/{mediaId}/status, POST /v1/scoring/criteria/metadata and GET /v1/media/updated-scores.\n    domain: scoring\n    access: read\n    kind: api-key\n    sources: [https://vidmob-api-docs.readme.io/docs/authentication]\n  - scope: scoring:read_write\n    description: >-\n      Submit media for scoring (POST /v1/media, and upload reservation on the MCP surface) plus everything\n      scoring:read grants.\n    domain: scoring\n    access: read_write\n    kind: api-key\n    sources: [https://vidmob-api-docs.readme.io/docs/authentication]\n  - scope: aperture:read\n    description: Retrieve Creative Tags job status and results — GET /v1/media/aperture/{jobId}.\n    domain: aperture\n    access: read\n    kind: api-key\n    sources: [https://vidmob-api-docs.readme.io/docs/authentication]\n  - scope: aperture:read_write\n    description: Submit assets for tagging — POST /v1/media/aperture — plus everything aperture:read grants.\n    domain: aperture\n    access: read_write\n\
  \    kind: api-key\n    sources: [https://vidmob-api-docs.readme.io/docs/authentication]\n  - scope: organization:read\n    description: >-\n      Workspace and ad-account reference data. A valid key with no specific scope already reaches\n      GET /v1/organization, GET /v1/permission and GET /v1/workspaces.\n    domain: organization\n    access: read\n    kind: api-key\n    sources: [https://help.vidmob.com/en/articles/15461399-vidmob-mcp-security-compliance-overview]\n  - scope: analytics:read\n    description: Media performance and KPI discovery. Exposed on the MCP surface only; no public REST operation.\n    domain: analytics\n    access: read\n    kind: api-key\n    sources: [https://help.vidmob.com/en/articles/15461399-vidmob-mcp-security-compliance-overview]\n  - scope: openid\n    description: OIDC subject identity on the MCP authorization server.\n    kind: oauth2\n    flows: [authorizationCode]\n    sources: [https://mcp-auth.vidmob.com/.well-known/openid-configuration]\n  -\
  \ scope: profile\n    kind: oauth2\n    flows: [authorizationCode]\n    sources: [https://mcp-auth.vidmob.com/.well-known/openid-configuration]\n  - scope: email\n    kind: oauth2\n    flows: [authorizationCode]\n    sources: [https://mcp-auth.vidmob.com/.well-known/openid-configuration]\n  - scope: phone\n    kind: oauth2\n    flows: [authorizationCode]\n    sources: [https://mcp-auth.vidmob.com/.well-known/openid-configuration]\n  - scope: offline_access\n    description: Issues a refresh token so an agent stays connected after the one-time interactive sign-in.\n    kind: oauth2\n    flows: [authorizationCode, refreshToken]\n    sources: [https://mcp-auth.vidmob.com/.well-known/openid-configuration]\n  - scope: full_access\n    description: >-\n      Advertised in the OIDC discovery document's scopes_supported but absent from the RFC 8414\n      oauth-authorization-server document and undocumented in the help center.\n    kind: oauth2\n    flows: [authorizationCode]\n    sources: [https://mcp-auth.vidmob.com/.well-known/openid-configuration]\n\
  withheld:\n  - scope: admin\n    reason: >-\n      Vidmob states administrative capabilities sit behind an internal-only admin scope that is never granted to\n      external partner credentials. Recorded for completeness; not obtainable by a customer.\n    sources: [https://help.vidmob.com/en/articles/15461399-vidmob-mcp-security-compliance-overview]\nx-evidence:\n  - fetched: '2026-08-05'\n    url: https://mcp-auth.vidmob.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - fetched: '2026-08-05'\n    url: https://mcp-auth.vidmob.com/.well-known/openid-configuration\n    http_status: 200\n  - fetched: '2026-08-05'\n    url: https://vidmob-api-docs.readme.io/docs/authentication.md\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/scopes/vidmob-scopes.yml
summary_line: 12 scopes · authorizationCode/refreshToken/jwtBearer
tags:
- Creative Intelligence
- creative-data
- Advertising
- Marketing
- Media Measurement
- Video
- Computer-Vision
- Creative Analytics
- AdTech
- MCP
- agent-native
- MarTech
token_urls:
- https://mcp-auth.vidmob.com/v1/oauth2/token
---
