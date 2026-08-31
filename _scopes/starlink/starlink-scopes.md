---
api_specs:
- filename: starlink-telemetry-asyncapi.yml
  format: yaml
  label: Starlink Telemetry Stream API
  slug: starlink-telemetry-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/asyncapi/starlink-telemetry-asyncapi.yml
- filename: starlink-account-api-openapi.yml
  format: yaml
  label: Starlink Account API
  slug: starlink-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-account-api-openapi.yml
- filename: starlink-addresses-api-openapi.yml
  format: yaml
  label: Starlink Addresses API
  slug: starlink-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-addresses-api-openapi.yml
- filename: starlink-billing-api-openapi.yml
  format: yaml
  label: Starlink Billing API
  slug: starlink-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-billing-api-openapi.yml
- filename: starlink-contacts-api-openapi.yml
  format: yaml
  label: Starlink Contacts API
  slug: starlink-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-contacts-api-openapi.yml
- filename: starlink-data-pools-api-openapi.yml
  format: yaml
  label: Starlink Data Pools API
  slug: starlink-data-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-data-pools-api-openapi.yml
- filename: starlink-flights-api-openapi.yml
  format: yaml
  label: Starlink Flights API
  slug: starlink-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-flights-api-openapi.yml
- filename: starlink-managed-accounts-api-openapi.yml
  format: yaml
  label: Starlink Managed Accounts API
  slug: starlink-managed-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-managed-accounts-api-openapi.yml
- filename: starlink-managed-api-openapi.yml
  format: yaml
  label: Starlink Managed API
  slug: starlink-managed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-managed-api-openapi.yml
- filename: starlink-mobile-api-openapi.yml
  format: yaml
  label: Starlink Mobile API
  slug: starlink-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-mobile-api-openapi.yml
- filename: starlink-routers-api-openapi.yml
  format: yaml
  label: Starlink Routers API
  slug: starlink-routers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-routers-api-openapi.yml
- filename: starlink-service-lines-api-openapi.yml
  format: yaml
  label: Starlink Service Lines API
  slug: starlink-service-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-service-lines-api-openapi.yml
- filename: starlink-user-terminals-api-openapi.yml
  format: yaml
  label: Starlink User Terminals API
  slug: starlink-user-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-user-terminals-api-openapi.yml
authorization_urls: []
description: ''
docs: https://starlink.readme.io/docs/api-v2-service-accounts
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Starlink Scopes
name_suffix: OAuth Scopes
note: 'Starlink''s identity provider is a full OIDC server and publishes scopes_supported anonymously, but the Starlink Public API V2 itself does NOT authorize on OAuth scopes. Service accounts use the client_credentials grant and are authorized by a role-based PERMISSION set assigned in the Starlink account settings page. The OIDC scopes below belong to the interactive user-facing flows on the same issuer; the permission set below is the real authorization surface for the API and is transcribed from the "Required permission:" line on each operation in the OpenAPI. No fabricated scopes: nothing here was invented.'
overview: 'Starlink publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Starlink API on a user''s behalf.


  Tokens are issued from https://starlink.com/api/auth/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Starlink
provider_slug: starlink
schemes:
- authorizationUrl: https://starlink.com/api/auth/connect/authorize
  flows:
  - flow: clientCredentials
    tokenUrl: https://starlink.com/api/auth/connect/token
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  - delegation
  - login_code
  introspection_endpoint: https://starlink.com/api/auth/connect/introspect
  issuer: https://api.starlink.com/auth
  name: StarlinkServiceAccount
  revocation_endpoint: https://starlink.com/api/auth/connect/revocation
  source: well-known/starlink-openid-configuration.json
  type: oauth2
scope_count: 5
scope_names:
- openid
- email
- phone
- profile
- group
scopes:
- description: OpenID Connect subject identifier
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Email address and email_verified claims
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Phone number and phone_number_verified claims
  flows:
  - authorizationCode
  - implicit
  scope: phone
- description: Standard profile claims (name, family_name, given_name, picture, locale, updated_at)
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Group membership claim
  flows:
  - authorizationCode
  - implicit
  scope: group
slug: starlink-scopes
source_filename: starlink-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://starlink.com/api/auth/.well-known/openid-configuration\ndocs: https://starlink.readme.io/docs/api-v2-service-accounts\nnote: >-\n  Starlink's identity provider is a full OIDC server and publishes scopes_supported anonymously,\n  but the Starlink Public API V2 itself does NOT authorize on OAuth scopes. Service accounts\n  use the client_credentials grant and are authorized by a role-based PERMISSION set assigned in\n  the Starlink account settings page. The OIDC scopes below belong to the interactive user-facing\n  flows on the same issuer; the permission set below is the real authorization surface for the API\n  and is transcribed from the \"Required permission:\" line on each operation in the OpenAPI.\n  No fabricated scopes: nothing here was invented.\nschemes:\n- name: StarlinkServiceAccount\n  type: oauth2\n  source: well-known/starlink-openid-configuration.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://starlink.com/api/auth/connect/token\n  issuer: https://api.starlink.com/auth\n  authorizationUrl: https://starlink.com/api/auth/connect/authorize\n  introspection_endpoint: https://starlink.com/api/auth/connect/introspect\n  revocation_endpoint: https://starlink.com/api/auth/connect/revocation\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  - delegation\n  - login_code\nscopes:\n- scope: openid\n  description: OpenID Connect subject identifier\n  flows: [authorizationCode, implicit]\n  sources: [well-known/starlink-openid-configuration.json]\n- scope: email\n  description: Email address and email_verified claims\n  flows: [authorizationCode, implicit]\n  sources: [well-known/starlink-openid-configuration.json]\n- scope: phone\n  description: Phone number and phone_number_verified claims\n  flows: [authorizationCode, implicit]\n\
  \  sources: [well-known/starlink-openid-configuration.json]\n- scope: profile\n  description: Standard profile claims (name, family_name, given_name, picture, locale, updated_at)\n  flows: [authorizationCode, implicit]\n  sources: [well-known/starlink-openid-configuration.json]\n- scope: group\n  description: Group membership claim\n  flows: [authorizationCode, implicit]\n  sources: [well-known/starlink-openid-configuration.json]\npermissions:\n  model: role-based access control on the V2 service account\n  source: openapi/starlink-public-api-v2-openapi.json\n  entries:\n  - permission: Account information\n    levels: [View, Edit]\n    covers:\n    - GET /public/v2/account\n    - GET/POST /public/v2/addresses\n    - 'GET/PUT /public/v2/addresses/{addressReferenceId}'\n  - permission: Service plan\n    levels: [View, Edit]\n    covers: [service lines, products, data usage, data pools, data blocks, top-ups, proration]\n  - permission: Device management\n    levels: [View, Edit]\n    covers:\
  \ [user terminal inventory on the account]\n  - permission: Device command and configuration\n    levels: [View, Edit]\n    covers: [router configs, TLS configs, local content, sandbox clients and heartbeat, reboots, public IP, L2VPN read]\n  - permission: Device configuration assignment\n    levels: [Edit]\n    covers: [assigning router and user terminal configs, setting L2VPN VLANs]\n  - permission: Device telemetry\n    levels: [View]\n    covers: [POST /public/v2/telemetry/stream, POST /public/v2/telemetry/query]\n  - permission: Financial\n    levels: [View]\n    covers: [invoices, invoice details, account balance]\n  - permission: User management\n    levels: [Edit]\n    covers: [GET /public/v2/contacts]\n  - permission: Admin Only - API User Management\n    levels: [Edit]\n    covers: [create, update and delete contacts]\n  - permission: Managed Account Information\n    levels: [View]\n    covers: [managed account tree and managed account queries]\n  - permission: Aviation flight\
  \ status management\n    levels: [Edit]\n    covers: [POST /public/v2/flights/status]\n  - permission: Gated Feature - Starlink Mobile Data\n    levels: [View]\n    covers: [mobile radio access network, timeseries and map data]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/scopes/starlink-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Telecommunications
- United States
- Satellite
- Broadband
- Non-Terrestrial Networks
- Connectivity
- Device Management
- Telemetry
- Aviation
- Maritime
- Enterprise
token_urls:
- https://starlink.com/api/auth/connect/token
---
