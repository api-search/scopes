---
authorization_urls: []
description: ''
docs: https://docs.bodygram.com/platform/api-reference
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Original Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bodygram publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bodygram API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bodygram
provider_slug: original
schemes: []
scope_count: 2
scope_names:
- api.platform.bodygram.com/scans:create
- api.platform.bodygram.com/scans:read
scopes:
- description: Create a body scan (submit stats and/or two photos for measurement).
  flows: []
  scope: api.platform.bodygram.com/scans:create
- description: Read a previously created scan's measurements, 3D avatar, and (when photos were provided) body composition and posture data.
  flows: []
  scope: api.platform.bodygram.com/scans:read
slug: original-scopes
source_filename: original-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.bodygram.com/platform/api-reference\ndocs: https://docs.bodygram.com/platform/api-reference\napi: Bodygram Platform API\nstyle: api-key permission scopes\naudience: api.platform.bodygram.com\nscopes:\n- name: api.platform.bodygram.com/scans:create\n  description: Create a body scan (submit stats and/or two photos for measurement).\n- name: api.platform.bodygram.com/scans:read\n  description: >-\n    Read a previously created scan's measurements, 3D avatar, and (when photos were\n    provided) body composition and posture data.\nnotes: >-\n  Scopes are permission strings attached to Bodygram API keys, addressed to the\n  api.platform.bodygram.com audience; the API does not run a full OAuth 2.0\n  authorization-code flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/original/refs/heads/main/scopes/original-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Body Measurement
- Computer Vision
- Artificial Intelligence
- Sizing
- Retail
- 3D Avatar
- Health
- SDK
token_bound: false
token_urls: []
---
