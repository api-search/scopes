---
authorization_urls: []
description: Scope surface read directly from the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata served at www.reedsemi.com. The deployment declares exactly one scope. There is no published scopes/permissions reference page — Reed operates no developer portal — so the metadata documents are the only source.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Reed Semiconductor Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Reed Semiconductor uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Reed Semiconductor
provider_slug: reed-semiconductor
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: reed-semiconductor-scopes
source_filename: reed-semiconductor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://www.reedsemi.com/.well-known/oauth-authorization-server\nname: Reed Semiconductor OAuth Scopes\ndescription: >-\n  Scope surface read directly from the RFC 8414 authorization-server metadata and the\n  RFC 9728 protected-resource metadata served at www.reedsemi.com. The deployment\n  declares exactly one scope. There is no published scopes/permissions reference page\n  — Reed operates no developer portal — so the metadata documents are the only source.\nissuer: https://www.reedsemi.com\ndocs: null\ndocs_note: >-\n  No scopes or permissions reference is published. Reed Semiconductor runs no developer\n  documentation site; the OAuth surface exists only as plugin-emitted metadata.\nauthorization_endpoint: https://www.reedsemi.com/wp-admin/admin.php?page=novamira-oauth-authorize\ntoken_endpoint: https://www.reedsemi.com/wp-json/novamira/v1/oauth/token\nflows:\n- type: authorization_code\n  pkce: required\n  code_challenge_methods:\n\
  \  - S256\n- type: refresh_token\n- type: device_code\n  grant: 'urn:ietf:params:oauth:grant-type:device_code'\n  device_authorization_endpoint: https://www.reedsemi.com/wp-json/novamira/v1/oauth/device\ntoken_endpoint_auth_methods:\n- none\ndynamic_client_registration:\n  supported: true\n  endpoint: https://www.reedsemi.com/wp-json/novamira/v1/oauth/register\n  note: RFC 7591 dynamic client registration is open — no pre-registration required.\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    The only scope the authorization server advertises. Grants access to the Model\n    Context Protocol server at /wp-json/mcp/novamira-oauth and to the WordPress\n    Abilities API at /wp-json/wp-abilities/v1/*, both of which return\n    rest_oauth_required without it.\n  resources:\n  - https://www.reedsemi.com/wp-json/mcp/novamira-oauth\n  - https://www.reedsemi.com/wp-json/wp-abilities/v1/abilities\n  source: '.well-known/oauth-authorization-server -> scopes_supported'\nfindings:\n \
  \ granularity: coarse\n  note: >-\n    A single undifferentiated scope covers the whole agent surface. Because the tool\n    list is gated, a client cannot tell before authorizing what capabilities \"mcp\"\n    actually confers — there is no read/write split and no per-tool scope.\nx-evidence:\n  fetched: '2026-08-26'\n  probes:\n  - url: https://www.reedsemi.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://www.reedsemi.com/.well-known/oauth-protected-resource\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reed-semiconductor/refs/heads/main/scopes/reed-semiconductor-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Semiconductors
- Power Management
- Electronic Components
- Data-Center
- Artificial Intelligence
- Automotive
- Hardware
- Manufacturing
- Product Catalog
token_urls: []
---
