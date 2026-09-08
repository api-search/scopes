---
api_specs:
- filename: vergesense-api-openapi.json
  format: json
  label: VergeSense API
  slug: vergesense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/openapi/vergesense-api-openapi.json
authorization_urls: []
description: ''
docs: https://vergesense.readme.io/reference/reference-getting-started
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Vergesense Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'VergeSense uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: VergeSense
provider_slug: vergesense
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: vergesense-scopes
source_filename: vergesense-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://vergesense.auth0.com/.well-known/openid-configuration\ndocs: https://vergesense.readme.io/reference/reference-getting-started\nsummary: >-\n  The VergeSense REST API has NO OAuth scopes — it is authenticated with a single static header key\n  and authorized by a building selection made when the key is created. The only scope vocabulary\n  anywhere in the estate belongs to the Auth0 tenant that guards the remote MCP server, and it is the\n  stock OIDC/Auth0 set rather than a VergeSense-defined product permission model.\nrest_api:\n  oauth2: false\n  scopes: []\n  authorization_model: building-scoped API key\n  detail: >-\n    An API key is bound at creation to a selected set of buildings, editable afterwards under\n    Integrations > Details. There is no per-endpoint, per-resource or read/write distinction — a key\n    that can read metrics can also create, patch and delete webhooks. An agent holding a VergeSense\n   \
  \ key holds every capability the API exposes for its buildings.\n  source: https://vergesense.readme.io/reference/reference-getting-started\nmcp_authorization_server:\n  issuer: https://vergesense.auth0.com/\n  discovery: https://vergesense.auth0.com/.well-known/openid-configuration\n  protected_resource: https://mcp.vergesense.com/mcp\n  scopes_supported:\n  - {name: openid, description: OIDC authentication}\n  - {name: profile, description: basic profile claims}\n  - {name: offline_access, description: refresh-token issuance}\n  - {name: email, description: email address claim}\n  - {name: email_verified, description: email verification state claim}\n  - {name: name, description: full name claim}\n  - {name: given_name, description: given name claim}\n  - {name: family_name, description: family name claim}\n  - {name: nickname, description: nickname claim}\n  - {name: picture, description: profile picture claim}\n  - {name: created_at, description: account creation timestamp claim}\n\
  \  - {name: identities, description: linked identity claim}\n  - {name: phone, description: phone number claim}\n  - {name: address, description: address claim}\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  - 'urn:ietf:params:oauth:grant-type:token-exchange'\n  dynamic_client_registration: https://vergesense.auth0.com/oidc/register\n  caveat: >-\n    Every scope above is an Auth0 platform default identity scope. NONE is a VergeSense product\n    permission — there is no vergesense:read, no metrics:read, no webhooks:write. Whatever\n    authorization the MCP server applies to its tools is either audience-based or internal, and is\n    not discoverable anonymously.\ngaps:\n- No product scope vocabulary on either surface.\n- No read-only credential option for the REST API — every key is full-capability for its buildings.\n- No published scope reference page.\nchecked: '2026-09-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/scopes/vergesense-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Occupancy Intelligence
- Workplace Analytics
- Corporate Real Estate
- PropTech
- IoT Sensors
- Building Data
- Space Utilization
- Facilities Management
- Smart Buildings
- Webhooks
- MCP
- JSON:API
token_urls: []
---
