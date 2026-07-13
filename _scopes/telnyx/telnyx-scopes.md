---
api_specs:
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Voice API
  slug: telnyx-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Messaging API
  slug: telnyx-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Numbers API
  slug: telnyx-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Verify API
  slug: telnyx-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Fax API
  slug: telnyx-fax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Wireless API
  slug: telnyx-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Networking API
  slug: telnyx-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx AI API
  slug: telnyx-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Billing & Reporting API
  slug: telnyx-billing-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
authorization_urls:
- https://api.telnyx.com/v2/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Telnyx Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Telnyx publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Telnyx API on a user''s behalf.


  Tokens are issued from https://api.telnyx.com/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Telnyx
provider_slug: telnyx
schemes:
- description: OAuth 2.0 authentication for Telnyx API and MCP integrations
  flows:
  - authorizationUrl: https://api.telnyx.com/v2/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.telnyx.com/v2/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.telnyx.com/v2/oauth/token
  name: oauthClientAuth
  source: openapi/telnyx-openapi.yml
scope_count: 1
scope_names:
- admin
scopes:
- description: Administrative access to Telnyx resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: admin
slug: telnyx-scopes
source_filename: telnyx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telnyx-openapi.yml\nschemes:\n- name: oauthClientAuth\n  source: openapi/telnyx-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.telnyx.com/v2/oauth/authorize\n    tokenUrl: https://api.telnyx.com/v2/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.telnyx.com/v2/oauth/token\n  description: OAuth 2.0 authentication for Telnyx API and MCP integrations\nscopes:\n- scope: admin\n  description: Administrative access to Telnyx resources\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/telnyx-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/scopes/telnyx-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Communications
- CPaaS
- Voice
- SMS
- IoT
token_urls:
- https://api.telnyx.com/v2/oauth/token
---
