---
authorization_urls: []
description: The single OAuth scope advertised by the authorization server metadata the site serves. Advanced Aircraft Company publishes no scope reference page; this is read verbatim from scopes_supported in the RFC 8414 document. The RFC 9728 protected-resource document independently advertises the same single scope.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Advanced Aircraft Company Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Advanced Aircraft Company publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Advanced Aircraft Company API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Advanced Aircraft Company
provider_slug: advanced-aircraft-company
schemes: []
scope_count: 1
scope_names:
- mcp
scopes:
- description: Grants a client access to the Model Context Protocol server at https://advancedaircraftcompany.com/wp-json/mcp/mcp-oauth-server. The metadata offers no finer granularity — there is no read/write split and no per-ability scope. The effective permissions behind this scope are whatever the WordPress Abilities API exposes to the granting user, which could not be enumerated anonymously (GET /wp-json/wp-abilities/v1/abilities returns 401).
  flows: []
  scope: mcp
slug: advanced-aircraft-company-scopes
source_filename: advanced-aircraft-company-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://advancedaircraftcompany.com/.well-known/oauth-authorization-server\nname: Advanced Aircraft Company OAuth Scopes\ndescription: >-\n  The single OAuth scope advertised by the authorization server metadata the site serves. Advanced\n  Aircraft Company publishes no scope reference page; this is read verbatim from scopes_supported in\n  the RFC 8414 document. The RFC 9728 protected-resource document independently advertises the same\n  single scope.\ndocs: null\ndocs_note: No provider-published scopes or permissions reference exists.\nissuer: https://advancedaircraftcompany.com\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Grants a client access to the Model Context Protocol server at\n    https://advancedaircraftcompany.com/wp-json/mcp/mcp-oauth-server. The metadata offers no finer\n    granularity — there is no read/write split and no per-ability scope. The effective permissions\n    behind this scope are\
  \ whatever the WordPress Abilities API exposes to the granting user, which\n    could not be enumerated anonymously (GET /wp-json/wp-abilities/v1/abilities returns 401).\n  source: scopes_supported\n  evidence: https://advancedaircraftcompany.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanced-aircraft-company/refs/heads/main/scopes/advanced-aircraft-company-scopes.yml
summary_line: 1 scope
tags:
- Company
- Aerospace
- Defense
- Drones
- Unmanned Aircraft Systems
- UAV
- VTOL
- Manufacturing
- Public Safety
token_bound: false
token_urls: []
---
