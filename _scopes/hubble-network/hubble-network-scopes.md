---
api_specs:
- filename: hubble-network-api-keys-api-openapi.yml
  format: yaml
  label: Hubble Network API Keys API
  slug: hubble-network-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-api-keys-api-openapi.yml
- filename: hubble-network-billing-api-openapi.yml
  format: yaml
  label: Hubble Network Billing API
  slug: hubble-network-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-billing-api-openapi.yml
- filename: hubble-network-devices-api-openapi.yml
  format: yaml
  label: Hubble Network Devices API
  slug: hubble-network-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-devices-api-openapi.yml
- filename: hubble-network-organizations-api-openapi.yml
  format: yaml
  label: Hubble Network Organizations API
  slug: hubble-network-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-organizations-api-openapi.yml
- filename: hubble-network-packet-webhooks-api-openapi.yml
  format: yaml
  label: Hubble Network Packet Webhooks API
  slug: hubble-network-packet-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-packet-webhooks-api-openapi.yml
- filename: hubble-network-packets-api-openapi.yml
  format: yaml
  label: Hubble Network Packets API
  slug: hubble-network-packets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-packets-api-openapi.yml
- filename: hubble-network-platform-metrics-api-openapi.yml
  format: yaml
  label: Hubble Network Platform Metrics API
  slug: hubble-network-platform-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-platform-metrics-api-openapi.yml
authorization_urls: []
description: ''
docs: https://hubble.com/docs/api-specification/hubble-platform-api
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Hubble Network Scopes
name_suffix: OAuth Scopes
note: 'Hubble does NOT implement OAuth 2.0. These are authorization scopes attached to an organization API key at issuance. Recorded here because they are a genuine, enumerable, documented permission surface, retrievable at runtime via GET /v1/org/{org_id}/key_scopes. Default behaviour: a key created with no scopes receives all 16 (admin-level).'
overview: 'Hubble Network publishes 16 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hubble Network API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hubble Network
provider_slug: hubble-network
schemes:
- flows: []
  name: BearerAuth
  source: openapi/hubble-network-platform-openapi.yml
  type: http-bearer-jwt
scope_count: 16
scope_names:
- read-api-keys
- write-api-keys
- read-users
- write-users
- read-organization-metadata
- write-organization-metadata
- read-devices
- write-devices
- read-invitations
- write-invitations
- read-packets
- read-platform-metrics
- read-billing-usage
- read-billing-invoices
- read-webhooks
- write-webhooks
scopes:
- description: View API keys and their metadata
  flows: []
  scope: read-api-keys
- description: Create, update, and delete API keys
  flows: []
  scope: write-api-keys
- description: View user information and roles
  flows: []
  scope: read-users
- description: Add, update, and remove users from the organization
  flows: []
  scope: write-users
- description: View organization details and settings
  flows: []
  scope: read-organization-metadata
- description: Update organization information
  flows: []
  scope: write-organization-metadata
- description: View device information and status
  flows: []
  scope: read-devices
- description: Register and manage devices
  flows: []
  scope: write-devices
- description: View pending invitations
  flows: []
  scope: read-invitations
- description: Create and revoke user invitations
  flows: []
  scope: write-invitations
- description: Access packet data and retrieval endpoints
  flows: []
  scope: read-packets
- description: View platform metrics and analytics
  flows: []
  scope: read-platform-metrics
- description: View billing usage information
  flows: []
  scope: read-billing-usage
- description: View billing invoices
  flows: []
  scope: read-billing-invoices
- description: View webhook configurations
  flows: []
  scope: read-webhooks
- description: Create and manage webhook endpoints
  flows: []
  scope: write-webhooks
slug: hubble-network-scopes
source_filename: hubble-network-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/hubble-network-platform-openapi.yml (components.schemas.authScope)\ndocs: https://hubble.com/docs/api-specification/hubble-platform-api\nmodel: api-key-scopes\nnote: 'Hubble does NOT implement OAuth 2.0. These are authorization scopes attached to an organization\n  API key at issuance. Recorded here because they are a genuine, enumerable, documented permission surface,\n  retrievable at runtime via GET /v1/org/{org_id}/key_scopes. Default behaviour: a key created with no\n  scopes receives all 16 (admin-level).'\nenumeration_endpoint:\n  operationId: list-key-scopes\n  path: /v1/org/{org_id}/key_scopes\n  method: get\nschemes:\n- name: BearerAuth\n  source: openapi/hubble-network-platform-openapi.yml\n  type: http-bearer-jwt\n  flows: []\nscopes:\n- scope: read-api-keys\n  description: View API keys and their metadata\n  access: read\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n\
  - scope: write-api-keys\n  description: Create, update, and delete API keys\n  access: write\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: read-users\n  description: View user information and roles\n  access: read\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: write-users\n  description: Add, update, and remove users from the organization\n  access: write\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: read-organization-metadata\n  description: View organization details and settings\n  access: read\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: write-organization-metadata\n  description: Update organization information\n  access:\
  \ write\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: read-devices\n  description: View device information and status\n  access: read\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: write-devices\n  description: Register and manage devices\n  access: write\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: read-invitations\n  description: View pending invitations\n  access: read\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: write-invitations\n  description: Create and revoke user invitations\n  access: write\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n\
  - scope: read-packets\n  description: Access packet data and retrieval endpoints\n  access: read\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: read-platform-metrics\n  description: View platform metrics and analytics\n  access: read\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: read-billing-usage\n  description: View billing usage information\n  access: read\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: read-billing-invoices\n  description: View billing invoices\n  access: read\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: read-webhooks\n  description: View webhook configurations\n  access: read\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n\
  \  - https://hubble.com/docs/api-specification/hubble-platform-api\n- scope: write-webhooks\n  description: Create and manage webhook endpoints\n  access: write\n  sources:\n  - openapi/hubble-network-platform-openapi.yml\n  - https://hubble.com/docs/api-specification/hubble-platform-api\nexample_combinations:\n- name: Read-only\n  scopes:\n  - read-api-keys\n  - read-users\n  - read-devices\n- name: Device management\n  scopes:\n  - read-devices\n  - write-devices\n- name: User management\n  scopes:\n  - read-users\n  - write-users\n  - read-invitations\n  - write-invitations\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/scopes/hubble-network-scopes.yml
summary_line: 16 scopes
tags:
- Company
- IoT
- Bluetooth
- Satellite
- Connectivity
- Asset Tracking
- Devices
- Networks
- Telemetry
- Logistics
token_urls: []
---
