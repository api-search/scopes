---
api_specs:
- filename: losant-application-api-openapi.yml
  format: yaml
  label: Losant Application API
  slug: losant-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-application-api-openapi.yml
- filename: losant-device-api-openapi.yml
  format: yaml
  label: Losant Device API
  slug: losant-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-device-api-openapi.yml
- filename: losant-experience-api-openapi.yml
  format: yaml
  label: Losant Experience API
  slug: losant-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-experience-api-openapi.yml
- filename: losant-authentication-and-account-api-openapi.yml
  format: yaml
  label: Losant Authentication and Account API
  slug: losant-authentication-and-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-authentication-and-account-api-openapi.yml
- filename: losant-data-and-data-tables-api-openapi.yml
  format: yaml
  label: Losant Data and Data Tables API
  slug: losant-data-and-data-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-data-and-data-tables-api-openapi.yml
- filename: losant-edge-and-embedded-compute-api-openapi.yml
  format: yaml
  label: Losant Edge and Embedded Compute API
  slug: losant-edge-and-embedded-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-edge-and-embedded-compute-api-openapi.yml
- filename: losant-enterprise-instance-api-openapi.yml
  format: yaml
  label: Losant Enterprise Instance API
  slug: losant-enterprise-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-enterprise-instance-api-openapi.yml
- filename: losant-notebooks-api-openapi.yml
  format: yaml
  label: Losant Notebooks API
  slug: losant-notebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-notebooks-api-openapi.yml
- filename: losant-workflow-engine-api-openapi.yml
  format: yaml
  label: Losant Workflow Engine API
  slug: losant-workflow-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-workflow-engine-api-openapi.yml
authorization_urls:
- https://accounts.losant.com/oauth
description: ''
docs: https://docs.losant.com/user-accounts/oauth-tokens/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Losant Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Losant publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Losant API on a user''s behalf.


  Tokens are issued from https://api.losant.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Losant
provider_slug: losant
schemes:
- flows:
  - authorizationUrl: https://accounts.losant.com/oauth
    flow: authorizationCode
    pkce:
    - S256
    registrationUrl: https://api.losant.com/oauth/clients
    response_types:
    - code
    revocationUrl: https://api.losant.com/oauth/revoke
    tokenUrl: https://api.losant.com/oauth/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
    - none
  name: OAuth2
  source: https://api.losant.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 7
scope_names:
- all.Application.read
- all.Application.bounded
- only.Organization.read
- only.Organization.bounded
- all.Organization.read
- all.Organization.bounded
- only.User.read
scopes:
- description: Read-only access to all application data and sub-resources (devices, telemetry data, dashboards, workflows and more).
  flows:
  - authorizationCode
  scope: all.Application.read
- description: Read and write access to all application data and sub-resources, excluding token management, org membership, resource transfer and credential changes.
  flows:
  - authorizationCode
  scope: all.Application.bounded
- description: Read-only access to organizations and a list of their applications, but no access to application sub-resources.
  flows:
  - authorizationCode
  scope: only.Organization.read
- description: Read and write access to organizations and read access to listing their applications, but no access to application sub-resources.
  flows:
  - authorizationCode
  scope: only.Organization.bounded
- description: Read-only access to organizations and all of their application data and sub-resources.
  flows:
  - authorizationCode
  scope: all.Organization.read
- description: Read and write access to organizations and all of their application data and sub-resources.
  flows:
  - authorizationCode
  scope: all.Organization.bounded
- description: Read-only access to the user profile (name, email address, sandbox usage).
  flows:
  - authorizationCode
  scope: only.User.read
slug: losant-scopes
source_filename: losant-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.losant.com/user-accounts/oauth-tokens/\ndocs: https://docs.losant.com/user-accounts/oauth-tokens/\ndiscovery: https://api.losant.com/.well-known/oauth-authorization-server\nnotes: |\n  Losant runs TWO distinct permission models and they are easy to confuse.\n  (1) OAuth 2.0 user scopes - the scopes a third-party application (an MCP client, for example) requests\n      during the consent flow. These are the seven scopes below, authoritative in the scopes_supported\n      field of the RFC 8414 metadata at https://api.losant.com/.well-known/oauth-authorization-server.\n  (2) API token scopes - the per-operation permissions baked into a User/Application/Instance API token\n      (all.User, all.Application, all.Device, all.User.cli, and per-operation names of the form\n      <resource>.<action>, e.g. device.get, devices.post). These are not OAuth scopes; they are captured in\n      token_scopes below and carried per\
  \ operation as operationId in openapi/.\n  The OpenAPI files declare only http bearer security, so this file was NOT derivable from the specs -\n  derive-oauth-scopes.py found zero oauth2 schemes. It is written from the provider's published scope\n  reference plus the live authorization-server metadata.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    source: https://api.losant.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.losant.com/oauth\n        tokenUrl: https://api.losant.com/oauth/token\n        revocationUrl: https://api.losant.com/oauth/revoke\n        registrationUrl: https://api.losant.com/oauth/clients\n        pkce: [S256]\n        response_types: [code]\n        token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\nscopes:\n  - scope: all.Application.read\n    description: Read-only access to all application data and sub-resources (devices, telemetry data, dashboards,\
  \ workflows and more).\n    flows: [authorizationCode]\n  - scope: all.Application.bounded\n    description: Read and write access to all application data and sub-resources, excluding token management, org membership, resource transfer and credential changes.\n    flows: [authorizationCode]\n  - scope: only.Organization.read\n    description: Read-only access to organizations and a list of their applications, but no access to application sub-resources.\n    flows: [authorizationCode]\n  - scope: only.Organization.bounded\n    description: Read and write access to organizations and read access to listing their applications, but no access to application sub-resources.\n    flows: [authorizationCode]\n  - scope: all.Organization.read\n    description: Read-only access to organizations and all of their application data and sub-resources.\n    flows: [authorizationCode]\n  - scope: all.Organization.bounded\n    description: Read and write access to organizations and all of their application\
  \ data and sub-resources.\n    flows: [authorizationCode]\n  - scope: only.User.read\n    description: Read-only access to the user profile (name, email address, sandbox usage).\n    flows: [authorizationCode]\nbounded_semantics:\n  description: |\n    A .bounded scope grants read and write access to the resources it covers but excludes a fixed set of\n    sensitive actions.\n  excluded_actions:\n    - managing API tokens\n    - managing organization members and invitations\n    - transferring resources\n    - changing account credentials\n  immutability: A token's scope cannot be changed after authorization; a new authorization flow is required to add scopes.\n  permission_cap: |\n    Beyond scope, every OAuth token carries a Default Maximum Client Role that caps the role it may assume\n    in each organization, with per-organization and per-application overrides. A token can never exceed the\n    permissions its owning user holds; if the user's role is reduced later, the token's effective\n\
  \    permissions are reduced with it.\ntoken_scopes:\n  description: |\n    API token (non-OAuth) scopes, published in the Bravado API schema at https://api.losant.com/ as the\n    `auth` value on each operation and as `authGroups`. Each operation carries a per-operation scope named\n    <resource>.<action>; wildcards (<resource>.*) and the named groups below are also accepted.\n  broad:\n    - {scope: all.User, description: 'Full access to everything the authenticating user can do.'}\n    - {scope: all.Application, description: 'Full access within one application; the default for application API tokens.'}\n    - {scope: all.Device, description: 'Device-scoped token issued by POST /auth/device; limited to the device (and its peers under the access key).'}\n    - {scope: all.User.cli, description: 'The exact permission set the Losant CLI needs; the \"CLI developer\" option in the UI.'}\n  groups_deprecated:\n    source: 'deprecatedAuthScopes in https://api.losant.com/'\n    scopes: [applications,\
  \ dashboards, dashboards.read, devices, devices.read, devices.state, devices.command, events, flows, me, orgs, webhooks]\n  per_operation_example:\n    - {scope: device.get, grants: 'GET /applications/{applicationId}/devices/{deviceId}'}\n    - {scope: devices.post, grants: 'POST /applications/{applicationId}/devices'}\n    - {scope: data.timeSeriesQuery, grants: 'POST /applications/{applicationId}/data/time-series-query'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/scopes/losant-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- IoT
- Internet of Things
- Devices
- Edge Compute
- Embedded
- MQTT
- Industrial IoT
- Telemetry
- Workflow-Automation
- Visual Workflow Engine
- Dashboards
- Time Series
- Connected Products
- Enterprise
token_urls:
- https://api.losant.com/oauth/token
---
