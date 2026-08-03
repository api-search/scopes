---
authorization_urls: []
description: ''
docs: https://docs.maymobility.com/docs/fleet-api/connecting-to-fleet-api
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: May Mobility Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'May Mobility uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: May Mobility
provider_slug: may-mobility
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: null
    tokenUrl_note: Issued per account by the Fleet API team; documented in code samples as 'provided-by-fleet-api-team'.
  name: cognitoClientCredentials
  source: https://docs.maymobility.com/docs/fleet-api/connecting-to-fleet-api
scope_count: 0
scope_names: []
scopes: []
slug: may-mobility-scopes
source_filename: may-mobility-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://docs.maymobility.com/docs/fleet-api/connecting-to-fleet-api\ndocs: https://docs.maymobility.com/docs/fleet-api/connecting-to-fleet-api\ngrant: clientCredentials\nidentity_provider: AWS Cognito\nschemes:\n- name: cognitoClientCredentials\n  source: https://docs.maymobility.com/docs/fleet-api/connecting-to-fleet-api\n  flows:\n  - flow: clientCredentials\n    tokenUrl: null\n    tokenUrl_note: Issued per account by the Fleet API team; documented in code\n      samples as 'provided-by-fleet-api-team'.\nscopes: []\nscopes_note: 'May Mobility documents that an OAuth 2.0 `scope` is REQUIRED on every\n  token request and that the required scope DIFFERS between the Realtime and Batch\n  surfaces — but it does not publish any scope string. Every published reference\n  writes the value as `provided-by-fleet-api-team`. No scope values have been\n  invented here; the list is deliberately empty.'\nscope_classes:\n- class: realtime\n\
  \  description: Scope used to authorize the WebSocket Realtime API (telemetry and\n    video modes).\n  values_published: false\n  evidence: https://docs.maymobility.com/docs/fleet-api/connecting-to-fleet-api\n- class: batch\n  description: Scope used to authorize the Batch (REST) endpoints. Documented\n    separately on the last-active, shift-timing and LiDAR pages, each of which states\n    that the scope required \"may differ from the real-time API endpoints\" and that\n    the batch scope must be used.\n  values_published: false\n  evidence:\n  - https://docs.maymobility.com/docs/fleet-api/topics-channels/last-active\n  - https://docs.maymobility.com/docs/fleet-api/topics-channels/vehicle-shift-timing\n  - https://docs.maymobility.com/docs/fleet-api/topics-channels/lidar\n  quote: 'Scope: Scope to get authorization to this endpoint might vary with other\n    endpoints.'\nx-findings:\n- id: scope-values-unpublished\n  severity: medium\n  detail: 'A per-surface scope model exists and\
  \ is enforced, but no scope name is\n    published anywhere in the documentation. A consumer cannot determine, before\n    contacting the Fleet API team, what authority a token will carry or how narrowly\n    it can be scoped. This is the single largest documentation gap in the May\n    Mobility auth contract, and it also blocks any least-privilege review of an\n    agent integration against a safety-relevant fleet surface.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/may-mobility/refs/heads/main/scopes/may-mobility-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Autonomous Vehicles
- Transportation
- Mobility
- Robotaxi
- Fleet Management
- Telemetry
- Public Transit
- Automotive
- Streaming
token_urls: []
---
