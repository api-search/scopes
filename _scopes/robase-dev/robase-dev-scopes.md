---
api_specs:
- filename: robase-dev-dashboard-api-openapi.yml
  format: yaml
  label: robase-dev Dashboard API
  slug: robase-dev-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-dashboard-api-openapi.yml
- filename: robase-dev-otp-api-openapi.yml
  format: yaml
  label: robase-dev OTP API
  slug: robase-dev-otp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-otp-api-openapi.yml
- filename: robase-dev-sms-api-openapi.yml
  format: yaml
  label: robase-dev SMS API
  slug: robase-dev-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-sms-api-openapi.yml
- filename: robase-dev-system-api-openapi.yml
  format: yaml
  label: robase-dev System API
  slug: robase-dev-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-system-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Robase Dev Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'robase-dev publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the robase-dev API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: robase-dev
provider_slug: robase-dev
schemes: []
scope_count: 5
scope_names:
- otp:send
- otp:verify
- sms:send
- read
- approvals:request
scopes:
- description: Allows POST /v1/otp/send and MCP send_otp
  flows: []
  scope: otp:send
- description: Allows POST /v1/otp/verify and MCP verify_otp
  flows: []
  scope: otp:verify
- description: Allows POST /v1/sms/send and MCP send_sms
  flows: []
  scope: sms:send
- description: Allows GET /v1/otp/{id}, GET /v1/sms/{id} and MCP get_* tools
  flows: []
  scope: read
- description: Reserved for approval requests (no endpoint yet)
  flows: []
  scope: approvals:request
slug: robase-dev-scopes
source_filename: robase-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: \"https://docs.robase.dev/concepts/authentication.md\"\nscopes:\n  - name: \"otp:send\"\n    description: \"Allows POST /v1/otp/send and MCP send_otp\"\n  - name: \"otp:verify\"\n    description: \"Allows POST /v1/otp/verify and MCP verify_otp\"\n  - name: \"sms:send\"\n    description: \"Allows POST /v1/sms/send and MCP send_sms\"\n  - name: \"read\"\n    description: \"Allows GET /v1/otp/{id}, GET /v1/sms/{id} and MCP get_* tools\"\n  - name: \"approvals:request\"\n    description: \"Reserved for approval requests (no endpoint yet)\"\n"
source_yaml_url: https://artifacts.apis.io/robase-dev/scopes/robase-dev-scopes.yml
summary_line: 5 scopes
tags:
- SMS
- OTP
- Africa
- Messaging
- API
- Communications
token_bound: false
token_urls: []
---
