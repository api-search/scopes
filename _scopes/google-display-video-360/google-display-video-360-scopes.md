---
api_specs:
- filename: google-display-video-360-api-openapi.yml
  format: yaml
  label: Google Display & Video 360 API
  slug: google-display-video-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-display-video-360/refs/heads/main/openapi/google-display-video-360-api-openapi.yml
- filename: google-display-video-360-advertisers-api-openapi.yml
  format: yaml
  label: Google Display & Video 360 Advertisers API
  slug: google-display-video-360-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-display-video-360/refs/heads/main/openapi/google-display-video-360-advertisers-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: 'The complete OAuth 2.0 scope surface for the Display & Video 360 API, taken from the auth.oauth2.scopes block of Google''s own Discovery Document rather than inferred from operation security requirements. Four scopes, all authorization-code flow, all issued by accounts.google.com. There is no read-only variant: display-video is read AND write AND delete in a single grant, which is the most consequential fact in this file for anyone binding an agent to this API.'
docs: https://developers.google.com/display-video/api/guides/how-tos/authorizing
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Display Video 360 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Display & Video 360 publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Display & Video 360 API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Display & Video 360
provider_slug: google-display-video-360
schemes:
- authorization_server_metadata: well-known/google-display-video-360-oauth-authorization-server.json
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    refreshUrl: https://oauth2.googleapis.com/token
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  pkce: supported (S256)
  source: openapi/google-display-video-360-api-openapi.yml
scope_count: 4
scope_names:
- https://www.googleapis.com/auth/display-video
- https://www.googleapis.com/auth/display-video-mediaplanning
- https://www.googleapis.com/auth/display-video-user-management
- https://www.googleapis.com/auth/doubleclickbidmanager
scopes:
- description: Create, see, edit, and permanently delete your Display & Video 360 entities and reports
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/display-video
- description: Create, see, and edit Display & Video 360 Campaign entities and see billing invoices
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/display-video-mediaplanning
- description: 'Private Service: https://www.googleapis.com/auth/display-video-user-management'
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/display-video-user-management
- description: View and manage your reports in DoubleClick Bid Manager
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/doubleclickbidmanager
slug: google-display-video-360-scopes
source_filename: google-display-video-360-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://displayvideo.googleapis.com/$discovery/rest?version=v4 (auth.oauth2.scopes, revision\n  20260813) cross-checked against\n  https://developers.google.com/display-video/api/guides/how-tos/authorizing\ndocs: https://developers.google.com/display-video/api/guides/how-tos/authorizing\ndescription: >-\n  The complete OAuth 2.0 scope surface for the Display & Video 360 API, taken from the\n  auth.oauth2.scopes block of Google's own Discovery Document rather than inferred from operation\n  security requirements. Four scopes, all authorization-code flow, all issued by\n  accounts.google.com. There is no read-only variant: display-video is read AND write AND delete\n  in a single grant, which is the most consequential fact in this file for anyone binding an\n  agent to this API.\nschemes:\n  - name: oauth2\n    source: openapi/google-display-video-360-api-openapi.yml\n    flows:\n      - flow: authorizationCode\n      \
  \  authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n        refreshUrl: https://oauth2.googleapis.com/token\n    authorization_server_metadata: well-known/google-display-video-360-oauth-authorization-server.json\n    pkce: supported (S256)\nscopes:\n  - scope: https://www.googleapis.com/auth/display-video\n    description: Create, see, edit, and permanently delete your Display & Video 360 entities and reports\n    flows: [authorizationCode]\n    grants: read+write+delete\n    note: >-\n      The default scope for the API and the one most integrations request. It is not\n      least-privilege: there is no read-only counterpart, so an agent that only needs to report\n      on campaigns still receives permanent-delete authority over every entity the user can see.\n      Constrain that at the DV360 user-profile layer instead — a profile with \"Read only\"\n      permission on the advertiser cannot write regardless of the\
  \ scope on the token.\n    sources: [openapi/google-display-video-360-api-openapi.yml, discovery]\n  - scope: https://www.googleapis.com/auth/display-video-mediaplanning\n    description: Create, see, and edit Display & Video 360 Campaign entities and see billing invoices\n    flows: [authorizationCode]\n    grants: read+write on campaign entities, read on invoices\n    note: >-\n      The narrower of the two generally-grantable scopes. Covers the\n      campaign/insertion-order/line-item planning surface and invoice reads without the delete\n      authority the full display-video scope carries. Prefer it for planning and reporting.\n    sources: [openapi/google-display-video-360-api-openapi.yml, discovery]\n  - scope: https://www.googleapis.com/auth/display-video-user-management\n    description: 'Private Service: https://www.googleapis.com/auth/display-video-user-management'\n    flows: [authorizationCode]\n    grants: read+write on DV360 user profiles and role assignments\n    private:\
  \ true\n    note: >-\n      Google marks this a Private Service in its own Discovery Document — it is allowlist-gated\n      and not grantable by a standard OAuth client. It backs the /v4/users resource\n      (usersList, usersGet, usersCreate, usersPatch, usersDelete,\n      usersBulkEditAssignedUserRoles). Those operations are in the contract and will\n      authenticate, but will not authorize for a project that has not been allowlisted.\n    sources: [openapi/google-display-video-360-api-openapi.yml, discovery]\n  - scope: https://www.googleapis.com/auth/doubleclickbidmanager\n    description: View and manage your reports in DoubleClick Bid Manager\n    flows: [authorizationCode]\n    grants: read+write on Bid Manager reporting\n    note: >-\n      Reporting scope inherited from the Bid Manager API\n      (doubleclickbidmanager.googleapis.com), which is where DV360 reporting actually lives. It\n      is declared on this API's Discovery Document, but the reporting operations themselves\
  \ are\n      served by that sibling API rather than by displayvideo.googleapis.com.\n    sources: [discovery]\nscope_count: 4\nread_only_scope_available: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-display-video-360/refs/heads/main/scopes/google-display-video-360-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Campaign Management
- Display Ads
- DV360
- Programmatic Advertising
- Targeting
- Video Ads
- Advertising
- AdTech
- Demand-Side Platform
- Media Buying
- Audiences
- Google Marketing Platform
token_urls:
- https://oauth2.googleapis.com/token
---
