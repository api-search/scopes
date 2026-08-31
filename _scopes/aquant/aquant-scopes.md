---
api_specs:
- filename: aquant-agent-data-api-openapi.yml
  format: yaml
  label: Aquant Agent Data API
  slug: aquant-agent-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-agent-data-api-openapi.yml
- filename: aquant-asset-location-api-openapi.yml
  format: yaml
  label: Aquant Asset Location API
  slug: aquant-asset-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-asset-location-api-openapi.yml
- filename: aquant-health-api-openapi.yml
  format: yaml
  label: Aquant Health API
  slug: aquant-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-health-api-openapi.yml
- filename: aquant-next-symptom-api-openapi.yml
  format: yaml
  label: Aquant Next Symptom API
  slug: aquant-next-symptom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-next-symptom-api-openapi.yml
- filename: aquant-observation-existence-api-openapi.yml
  format: yaml
  label: Aquant Observation Existence API
  slug: aquant-observation-existence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-observation-existence-api-openapi.yml
- filename: aquant-part-catalog-lookup-api-openapi.yml
  format: yaml
  label: Aquant Part Catalog Lookup API
  slug: aquant-part-catalog-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-part-catalog-lookup-api-openapi.yml
- filename: aquant-part-info-api-openapi.yml
  format: yaml
  label: Aquant Part Info API
  slug: aquant-part-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-part-info-api-openapi.yml
- filename: aquant-part-sources-api-openapi.yml
  format: yaml
  label: Aquant Part Sources API
  slug: aquant-part-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-part-sources-api-openapi.yml
- filename: aquant-preventive-maintenance-check-list-api-openapi.yml
  format: yaml
  label: Aquant Preventive Maintenance Check List API
  slug: aquant-preventive-maintenance-check-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-preventive-maintenance-check-list-api-openapi.yml
- filename: aquant-summary-report-api-openapi.yml
  format: yaml
  label: Aquant Summary Report API
  slug: aquant-summary-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-summary-report-api-openapi.yml
- filename: aquant-technician-proximity-api-openapi.yml
  format: yaml
  label: Aquant Technician Proximity API
  slug: aquant-technician-proximity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/openapi/aquant-technician-proximity-api-openapi.yml
authorization_urls:
- https://login.aquant.ai/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
- deviceCode
- password
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Aquant Scopes
name_suffix: OAuth Scopes
note: Neither Aquant OpenAPI declares an oauth2 security scheme, so the mechanical derive pass (0-working/derive-oauth-scopes.py) returns nothing. The only OAuth/OIDC surface Aquant operates is its Okta customer-identity tenant at login.aquant.ai, which is used for human sign-in to the Aquant platform rather than for API authorization. The scopes below are the standard OIDC set advertised by that discovery document — they are recorded because they are real and anonymously discoverable, NOT because they authorize the MCP or ACP APIs.
overview: 'Aquant publishes 7 OAuth 2.0 scopes via the authorizationCode, implicit, deviceCode, password, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aquant API on a user''s behalf.


  Tokens are issued from https://login.aquant.ai/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aquant
provider_slug: aquant
schemes:
- flows:
  - authorizationUrl: https://login.aquant.ai/oauth2/v1/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://login.aquant.ai/oauth2/v1/token
  - authorizationUrl: https://login.aquant.ai/oauth2/v1/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://login.aquant.ai/oauth2/v1/device/authorize
    flow: deviceCode
    tokenUrl: https://login.aquant.ai/oauth2/v1/token
  - flow: password
    tokenUrl: https://login.aquant.ai/oauth2/v1/token
  - flow: refreshToken
    tokenUrl: https://login.aquant.ai/oauth2/v1/token
  issuer: https://login.aquant.ai
  name: aquant-okta
  source: well-known/aquant-openid-configuration.json
  type: openIdConnect
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- groups
scopes:
- description: Required to obtain an ID token; identifies the request as an OpenID Connect request.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: openid
- description: Access to default profile claims (name, family_name, given_name, locale, zoneinfo, updated_at).
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: profile
- description: Access to the email and email_verified claims.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: email
- description: Access to the address claim.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: address
- description: Access to the phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: phone
- description: Issues a refresh token so the client can renew access without re-prompting the user.
  flows:
  - authorizationCode
  - deviceCode
  - password
  scope: offline_access
- description: Includes the user's group memberships as a claim — the Okta-specific scope Aquant uses for role/tenant assignment.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: groups
slug: aquant-scopes
source_filename: aquant-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://login.aquant.ai/.well-known/openid-configuration\nnote: >-\n  Neither Aquant OpenAPI declares an oauth2 security scheme, so the mechanical derive pass\n  (0-working/derive-oauth-scopes.py) returns nothing. The only OAuth/OIDC surface Aquant\n  operates is its Okta customer-identity tenant at login.aquant.ai, which is used for human\n  sign-in to the Aquant platform rather than for API authorization. The scopes below are the\n  standard OIDC set advertised by that discovery document — they are recorded because they are\n  real and anonymously discoverable, NOT because they authorize the MCP or ACP APIs.\napplies_to: platform sign-in (login.aquant.ai) — not aquant:mcp-server or aquant:acp-voiceai\nschemes:\n- name: aquant-okta\n  type: openIdConnect\n  issuer: https://login.aquant.ai\n  source: well-known/aquant-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.aquant.ai/oauth2/v1/authorize\n\
  \    tokenUrl: https://login.aquant.ai/oauth2/v1/token\n    pkce: S256\n  - flow: implicit\n    authorizationUrl: https://login.aquant.ai/oauth2/v1/authorize\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.aquant.ai/oauth2/v1/device/authorize\n    tokenUrl: https://login.aquant.ai/oauth2/v1/token\n  - flow: password\n    tokenUrl: https://login.aquant.ai/oauth2/v1/token\n  - flow: refreshToken\n    tokenUrl: https://login.aquant.ai/oauth2/v1/token\nscopes:\n- scope: openid\n  description: Required to obtain an ID token; identifies the request as an OpenID Connect request.\n  flows: [authorizationCode, implicit, deviceCode, password]\n  sources: [well-known/aquant-openid-configuration.json]\n- scope: profile\n  description: Access to default profile claims (name, family_name, given_name, locale, zoneinfo, updated_at).\n  flows: [authorizationCode, implicit, deviceCode, password]\n  sources: [well-known/aquant-openid-configuration.json]\n- scope: email\n  description: Access\
  \ to the email and email_verified claims.\n  flows: [authorizationCode, implicit, deviceCode, password]\n  sources: [well-known/aquant-openid-configuration.json]\n- scope: address\n  description: Access to the address claim.\n  flows: [authorizationCode, implicit, deviceCode, password]\n  sources: [well-known/aquant-openid-configuration.json]\n- scope: phone\n  description: Access to the phone_number and phone_number_verified claims.\n  flows: [authorizationCode, implicit, deviceCode, password]\n  sources: [well-known/aquant-openid-configuration.json]\n- scope: offline_access\n  description: Issues a refresh token so the client can renew access without re-prompting the user.\n  flows: [authorizationCode, deviceCode, password]\n  sources: [well-known/aquant-openid-configuration.json]\n- scope: groups\n  description: Includes the user's group memberships as a claim — the Okta-specific scope Aquant uses for role/tenant assignment.\n  flows: [authorizationCode, implicit, deviceCode, password]\n\
  \  sources: [well-known/aquant-openid-configuration.json]\ngaps:\n- >-\n  No API-level scope surface exists. The MCP server and the ACP/VoiceAI API authorize by\n  API key/secret and tenant_id, with no scope vocabulary published for either.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aquant/refs/heads/main/scopes/aquant-scopes.yml
summary_line: 7 scopes · authorizationCode/implicit/deviceCode/password/refreshToken
tags:
- Company
- Artificial Intelligence
- Agents
- Field Service
- Service Management
- Manufacturing
- Medical Devices
- Industrial Equipment
- Knowledge-Management
- Voice AI
- MCP
- Predictive Maintenance
token_urls:
- https://login.aquant.ai/oauth2/v1/token
---
