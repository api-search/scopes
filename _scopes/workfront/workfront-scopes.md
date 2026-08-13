---
api_specs:
- filename: workfront-planning-v2-openapi.json
  format: json
  label: Adobe Workfront Planning API v2
  slug: workfront-planning-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workfront/refs/heads/main/openapi/workfront-planning-v2-openapi.json
- filename: workfront-planning-v1-openapi.json
  format: json
  label: Adobe Workfront Planning API v1
  slug: workfront-planning-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workfront/refs/heads/main/openapi/workfront-planning-v1-openapi.json
authorization_urls:
- https://mcp.workfront.adobe.com/oauth/authorize
description: ''
docs: https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/configure-integrations/create-oauth-application
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Workfront Scopes
name_suffix: OAuth Scopes
note: Neither published Workfront Planning OpenAPI declares an oauth2 securityScheme, so derive-oauth-scopes.py found nothing. The scope list below is read verbatim from the two live OAuth discovery documents the Workfront MCP host serves (RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata), which advertise an identical scopes_supported array. These are Adobe IMS scopes, not Workfront-object scopes — Workfront itself does not publish a per-resource scope reference; object-level authorization is enforced by Workfront access levels and sharing (accessRules), not by OAuth scope.
overview: 'Adobe Workfront publishes 18 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Adobe Workfront API on a user''s behalf.


  Tokens are issued from https://mcp.workfront.adobe.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adobe Workfront
provider_slug: workfront
schemes:
- flows:
  - authorizationUrl: https://mcp.workfront.adobe.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://mcp.workfront.adobe.com/oauth/token
  issuer: https://mcp.workfront.adobe.com/mcp/v1
  name: Workfront MCP OAuth 2.1
  source: well-known/workfront-oauth-authorization-server.json
scope_count: 18
scope_names:
- AdobeID
- openid
- profile
- email
- additional_info.projectedProductContext
- read_pc.workfront
- read_organizations
- org.read
- accounts.read
- session
- read_pc
- read_pc.acp
- read_pc.dma_tartan
- aem.folders
- aem.assets.author
- aem.assets.delivery
- ab.manage
- creative_cloud
scopes:
- description: Core Adobe IMS identity scope.
  flows:
  - authorizationCode
  scope: AdobeID
- description: OpenID Connect — issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the signed-in user's Adobe profile.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the signed-in user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Adobe IMS product-context claim; resolves which Adobe products and organizations the user is entitled to, including the Workfront instance.
  flows:
  - authorizationCode
  scope: additional_info.projectedProductContext
- description: Read the user's Workfront product context — the Workfront-specific entitlement scope.
  flows:
  - authorizationCode
  scope: read_pc.workfront
- description: Read the Adobe organizations (IMS orgs) the user belongs to.
  flows:
  - authorizationCode
  scope: read_organizations
- description: Read organization metadata.
  flows:
  - authorizationCode
  scope: org.read
- description: Read account information.
  flows:
  - authorizationCode
  scope: accounts.read
- description: Session management scope.
  flows:
  - authorizationCode
  scope: session
- description: Read product context (generic).
  flows:
  - authorizationCode
  scope: read_pc
- description: Read Adobe Cloud Platform product context.
  flows:
  - authorizationCode
  scope: read_pc.acp
- description: Read product context for the Adobe DMA (tartan) service group.
  flows:
  - authorizationCode
  scope: read_pc.dma_tartan
- description: Adobe Experience Manager folder access — used by the Workfront/AEM document tools.
  flows:
  - authorizationCode
  scope: aem.folders
- description: Adobe Experience Manager Assets authoring access.
  flows:
  - authorizationCode
  scope: aem.assets.author
- description: Adobe Experience Manager Assets delivery access.
  flows:
  - authorizationCode
  scope: aem.assets.delivery
- description: Adobe App Builder management scope.
  flows:
  - authorizationCode
  scope: ab.manage
- description: Creative Cloud access.
  flows:
  - authorizationCode
  scope: creative_cloud
slug: workfront-scopes
source_filename: workfront-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://mcp.workfront.adobe.com/.well-known/oauth-authorization-server\ndocs: https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/configure-integrations/create-oauth-application\nnote: Neither published Workfront Planning OpenAPI declares an oauth2 securityScheme, so\n  derive-oauth-scopes.py found nothing. The scope list below is read verbatim from the two live OAuth\n  discovery documents the Workfront MCP host serves (RFC 8414 authorization-server metadata and RFC\n  9728 protected-resource metadata), which advertise an identical scopes_supported array. These are\n  Adobe IMS scopes, not Workfront-object scopes — Workfront itself does not publish a per-resource\n  scope reference; object-level authorization is enforced by Workfront access levels and sharing\n  (accessRules), not by OAuth scope.\nschemes:\n- name: Workfront MCP OAuth 2.1\n  source: well-known/workfront-oauth-authorization-server.json\n\
  \  issuer: https://mcp.workfront.adobe.com/mcp/v1\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.workfront.adobe.com/oauth/authorize\n    tokenUrl: https://mcp.workfront.adobe.com/oauth/token\n    pkce: [S256]\nscopes:\n- scope: AdobeID\n  description: Core Adobe IMS identity scope.\n  flows: [authorizationCode]\n- scope: openid\n  description: OpenID Connect — issue an ID token.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to the signed-in user's Adobe profile.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the signed-in user's email address.\n  flows: [authorizationCode]\n- scope: additional_info.projectedProductContext\n  description: Adobe IMS product-context claim; resolves which Adobe products and organizations the\n    user is entitled to, including the Workfront instance.\n  flows: [authorizationCode]\n- scope: read_pc.workfront\n  description: Read the user's Workfront product context — the Workfront-specific\
  \ entitlement scope.\n  flows: [authorizationCode]\n- scope: read_organizations\n  description: Read the Adobe organizations (IMS orgs) the user belongs to.\n  flows: [authorizationCode]\n- scope: org.read\n  description: Read organization metadata.\n  flows: [authorizationCode]\n- scope: accounts.read\n  description: Read account information.\n  flows: [authorizationCode]\n- scope: session\n  description: Session management scope.\n  flows: [authorizationCode]\n- scope: read_pc\n  description: Read product context (generic).\n  flows: [authorizationCode]\n- scope: read_pc.acp\n  description: Read Adobe Cloud Platform product context.\n  flows: [authorizationCode]\n- scope: read_pc.dma_tartan\n  description: Read product context for the Adobe DMA (tartan) service group.\n  flows: [authorizationCode]\n- scope: aem.folders\n  description: Adobe Experience Manager folder access — used by the Workfront/AEM document tools.\n  flows: [authorizationCode]\n- scope: aem.assets.author\n  description:\
  \ Adobe Experience Manager Assets authoring access.\n  flows: [authorizationCode]\n- scope: aem.assets.delivery\n  description: Adobe Experience Manager Assets delivery access.\n  flows: [authorizationCode]\n- scope: ab.manage\n  description: Adobe App Builder management scope.\n  flows: [authorizationCode]\n- scope: creative_cloud\n  description: Creative Cloud access.\n  flows: [authorizationCode]\nx-evidence:\n  fetched: '2026-08-12'\n  urls:\n  - url: https://mcp.workfront.adobe.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://mcp.workfront.adobe.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://mcp.workfront.adobe.com/mcp/v1/workfront/.well-known/oauth-protected-resource\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workfront/refs/heads/main/scopes/workfront-scopes.yml
summary_line: 18 scopes · authorizationCode
tags:
- Company
- Work Management
- Project Management
- Marketing Operations
- Creative Operations
- Collaboration
- Approvals
- Resource Management
- Workflow Automation
- Enterprise Software
- Adobe
- Model Context Protocol
token_urls:
- https://mcp.workfront.adobe.com/oauth/token
---
