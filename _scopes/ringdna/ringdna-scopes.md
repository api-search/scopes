---
authorization_urls:
- https://app.ringdna.com/mcp/oauth/authorize
- https://login.salesforce.com/services/oauth2/authorize
description: 'Two OAuth surfaces carry scopes. The first is Revenue.io''s own: the MCP authorization server at app.ringdna.com declares exactly one scope, `mcp`, in its RFC 8414 metadata. The second is not Revenue.io''s to define - it is the set of Salesforce Connected App scopes Revenue.io requests from the customer''s Salesforce org, published in the Knowledge Center. Both are recorded because an agent or admin evaluating Revenue.io''s access footprint needs both. No scope was derived from an OpenAPI - this repo has none.'
docs: https://support.revenue.io/integrations/salesforce/common-salesforce-errors/oauth-access-scope/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Ringdna Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RingDNA publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the RingDNA API on a user''s behalf.


  Tokens are issued from https://app.ringdna.com/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RingDNA
provider_slug: ringdna
schemes:
- flows:
  - authorizationUrl: https://app.ringdna.com/mcp/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://app.ringdna.com/mcp/oauth/token
  name: mcp-oauth
  owner: Revenue.io
  source: https://app.ringdna.com/.well-known/oauth-authorization-server
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
  name: salesforce-connected-app
  owner: Salesforce
  source: https://support.revenue.io/integrations/salesforce/common-salesforce-errors/oauth-access-scope/
scope_count: 4
scope_names:
- mcp
- api
- web
- refresh_token
scopes:
- description: The single scope advertised by the RingDNA MCP authorization server. It is coarse - there is no read/write split and no per-tool or per-resource scope - so an agent granted `mcp` receives whatever the server exposes to that user. Declared in both the authorization-server metadata and the protected-resource metadata for https://app.ringdna.com/mcp.
  flows:
  - authorizationCode
  scope: mcp
- description: Salesforce scope Revenue.io requests. Allows access to the logged-in user's account using APIs such as REST API and Bulk API 2.0; also includes chatter_api for Connect REST API resources.
  flows:
  - authorizationCode
  scope: api
- description: Salesforce scope Revenue.io requests. Allows use of the access_token on the web; includes visualforce, permitting access to customer-created Visualforce pages.
  flows:
  - authorizationCode
  scope: web
- description: Salesforce scope Revenue.io requests. Returns a refresh token so Revenue.io can log call data back to Salesforce while the user is offline. Synonymous with requesting offline_access. This is the scope that gives Revenue.io persistent, unattended access to the customer's CRM.
  flows:
  - authorizationCode
  scope: refresh_token
slug: ringdna-scopes
source_filename: ringdna-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://app.ringdna.com/.well-known/oauth-authorization-server\ndocs: https://support.revenue.io/integrations/salesforce/common-salesforce-errors/oauth-access-scope/\nname: RingDNA / Revenue.io OAuth Scopes\ndescription: >-\n  Two OAuth surfaces carry scopes. The first is Revenue.io's own: the MCP\n  authorization server at app.ringdna.com declares exactly one scope, `mcp`, in\n  its RFC 8414 metadata. The second is not Revenue.io's to define - it is the set\n  of Salesforce Connected App scopes Revenue.io requests from the customer's\n  Salesforce org, published in the Knowledge Center. Both are recorded because an\n  agent or admin evaluating Revenue.io's access footprint needs both. No scope\n  was derived from an OpenAPI - this repo has none.\n\nschemes:\n  - name: mcp-oauth\n    source: https://app.ringdna.com/.well-known/oauth-authorization-server\n    owner: Revenue.io\n    flows:\n      - flow: authorizationCode\n   \
  \     authorizationUrl: https://app.ringdna.com/mcp/oauth/authorize\n        tokenUrl: https://app.ringdna.com/mcp/oauth/token\n        pkce: S256\n\n  - name: salesforce-connected-app\n    source: https://support.revenue.io/integrations/salesforce/common-salesforce-errors/oauth-access-scope/\n    owner: Salesforce\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n\nscopes:\n  - scope: mcp\n    description: >-\n      The single scope advertised by the RingDNA MCP authorization server. It is\n      coarse - there is no read/write split and no per-tool or per-resource\n      scope - so an agent granted `mcp` receives whatever the server exposes to\n      that user. Declared in both the authorization-server metadata and the\n      protected-resource metadata for https://app.ringdna.com/mcp.\n    flows:\n      - authorizationCode\n    scheme: mcp-oauth\n    granularity: coarse\n    sources:\n      - https://app.ringdna.com/.well-known/oauth-authorization-server\n\
  \      - https://app.ringdna.com/.well-known/oauth-protected-resource\n\n  - scope: api\n    description: >-\n      Salesforce scope Revenue.io requests. Allows access to the logged-in user's\n      account using APIs such as REST API and Bulk API 2.0; also includes\n      chatter_api for Connect REST API resources.\n    flows:\n      - authorizationCode\n    scheme: salesforce-connected-app\n    owner: Salesforce\n    sources:\n      - https://support.revenue.io/integrations/salesforce/common-salesforce-errors/oauth-access-scope/\n\n  - scope: web\n    description: >-\n      Salesforce scope Revenue.io requests. Allows use of the access_token on the\n      web; includes visualforce, permitting access to customer-created\n      Visualforce pages.\n    flows:\n      - authorizationCode\n    scheme: salesforce-connected-app\n    owner: Salesforce\n    sources:\n      - https://support.revenue.io/integrations/salesforce/common-salesforce-errors/oauth-access-scope/\n\n  - scope: refresh_token\n\
  \    description: >-\n      Salesforce scope Revenue.io requests. Returns a refresh token so Revenue.io\n      can log call data back to Salesforce while the user is offline. Synonymous\n      with requesting offline_access. This is the scope that gives Revenue.io\n      persistent, unattended access to the customer's CRM.\n    flows:\n      - authorizationCode\n    scheme: salesforce-connected-app\n    owner: Salesforce\n    sources:\n      - https://support.revenue.io/integrations/salesforce/common-salesforce-errors/oauth-access-scope/\n\nrevocation:\n  supported: true\n  note: >-\n    Users and admins can revoke the Revenue.io Connected App at any time from\n    Salesforce. No revocation endpoint is advertised for the MCP authorization\n    server (no revocation_endpoint in its RFC 8414 metadata).\n\nnotes:\n  - >-\n    The Guided Selling API Key / API Secret credential has NO scope model at all -\n    it is an all-or-nothing credential bound to a Salesforce Org ID. See\n    authentication/ringdna-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ringdna/refs/heads/main/scopes/ringdna-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Sales Engagement
- Conversation Intelligence
- Sales Dialing
- Call Recording
- Revenue Orchestration
- CRM Integration
- Salesforce
- AI Coaching
- Sales Automation
token_urls:
- https://app.ringdna.com/mcp/oauth/token
---
