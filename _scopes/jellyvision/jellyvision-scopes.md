---
authorization_urls: []
description: ''
docs: https://partner-api-docs.myalex.com/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Jellyvision Scopes
name_suffix: OAuth Scopes
note: Jellyvision does not publish a scope/permission reference page. The single Partner Integration API scope below is read from the decoded JWT access-token example printed in the authentication section of the public API reference. The second scope is read from the RFC 9728 protected-resource metadata served at https://www.jellyvision.com/.well-known/oauth-protected-resource and applies to the MCP server on the marketing site, not to the Partner Integration API.
overview: 'Jellyvision uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jellyvision
provider_slug: jellyvision
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: jellyvision-scopes
source_filename: jellyvision-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://partner-api-docs.myalex.com/\ndocs: https://partner-api-docs.myalex.com/\nnote: >-\n  Jellyvision does not publish a scope/permission reference page. The single Partner Integration API\n  scope below is read from the decoded JWT access-token example printed in the authentication section\n  of the public API reference. The second scope is read from the RFC 9728 protected-resource metadata\n  served at https://www.jellyvision.com/.well-known/oauth-protected-resource and applies to the MCP\n  server on the marketing site, not to the Partner Integration API.\nflows:\n- flow: clientCredentials\n  token_url: https://login.myalex.com/oauth/token\n  audience: https://integrated-partner.myalex.com\n  scopes:\n  - name: 'rw:self'\n    description: >-\n      Read and write the partner's own end-user records and ALEX Sessions. This is the only scope\n      shown in the documented decoded access token; Jellyvision does not publish\
  \ a broader scope\n      catalog, and scope selection is not partner-configurable.\n    source: decoded access_token example, Authentication section of the V1 API Reference\n- flow: authorizationCode\n  resource: https://www.jellyvision.com/wp-json/mcp/mcp-oauth-server\n  authorization_server: https://www.jellyvision.com\n  scopes:\n  - name: mcp\n    description: >-\n      Access the OAuth-protected Model Context Protocol server published on www.jellyvision.com.\n      Advertised in both the authorization-server and protected-resource metadata documents.\n    source: https://www.jellyvision.com/.well-known/oauth-protected-resource\noidc_tenant_scopes:\n  note: >-\n    login.myalex.com is an Auth0 tenant whose OIDC discovery document advertises the standard Auth0\n    scope set. These are tenant defaults, not Partner Integration API permissions, and are recorded\n    here only so they are not mistaken for a published product scope catalog.\n  scopes:\n  - openid\n  - profile\n  - offline_access\n\
  \  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n  - identities\n  - phone\n  - address\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jellyvision/refs/heads/main/scopes/jellyvision-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Employee Benefits
- Human Resources
- Benefits Administration
- Benefits Enrollment
- Health Insurance
- Decision Support
- HR Technology
- Insurance
- Employee Engagement
token_urls: []
---
