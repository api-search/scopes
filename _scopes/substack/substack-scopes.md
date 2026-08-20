---
authorization_urls:
- https://substack.com/oauth/auth
description: ''
docs: https://substack.com/oauth/.well-known/openid-configuration
flows:
- authorizationCode
- deviceCode
- implicit
kind: oauth-scopes
layout: scope
method: probed
name: Substack Scopes
name_suffix: OAuth Scopes
note: 'Substack publishes no human-readable OAuth scope reference. Every scope below was read from the provider''s own machine-readable discovery documents: the RFC 8414 Authorization Server Metadata at the host root and the OpenID Connect Discovery document at /oauth/.well-known/openid-configuration. The two lists differ — the OIDC document additionally advertises apple_podcasts — so the union is recorded with the source of each. Descriptions marked derived are inferred from the scope name and the corresponding product surface; Substack does not document them.'
overview: 'Substack publishes 8 OAuth 2.0 scopes via the authorizationCode, deviceCode, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Substack API on a user''s behalf.


  Tokens are issued from https://substack.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Substack
provider_slug: substack
schemes:
- flows:
  - authorizationUrl: https://substack.com/oauth/auth
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://substack.com/oauth/token
  - deviceAuthorizationUrl: https://substack.com/oauth/device/auth
    flow: deviceCode
    source: https://substack.com/oauth/.well-known/openid-configuration
    tokenUrl: https://substack.com/oauth/token
  - authorizationUrl: https://substack.com/oauth/auth
    flow: implicit
    note: advertised in the OIDC document only; not in the RFC 8414 document
    source: https://substack.com/oauth/.well-known/openid-configuration
  issuer: https://substack.com
  name: SubstackOAuth
  source: https://substack.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 8
scope_names:
- openid
- profile
- email
- offline_access
- mcp:read
- notes.read
- notes.write
- apple_podcasts
scopes:
- description: OpenID Connect authentication; issue an ID token for the signed-in Substack account.
  flows: []
  scope: openid
- description: Read the standard OIDC profile claims for the account.
  flows: []
  scope: profile
- description: Read the account email claim.
  flows: []
  scope: email
- description: Issue a refresh token so access can be renewed without re-consent.
  flows: []
  scope: offline_access
- description: Read-only access through the official Substack MCP server at https://mcp.substack.com/api/v1/mcp. This is the only scope the MCP protected resource metadata declares as supported.
  flows: []
  scope: mcp:read
- description: Read access to Substack Notes.
  flows: []
  scope: notes.read
- description: Write access to Substack Notes.
  flows: []
  scope: notes.write
- description: Podcast-feed linkage for the Apple Podcasts integration.
  flows: []
  scope: apple_podcasts
slug: substack-scopes
source_filename: substack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://substack.com/.well-known/oauth-authorization-server\ndocs: https://substack.com/oauth/.well-known/openid-configuration\nnote: >-\n  Substack publishes no human-readable OAuth scope reference. Every scope below was\n  read from the provider's own machine-readable discovery documents: the RFC 8414\n  Authorization Server Metadata at the host root and the OpenID Connect Discovery\n  document at /oauth/.well-known/openid-configuration. The two lists differ — the OIDC\n  document additionally advertises apple_podcasts — so the union is recorded with the\n  source of each. Descriptions marked derived are inferred from the scope name and the\n  corresponding product surface; Substack does not document them.\nschemes:\n  - name: SubstackOAuth\n    type: oauth2\n    issuer: https://substack.com\n    source: https://substack.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://substack.com/oauth/auth\n        tokenUrl: https://substack.com/oauth/token\n        pkce: S256\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://substack.com/oauth/device/auth\n        tokenUrl: https://substack.com/oauth/token\n        source: https://substack.com/oauth/.well-known/openid-configuration\n      - flow: implicit\n        authorizationUrl: https://substack.com/oauth/auth\n        source: https://substack.com/oauth/.well-known/openid-configuration\n        note: advertised in the OIDC document only; not in the RFC 8414 document\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token for the signed-in Substack account.\n    description_method: derived\n    sources: [oauth-authorization-server, openid-configuration]\n  - scope: profile\n    description: Read the standard OIDC profile claims for the account.\n    description_method: derived\n    sources: [oauth-authorization-server, openid-configuration]\n  -\
  \ scope: email\n    description: Read the account email claim.\n    description_method: derived\n    sources: [oauth-authorization-server, openid-configuration]\n  - scope: offline_access\n    description: Issue a refresh token so access can be renewed without re-consent.\n    description_method: derived\n    sources: [oauth-authorization-server, openid-configuration]\n  - scope: mcp:read\n    description: >-\n      Read-only access through the official Substack MCP server at\n      https://mcp.substack.com/api/v1/mcp. This is the only scope the MCP protected\n      resource metadata declares as supported.\n    description_method: probed\n    sources: [oauth-authorization-server, openid-configuration, oauth-protected-resource]\n    protected_resource: https://mcp.substack.com/api/v1/mcp\n  - scope: notes.read\n    description: Read access to Substack Notes.\n    description_method: derived\n    sources: [oauth-authorization-server, openid-configuration]\n    note: >-\n      Advertised\
  \ by the authorization server but not reachable through any documented\n      Substack surface — the MCP server's own documentation states it cannot access\n      Notes activity, and there is no published Notes REST API. Recorded because the\n      provider advertises it, not because a consumer-facing contract exists.\n  - scope: notes.write\n    description: Write access to Substack Notes.\n    description_method: derived\n    sources: [oauth-authorization-server, openid-configuration]\n    note: >-\n      Same as notes.read — advertised in discovery, with no published contract behind\n      it. This is the only write scope Substack advertises anywhere.\n  - scope: apple_podcasts\n    description: Podcast-feed linkage for the Apple Podcasts integration.\n    description_method: derived\n    sources: [openid-configuration]\n    note: present only in the OIDC discovery document, not in the RFC 8414 document\nclaims_supported:\n  - sub\n  - name\n  - subscription\n  - publication_role\n\
  \  - email\n  - publication_id\n  - sid\n  - auth_time\n  - iss\nx-evidence:\n  - fetched: '2026-08-13'\n    url: https://substack.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - fetched: '2026-08-13'\n    url: https://substack.com/oauth/.well-known/openid-configuration\n    http_status: 200\n  - fetched: '2026-08-13'\n    url: https://mcp.substack.com/.well-known/oauth-protected-resource/api/v1/mcp\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/substack/refs/heads/main/scopes/substack-scopes.yml
summary_line: 8 scopes · authorizationCode/deviceCode/implicit
tags:
- Newsletters
- Publishing
- Creator Economy
- Subscription
- Email
- Podcasting
- Notes
- Media
- Independent Media
- Paid Content
- MCP
- Agents
- RSS
- Analytics
token_urls:
- https://substack.com/oauth/token
---
