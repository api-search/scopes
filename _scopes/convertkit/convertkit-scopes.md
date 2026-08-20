---
api_specs:
- filename: convertkit-accounts-api-openapi.yml
  format: yaml
  label: Kit Accounts API
  slug: convertkit-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-accounts-api-openapi.yml
- filename: convertkit-broadcasts-api-openapi.yml
  format: yaml
  label: Kit Broadcasts API
  slug: convertkit-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-broadcasts-api-openapi.yml
- filename: convertkit-custom-fields-api-openapi.yml
  format: yaml
  label: Kit Custom Fields API
  slug: convertkit-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-custom-fields-api-openapi.yml
- filename: convertkit-email-templates-api-openapi.yml
  format: yaml
  label: Kit Email Templates API
  slug: convertkit-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-email-templates-api-openapi.yml
- filename: convertkit-forms-api-openapi.yml
  format: yaml
  label: Kit Forms API
  slug: convertkit-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-forms-api-openapi.yml
- filename: convertkit-posts-api-openapi.yml
  format: yaml
  label: Kit Posts API
  slug: convertkit-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-posts-api-openapi.yml
- filename: convertkit-purchases-api-openapi.yml
  format: yaml
  label: Kit Purchases API
  slug: convertkit-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-purchases-api-openapi.yml
- filename: convertkit-segments-api-openapi.yml
  format: yaml
  label: Kit Segments API
  slug: convertkit-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-segments-api-openapi.yml
- filename: convertkit-sequence-emails-api-openapi.yml
  format: yaml
  label: Kit Sequence Emails API
  slug: convertkit-sequence-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-sequence-emails-api-openapi.yml
- filename: convertkit-sequences-api-openapi.yml
  format: yaml
  label: Kit Sequences API
  slug: convertkit-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-sequences-api-openapi.yml
- filename: convertkit-snippets-api-openapi.yml
  format: yaml
  label: Kit Snippets API
  slug: convertkit-snippets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-snippets-api-openapi.yml
- filename: convertkit-subscribers-api-openapi.yml
  format: yaml
  label: Kit Subscribers API
  slug: convertkit-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-subscribers-api-openapi.yml
- filename: convertkit-tags-api-openapi.yml
  format: yaml
  label: Kit Tags API
  slug: convertkit-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-tags-api-openapi.yml
- filename: convertkit-webhooks-api-openapi.yml
  format: yaml
  label: Kit Webhooks API
  slug: convertkit-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-webhooks-api-openapi.yml
authorization_urls:
- https://app.kit.com/oauth/authorize
- https://api.kit.com/v4/oauth/authorize
description: ''
docs: https://developers.kit.com/api-reference/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Convertkit Scopes
name_suffix: OAuth Scopes
note: Kit publishes NO scopes/permissions reference page. This artifact reconciles the only two machine-readable sources that exist, and they DISAGREE — recorded rather than reconciled away.
overview: 'Kit publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kit API on a user''s behalf.


  Tokens are issued from https://api.kit.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kit
provider_slug: convertkit
schemes:
- code_challenge_methods_supported:
  - S256
  description: Live OAuth 2.0 authorization server metadata (RFC 8414).
  flows:
  - authorizationUrl: https://app.kit.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.kit.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  http_status: 200
  issuer: https://api.kit.com
  name: OAuth2
  probed: '2026-08-13'
  registration_endpoint: https://app.kit.com/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://api.kit.com/oauth/revoke
  source: https://api.kit.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - none
- description: As declared in components.securitySchemes across all 14 refined specs. Endpoint URLs conflict with the live well-known document above.
  flows:
  - authorizationUrl: https://api.kit.com/v4/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.kit.com/v4/oauth/token
  name: OAuth2
  source: openapi/_original/openapi.json
scope_count: 3
scope_names:
- public
- read
- write
scopes:
- description: 'The only scope Kit''s live authorization server advertises (scopes_supported: ["public"]). Kit does not document what it grants; in practice a Kit OAuth token reaches the whole v4 surface the account is entitled to, so this is a coarse, all-or-nothing grant rather than a least-privilege scope model.'
  flows:
  - authorizationCode
  scope: public
- description: Read access to Kit API v4, as declared in the OpenAPI oauth2 flow scopes map.
  flows:
  - authorizationCode
  scope: read
- description: Write access to Kit API v4, as declared in the OpenAPI oauth2 flow scopes map.
  flows:
  - authorizationCode
  scope: write
slug: convertkit-scopes
source_filename: convertkit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api.kit.com/.well-known/oauth-authorization-server\ndocs: https://developers.kit.com/api-reference/authentication\nderived_from: openapi/_original/openapi.json (14 refined per-tag specs declare the same two scopes)\nnote: >-\n  Kit publishes NO scopes/permissions reference page. This artifact reconciles\n  the only two machine-readable sources that exist, and they DISAGREE — recorded\n  rather than reconciled away.\ndiscrepancy:\n  summary: >-\n    The OpenAPI declares scopes `read` and `write` and points at\n    https://api.kit.com/v4/oauth/authorize + /v4/oauth/token. The live RFC 8414\n    authorization-server metadata declares a single scope `public` and points at\n    https://app.kit.com/oauth/authorize + https://api.kit.com/oauth/token — a\n    different host for authorize and no /v4 prefix on either endpoint.\n  authoritative: >-\n    The well-known document is the live runtime contract and should be preferred\n\
  \    by a client; the spec's oauth2 block appears stale. Neither has been edited\n    here.\nschemes:\n- name: OAuth2\n  source: https://api.kit.com/.well-known/oauth-authorization-server\n  probed: '2026-08-13'\n  http_status: 200\n  issuer: https://api.kit.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.kit.com/oauth/authorize\n    tokenUrl: https://api.kit.com/oauth/token\n  revocation_endpoint: https://api.kit.com/oauth/revoke\n  registration_endpoint: https://app.kit.com/oauth/register\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code, refresh_token]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_post, none]\n  description: Live OAuth 2.0 authorization server metadata (RFC 8414).\n- name: OAuth2\n  source: openapi/_original/openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.kit.com/v4/oauth/authorize\n    tokenUrl: https://api.kit.com/v4/oauth/token\n\
  \  description: >-\n    As declared in components.securitySchemes across all 14 refined specs.\n    Endpoint URLs conflict with the live well-known document above.\nscopes:\n- scope: public\n  description: >-\n    The only scope Kit's live authorization server advertises\n    (scopes_supported: [\"public\"]). Kit does not document what it grants; in\n    practice a Kit OAuth token reaches the whole v4 surface the account is\n    entitled to, so this is a coarse, all-or-nothing grant rather than a\n    least-privilege scope model.\n  flows: [authorizationCode]\n  sources: [https://api.kit.com/.well-known/oauth-authorization-server]\n  authoritative: true\n- scope: read\n  description: Read access to Kit API v4, as declared in the OpenAPI oauth2 flow scopes map.\n  flows: [authorizationCode]\n  sources: [openapi/_original/openapi.json]\n  authoritative: false\n  note: Not advertised by the live authorization server.\n- scope: write\n  description: Write access to Kit API v4, as declared\
  \ in the OpenAPI oauth2 flow scopes map.\n  flows: [authorizationCode]\n  sources: [openapi/_original/openapi.json]\n  authoritative: false\n  note: Not advertised by the live authorization server.\ngranularity:\n  model: coarse\n  per_resource_scopes: false\n  note: >-\n    There is no per-resource or per-verb scope (no subscribers:read,\n    broadcasts:write). An agent granted a Kit token can send broadcasts and\n    delete data with the same credential it uses to read a subscriber count.\n    Kit mitigates this at the MCP layer with per-tool annotation hints\n    (destructiveHint) and client-side confirmation, not with scopes.\nresource_indicators:\n  protected_resource: https://app.kit.com/mcp\n  metadata: https://api.kit.com/.well-known/oauth-protected-resource\n  spec: RFC 9728\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/scopes/convertkit-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Email Marketing
- Creator Economy
- Subscribers
- Automation
- Newsletters
- Sequences
- Forms
- Broadcasts
- Webhook
- MCP
- Agents
- Authentication
- Marketing Automation
- Landing Pages
- Segmentation
- Email Campaigns
- Software-as-a-Service
- Commerce
token_urls:
- https://api.kit.com/oauth/token
- https://api.kit.com/v4/oauth/token
---
