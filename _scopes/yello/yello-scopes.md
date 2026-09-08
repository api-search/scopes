---
authorization_urls:
- https://www.wayup.com/api/v1/oauth/o/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Yello Scopes
name_suffix: OAuth Scopes
note: The authorization server advertises exactly one scope. No scopes/permissions reference page was found on wayup.com or yello.co, so no descriptions beyond the observed value are asserted.
overview: 'Yello publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Yello API on a user''s behalf.


  Tokens are issued from https://www.wayup.com/api/v1/oauth/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Yello
provider_slug: yello
schemes:
- flows:
  - authorizationUrl: https://www.wayup.com/api/v1/oauth/o/authorize/
    flow: authorizationCode
    tokenUrl: https://www.wayup.com/api/v1/oauth/o/token/
  name: wayup-mcp-oauth
  source: well-known/yello-wayup-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: The only scope advertised in scopes_supported by both the authorization-server metadata and the protected-resource metadata; grants access to the WayUp MCP endpoint.
  flows:
  - authorizationCode
  scope: mcp
slug: yello-scopes
source_filename: yello-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://www.wayup.com/.well-known/oauth-authorization-server\nnote: >-\n  The authorization server advertises exactly one scope. No scopes/permissions reference page was\n  found on wayup.com or yello.co, so no descriptions beyond the observed value are asserted.\nschemes:\n- name: wayup-mcp-oauth\n  source: well-known/yello-wayup-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wayup.com/api/v1/oauth/o/authorize/\n    tokenUrl: https://www.wayup.com/api/v1/oauth/o/token/\nscopes:\n- scope: mcp\n  description: >-\n    The only scope advertised in scopes_supported by both the authorization-server metadata and the\n    protected-resource metadata; grants access to the WayUp MCP endpoint.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/yello-wayup-oauth-authorization-server.json\n  - well-known/yello-wayup-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yello/refs/heads/main/scopes/yello-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Talent Acquisition
- Recruiting
- Human Resources
- Campus Recruiting
- Applicant Tracking
- Recruitment CRM
- Interview Scheduling
- Jobs
- Model Context Protocol
- Government
token_urls:
- https://www.wayup.com/api/v1/oauth/o/token/
---
