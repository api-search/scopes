---
api_specs:
- filename: usertesting-results-v2-openapi.yml
  format: yaml
  label: UserTesting Results API (v2)
  slug: usertesting-results-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-results-v2-openapi.yml
- filename: usertesting-legacy-v1-openapi.yml
  format: yaml
  label: UserTesting Legacy API (v1)
  slug: usertesting-legacy-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/openapi/usertesting-legacy-v1-openapi.yml
authorization_urls: []
description: OAuth scopes for the UserTesting APIs. The OpenAPI models only the resulting bearer JWT (http/bearer), so no scopes are derivable from the spec; this file captures the scope surface documented in the Authorization guide and the Okta authorization-server metadata saved in well-known/usertesting-oauth-authorization-server.json. The API-specific scope surface is a single read scope — the platform's authorization server additionally lists standard OIDC scopes that are not used by the Results/Legacy APIs.
docs: https://developer.usertesting.com/docs/authorization
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Usertesting Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'UserTesting publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the UserTesting API on a user''s behalf.


  Tokens are issued from https://auth.usertesting.com/oauth2/aus1p3vtd8vtm4Bxv0h8/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: UserTesting
provider_slug: usertesting
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.usertesting.com/oauth2/aus1p3vtd8vtm4Bxv0h8/v1/token
  name: oauth2ClientCredentials
  source: https://developer.usertesting.com/docs/authorization
scope_count: 1
scope_names:
- studies:read
scopes:
- description: Read access to test/study results (session summaries and details, transcripts, videos, clips, highlight reels, QXscores) across the workspaces the API user belongs to. The only scope the API docs instruct clients to request.
  flows:
  - clientCredentials
  scope: studies:read
slug: usertesting-scopes
source_filename: usertesting-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.usertesting.com/docs/authorization\ndocs: https://developer.usertesting.com/docs/authorization\ndescription: >-\n  OAuth scopes for the UserTesting APIs. The OpenAPI models only the resulting bearer JWT\n  (http/bearer), so no scopes are derivable from the spec; this file captures the scope\n  surface documented in the Authorization guide and the Okta authorization-server metadata\n  saved in well-known/usertesting-oauth-authorization-server.json. The API-specific scope\n  surface is a single read scope — the platform's authorization server additionally lists\n  standard OIDC scopes that are not used by the Results/Legacy APIs.\nschemes:\n- name: oauth2ClientCredentials\n  source: https://developer.usertesting.com/docs/authorization\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.usertesting.com/oauth2/aus1p3vtd8vtm4Bxv0h8/v1/token\nscopes:\n- scope: studies:read\n  description: >-\n   \
  \ Read access to test/study results (session summaries and details, transcripts, videos,\n    clips, highlight reels, QXscores) across the workspaces the API user belongs to. The only\n    scope the API docs instruct clients to request.\n  flows: [clientCredentials]\n  sources: [https://developer.usertesting.com/docs/authorization]\nauthorization_server_scopes:\n  note: >-\n    scopes_supported advertised by the Okta authorization server (RFC 8414 metadata); standard\n    OIDC scopes, not API data scopes.\n  scopes: [openid, profile, email, address, phone, offline_access, device_sso]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usertesting/refs/heads/main/scopes/usertesting-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- UX Research
- Usability Testing
- Human Insight
- Customer Experience
- Surveys
- Video
- Transcripts
- Experience Metrics
token_urls:
- https://auth.usertesting.com/oauth2/aus1p3vtd8vtm4Bxv0h8/v1/token
---
