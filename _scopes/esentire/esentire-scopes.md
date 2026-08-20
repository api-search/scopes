---
authorization_urls: []
description: 'The complete scope set eSentire advertises across both of its public OAuth discovery documents. It is three OIDC identity scopes and nothing else — there is no resource, product, or action scope published anywhere. That is a real finding, not a gap in the probe: RFC 9728 protected-resource metadata is the document a client is directed to by the 401 challenge in order to learn what to ask for, and eSentire''s names only openid, profile and email.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Esentire Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'eSentire uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: eSentire
provider_slug: esentire
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: esentire-scopes
source_filename: esentire-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://api.esentire.com/.well-known/oauth-protected-resource\ndocs: null\nname: eSentire OAuth scopes\ndescription: >-\n  The complete scope set eSentire advertises across both of its public OAuth\n  discovery documents. It is three OIDC identity scopes and nothing else — there\n  is no resource, product, or action scope published anywhere. That is a real\n  finding, not a gap in the probe: RFC 9728 protected-resource metadata is the\n  document a client is directed to by the 401 challenge in order to learn what to\n  ask for, and eSentire's names only openid, profile and email.\nauthorization_server: https://esentire.okta.com\nresource: https://api.esentire.com\nscope_count: 3\nscopes:\n- name: openid\n  type: oidc\n  description: Request an ID token and the subject (sub) claim. Required to initiate the OpenID Connect flow.\n  source: https://api.esentire.com/.well-known/oauth-authorization-server\n- name: profile\n  type:\
  \ oidc\n  description: End-user profile claims from the Okta identity.\n  source: https://api.esentire.com/.well-known/oauth-authorization-server\n- name: email\n  type: oidc\n  description: End-user email claim from the Okta identity.\n  source: https://api.esentire.com/.well-known/oauth-authorization-server\nresource_scopes: []\nanalysis:\n  granular_authorization: false\n  note: >-\n    No least-privilege surface is exposed to a client. An agent connecting to the\n    eSentire MCP server cannot request read-only access, cannot scope itself to one\n    product (MDR vs DFIR vs CTEM), and cannot narrow to one class of action —\n    because no such scopes are advertised. Whatever authorization actually governs\n    the MCP tools is enforced behind the token, invisibly to the client. For an\n    agent surface in a security product, where tools can plausibly take containment\n    actions on customer infrastructure, publishing an action-scoped authorization\n    model is the single highest-value\
  \ change available here.\ngaps:\n- No scope or permission reference page is published on esentire.com.\n- No resource-level or action-level scopes are advertised in either discovery document.\n- Scope-to-tool mapping cannot be established because the MCP tool list is auth-gated.\nx-evidence:\n  fetched: '2026-08-12'\n  urls:\n  - url: https://api.esentire.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://api.esentire.com/.well-known/oauth-authorization-server\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esentire/refs/heads/main/scopes/esentire-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Threat Intelligence
- Incident Response
- MCP
- Agents
- Authentication
- Software-as-a-Service
token_urls: []
---
