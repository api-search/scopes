---
api_specs:
- filename: cohesity-cluster-v2-openapi.yml
  format: yaml
  label: Cohesity Helios REST API
  slug: helios-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohesity/refs/heads/main/openapi/cohesity-cluster-v2-openapi.yml
- filename: cohesity-cluster-v1-openapi.yml
  format: yaml
  label: Cohesity DataProtect REST API
  slug: dataprotect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohesity/refs/heads/main/openapi/cohesity-cluster-v1-openapi.yml
- filename: cohesity-helios-reporting-openapi.yml
  format: yaml
  label: Cohesity Helios Reporting API
  slug: helios-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohesity/refs/heads/main/openapi/cohesity-helios-reporting-openapi.yml
- filename: cohesity-site-continuity-openapi.yml
  format: yaml
  label: Cohesity Site Continuity API
  slug: site-continuity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cohesity/refs/heads/main/openapi/cohesity-site-continuity-openapi.yml
authorization_urls:
- https://helios.cohesity.com/oauth2/authorize
description: ''
docs: https://developers.cohesity.com/docs/getting-started
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cohesity Scopes
name_suffix: OAuth Scopes
note: The published Cohesity OpenAPI documents declare only an apiKey security scheme and carry no oauth2 flows, so derive-oauth-scopes.py returned nothing. The scope set below was read from the live OIDC / RFC 8414 discovery documents Helios serves, which is where Cohesity's OAuth surface is actually described. Scope descriptions are NOT published by Cohesity - the discovery documents list names only - so no description is asserted for the three vendor-specific scopes.
overview: 'Cohesity publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cohesity API on a user''s behalf.


  Tokens are issued from https://helios.cohesity.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cohesity
provider_slug: cohesity
schemes:
- flows:
  - authorizationUrl: https://helios.cohesity.com/oauth2/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://helios.cohesity.com/oauth2/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://helios.cohesity.com
  jwks_uri: https://helios.cohesity.com/oauth2/jwks.json
  name: Helios OAuth 2.0 / OpenID Connect
  revocation_endpoint: https://helios.cohesity.com/oauth2/revoke
  source: well-known/cohesity-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
scope_count: 6
scope_names:
- openid
- email
- profile
- cohesity_user
- cohesity_viewer
- cohesity_gaia_viewer
scopes:
- description: Standard OpenID Connect scope requesting an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OpenID Connect scope releasing the email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Standard OpenID Connect scope releasing the basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: ''
  flows:
  - authorizationCode
  scope: cohesity_user
- description: ''
  flows:
  - authorizationCode
  scope: cohesity_viewer
- description: ''
  flows:
  - authorizationCode
  scope: cohesity_gaia_viewer
slug: cohesity-scopes
source_filename: cohesity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://helios.cohesity.com/.well-known/openid-configuration\ndocs: https://developers.cohesity.com/docs/getting-started\nnote: >-\n  The published Cohesity OpenAPI documents declare only an apiKey security scheme\n  and carry no oauth2 flows, so derive-oauth-scopes.py returned nothing. The scope\n  set below was read from the live OIDC / RFC 8414 discovery documents Helios\n  serves, which is where Cohesity's OAuth surface is actually described. Scope\n  descriptions are NOT published by Cohesity - the discovery documents list names\n  only - so no description is asserted for the three vendor-specific scopes.\nschemes:\n  - name: Helios OAuth 2.0 / OpenID Connect\n    source: well-known/cohesity-openid-configuration.json\n    issuer: https://helios.cohesity.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://helios.cohesity.com/oauth2/authorize\n        tokenUrl: https://helios.cohesity.com/oauth2/token\n\
  \        pkce: [S256]\n    revocation_endpoint: https://helios.cohesity.com/oauth2/revoke\n    jwks_uri: https://helios.cohesity.com/oauth2/jwks.json\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope requesting an ID token.\n    flows: [authorizationCode]\n    standard: oidc-core\n    sources: [well-known/cohesity-openid-configuration.json]\n  - scope: email\n    description: Standard OpenID Connect scope releasing the email and email_verified claims.\n    flows: [authorizationCode]\n    standard: oidc-core\n    sources: [well-known/cohesity-openid-configuration.json]\n  - scope: profile\n    description: Standard OpenID Connect scope releasing the basic profile claims.\n    flows: [authorizationCode]\n    standard: oidc-core\n    sources: [well-known/cohesity-openid-configuration.json]\n  - scope: cohesity_user\n    description:\
  \ null\n    flows: [authorizationCode]\n    sources: [well-known/cohesity-openid-configuration.json, well-known/cohesity-oauth-protected-resource.json]\n    note: Vendor-specific Cohesity scope; no description published in the discovery document or the docs.\n  - scope: cohesity_viewer\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cohesity-openid-configuration.json, well-known/cohesity-oauth-protected-resource.json]\n    note: Vendor-specific Cohesity scope; no description published.\n  - scope: cohesity_gaia_viewer\n    description: null\n    flows: [authorizationCode]\n    sources: [well-known/cohesity-openid-configuration.json, well-known/cohesity-oauth-protected-resource.json]\n    note: >-\n      Vendor-specific Gaia read scope. The Cohesity Gaia MCP connector reference\n      separately states that all Gaia MCP tools require the GAIA_VIEW privilege;\n      no Cohesity document states the relationship between that privilege and this\n      scope,\
  \ so none is asserted here.\nprotected_resource:\n  resource: https://helios.cohesity.com\n  resource_name: Cohesity Data Cloud\n  authorization_servers: [https://helios.cohesity.com]\n  bearer_methods_supported: [header]\n  source: well-known/cohesity-oauth-protected-resource.json\n  spec: RFC 9728\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cohesity/refs/heads/main/scopes/cohesity-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Automation
- Backup
- Cyber Resilience
- Data Management
- Data Protection
- Data Security
- DataProtect
- Disaster Recovery
- Helios
- Orchestration
- Ransomware Recovery
- Site Continuity
- Reporting
- Model Context Protocol
- Enterprise Storage
token_urls:
- https://helios.cohesity.com/oauth2/token
---
