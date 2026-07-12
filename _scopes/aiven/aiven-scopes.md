---
authorization_urls:
- https://console.aiven.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Aiven Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aiven publishes 34 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aiven API on a user''s behalf.


  Tokens are issued from https://api.aiven.io/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aiven
provider_slug: aiven
schemes:
- description: OAuth2 security scheme
  flows:
  - authorizationUrl: https://console.aiven.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.aiven.io/v1/oauth2/token
  name: oauth2
  source: openapi/aiven-aiven-api-openapi.yml
scope_count: 34
scope_names:
- accounts
- accounts:read
- accounts:write
- all
- authentication
- authentication:read
- authentication:write
- billing
- billing:read
- billing:write
- payments
- payments:read
- payments:write
- privatelink
- privatelink:read
- privatelink:write
- projects
- projects:read
- projects:write
- scim
- scim:read
- scim:write
- services
- services:read
- services:write
- static_ips
- static_ips:read
- static_ips:write
- tickets
- tickets:read
- tickets:write
- user
- user:read
- user:write
scopes:
- description: Allow enumerating and reading accounts configuration
  flows:
  - authorizationCode
  scope: accounts
- description: Allow modifying account configuration
  flows:
  - authorizationCode
  scope: accounts:read
- description: Provides full access to authentication related API
  flows:
  - authorizationCode
  scope: accounts:write
- description: Provide full access to the API
  flows:
  - authorizationCode
  scope: all
- description: Provides full access to authentication related API
  flows:
  - authorizationCode
  scope: authentication
- description: Allow reading authentication related configuration on resources (user profile, accounts)
  flows:
  - authorizationCode
  scope: authentication:read
- description: Allow modifying authentication related configurations on resources (user profile, accounts)
  flows:
  - authorizationCode
  scope: authentication:write
- description: Provide full access to billing APIs
  flows:
  - authorizationCode
  scope: billing
- description: Allow reading billing information and configuration
  flows:
  - authorizationCode
  scope: billing:read
- description: Allow writing billing configuration
  flows:
  - authorizationCode
  scope: billing:write
- description: Provide full access to payment method APIs
  flows:
  - authorizationCode
  scope: payments
- description: Allow reading the payment method configurations
  flows:
  - authorizationCode
  scope: payments:read
- description: Allows writing payment method configuration
  flows:
  - authorizationCode
  scope: payments:write
- description: Provide full access to private link APIs
  flows:
  - authorizationCode
  scope: privatelink
- description: Allow enumerating and reading private link items and configurations
  flows:
  - authorizationCode
  scope: privatelink:read
- description: Allow writing (creating, modifying, deleting) private link items
  flows:
  - authorizationCode
  scope: privatelink:write
- description: Provide full access to projects APIs
  flows:
  - authorizationCode
  scope: projects
- description: Allow enumerating projects and reading their configuration
  flows:
  - authorizationCode
  scope: projects:read
- description: Allow writing (creating, modifying, deleting) projects
  flows:
  - authorizationCode
  scope: projects:write
- description: Provide full access to SCIM operations
  flows:
  - authorizationCode
  scope: scim
- description: Allow reading SCIM endpoints
  flows:
  - authorizationCode
  scope: scim:read
- description: Allow writing (modifying) SCIM endpoints
  flows:
  - authorizationCode
  scope: scim:write
- description: Provide full access to services APIs
  flows:
  - authorizationCode
  scope: services
- description: Allow enumerating services and reading their configuration
  flows:
  - authorizationCode
  scope: services:read
- description: Allow writing (creating, modifying, deleting) services
  flows:
  - authorizationCode
  scope: services:write
- description: Provide full access to static IPs APIs
  flows:
  - authorizationCode
  scope: static_ips
- description: Allow enumerating and reading static IP items and configurations
  flows:
  - authorizationCode
  scope: static_ips:read
- description: Allow writing (creating, modifying, deleting) static IP items
  flows:
  - authorizationCode
  scope: static_ips:write
- description: Provide full access to support ticket APIs
  flows:
  - authorizationCode
  scope: tickets
- description: Allow enumerating and reading support tickets
  flows:
  - authorizationCode
  scope: tickets:read
- description: Allow writing (creating, modifying) support tickets
  flows:
  - authorizationCode
  scope: tickets:write
- description: Provide full access to user profile APIs
  flows:
  - authorizationCode
  scope: user
- description: Allow reading user profile and configuration
  flows:
  - authorizationCode
  scope: user:read
- description: Allow writing (modifying) user profile and configuration
  flows:
  - authorizationCode
  scope: user:write
slug: aiven-scopes
source_filename: aiven-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aiven-aiven-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/aiven-aiven-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://console.aiven.io/oauth/authorize\n    tokenUrl: https://api.aiven.io/v1/oauth2/token\n  description: OAuth2 security scheme\nscopes:\n- scope: accounts\n  description: Allow enumerating and reading accounts configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: accounts:read\n  description: Allow modifying account configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: accounts:write\n  description: Provides full access to authentication related API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: all\n  description: Provide full access to the API\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/aiven-aiven-api-openapi.yml\n- scope: authentication\n  description: Provides full access to authentication related API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: authentication:read\n  description: Allow reading authentication related configuration on resources (user profile,\n    accounts)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: authentication:write\n  description: Allow modifying authentication related configurations on resources (user profile,\n    accounts)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: billing\n  description: Provide full access to billing APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: billing:read\n  description: Allow reading billing information and configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n\
  - scope: billing:write\n  description: Allow writing billing configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: payments\n  description: Provide full access to payment method APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: payments:read\n  description: Allow reading the payment method configurations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: payments:write\n  description: Allows writing payment method configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: privatelink\n  description: Provide full access to private link APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: privatelink:read\n  description: Allow enumerating and reading private link items and configurations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n\
  - scope: privatelink:write\n  description: Allow writing (creating, modifying, deleting) private link items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: projects\n  description: Provide full access to projects APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: projects:read\n  description: Allow enumerating projects and reading their configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: projects:write\n  description: Allow writing (creating, modifying, deleting) projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: scim\n  description: Provide full access to SCIM operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: scim:read\n  description: Allow reading SCIM endpoints\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n\
  - scope: scim:write\n  description: Allow writing (modifying) SCIM endpoints\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: services\n  description: Provide full access to services APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: services:read\n  description: Allow enumerating services and reading their configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: services:write\n  description: Allow writing (creating, modifying, deleting) services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: static_ips\n  description: Provide full access to static IPs APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: static_ips:read\n  description: Allow enumerating and reading static IP items and configurations\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/aiven-aiven-api-openapi.yml\n- scope: static_ips:write\n  description: Allow writing (creating, modifying, deleting) static IP items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: tickets\n  description: Provide full access to support ticket APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: tickets:read\n  description: Allow enumerating and reading support tickets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: tickets:write\n  description: Allow writing (creating, modifying) support tickets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: user\n  description: Provide full access to user profile APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: user:read\n  description: Allow reading user profile and configuration\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n- scope: user:write\n  description: Allow writing (modifying) user profile and configuration\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aiven-aiven-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiven/refs/heads/main/scopes/aiven-scopes.yml
summary_line: 34 scopes · authorizationCode
tags:
- Managed Data Infrastructure
- Apache Kafka
- PostgreSQL
- OpenSearch
- ClickHouse
- Redis
- MySQL
- Open Source
- Cloud Database
- DBaaS
- Data Streaming
- Data Platform
token_urls:
- https://api.aiven.io/v1/oauth2/token
---
