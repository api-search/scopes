---
authorization_urls:
- https://mcp.caisgroup.com/authorize
description: Twelve OAuth scopes advertised anonymously by the CAIS MCP server's RFC 9728 protected-resource metadata and repeated verbatim in its RFC 8414 authorization-server metadata. CAIS publishes no scopes reference page, so descriptions below are read directly from the scope strings' own domain:resource:action grammar and are marked as such — nothing has been invented beyond what the scope name states.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cais Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CAIS publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CAIS API on a user''s behalf.


  Tokens are issued from https://mcp.caisgroup.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CAIS
provider_slug: cais
schemes:
- bearer_methods_supported:
  - header
  flows:
  - authorizationUrl: https://mcp.caisgroup.com/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://mcp.caisgroup.com/register
    revocationUrl: https://mcp.caisgroup.com/revoke
    tokenUrl: https://mcp.caisgroup.com/token
  name: mcp-oauth
  resource: https://mcp.caisgroup.com/mcp
  source: well-known/cais-oauth-protected-resource.json
  type: oauth2
scope_count: 12
scope_names:
- openid
- caisiq:courses:list
- caisiq:reporting:read
- funds:holdings:read
- funds:orders:create
- funds:products:admin-read
- funds:products:advisor-read
- iam:firms:read
- iam:teams:read
- iam:users:read
- ips:contacts:write
- ips:profiles:read
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the authenticated advisor.
  flows: []
  scope: openid
- description: List CAIS IQ education courses.
  flows: []
  scope: caisiq:courses:list
- description: Read CAIS IQ reporting.
  flows: []
  scope: caisiq:reporting:read
- description: Read fund holdings.
  flows: []
  scope: funds:holdings:read
- description: Create fund orders. The only write-side transactional scope advertised.
  flows: []
  scope: funds:orders:create
- description: Read the fund product catalogue with administrator visibility.
  flows: []
  scope: funds:products:admin-read
- description: Read the fund product catalogue with advisor visibility.
  flows: []
  scope: funds:products:advisor-read
- description: Read firm records.
  flows: []
  scope: iam:firms:read
- description: Read team records.
  flows: []
  scope: iam:teams:read
- description: Read user records.
  flows: []
  scope: iam:users:read
- description: Write investor contacts.
  flows: []
  scope: ips:contacts:write
- description: Read investor profiles.
  flows: []
  scope: ips:profiles:read
slug: cais-scopes
source_filename: cais-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://mcp.caisgroup.com/.well-known/oauth-protected-resource\nalso: https://mcp.caisgroup.com/.well-known/oauth-authorization-server\ndescription: >-\n  Twelve OAuth scopes advertised anonymously by the CAIS MCP server's RFC 9728\n  protected-resource metadata and repeated verbatim in its RFC 8414 authorization-server\n  metadata. CAIS publishes no scopes reference page, so descriptions below are read\n  directly from the scope strings' own domain:resource:action grammar and are marked\n  as such — nothing has been invented beyond what the scope name states.\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  source: well-known/cais-oauth-protected-resource.json\n  resource: https://mcp.caisgroup.com/mcp\n  bearer_methods_supported: [header]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.caisgroup.com/authorize\n    tokenUrl: https://mcp.caisgroup.com/token\n    revocationUrl: https://mcp.caisgroup.com/revoke\n\
  \    registrationUrl: https://mcp.caisgroup.com/register\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\nscope_grammar: '<domain>:<resource>:<action>'\ndomains:\n- id: caisiq\n  label: CAIS IQ — advisor education and reporting\n- id: funds\n  label: Fund and product catalogue, holdings and orders\n- id: iam\n  label: Identity and access — firms, teams, users\n- id: ips\n  label: Investor profile service — profiles and contacts\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token for the authenticated advisor.\n  domain: null\n  action: identity\n  sources: [well-known/cais-oauth-protected-resource.json]\n- scope: caisiq:courses:list\n  description: List CAIS IQ education courses.\n  domain: caisiq\n  action: list\n  sources: [well-known/cais-oauth-protected-resource.json]\n- scope: caisiq:reporting:read\n  description: Read CAIS IQ reporting.\n  domain: caisiq\n  action: read\n  sources: [well-known/cais-oauth-protected-resource.json]\n\
  - scope: funds:holdings:read\n  description: Read fund holdings.\n  domain: funds\n  action: read\n  sources: [well-known/cais-oauth-protected-resource.json]\n- scope: funds:orders:create\n  description: Create fund orders. The only write-side transactional scope advertised.\n  domain: funds\n  action: create\n  write: true\n  sources: [well-known/cais-oauth-protected-resource.json]\n- scope: funds:products:admin-read\n  description: Read the fund product catalogue with administrator visibility.\n  domain: funds\n  action: admin-read\n  sources: [well-known/cais-oauth-protected-resource.json]\n- scope: funds:products:advisor-read\n  description: Read the fund product catalogue with advisor visibility.\n  domain: funds\n  action: advisor-read\n  sources: [well-known/cais-oauth-protected-resource.json]\n- scope: iam:firms:read\n  description: Read firm records.\n  domain: iam\n  action: read\n  sources: [well-known/cais-oauth-protected-resource.json]\n- scope: iam:teams:read\n  description:\
  \ Read team records.\n  domain: iam\n  action: read\n  sources: [well-known/cais-oauth-protected-resource.json]\n- scope: iam:users:read\n  description: Read user records.\n  domain: iam\n  action: read\n  sources: [well-known/cais-oauth-protected-resource.json]\n- scope: ips:contacts:write\n  description: Write investor contacts.\n  domain: ips\n  action: write\n  write: true\n  sources: [well-known/cais-oauth-protected-resource.json]\n- scope: ips:profiles:read\n  description: Read investor profiles.\n  domain: ips\n  action: read\n  sources: [well-known/cais-oauth-protected-resource.json]\nsummary:\n  total: 12\n  read_scopes: 9\n  write_scopes: 2\n  identity_scopes: 1\n  note: >-\n    The scope surface is read-dominant. Only funds:orders:create and ips:contacts:write\n    mutate state, which is a meaningful agent-safety property: an agent granted the\n    default read set cannot place an order.\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://mcp.caisgroup.com/.well-known/oauth-protected-resource\n\
  \  http_status: 200\n  content_type: application/json\ndocs: null\ndocs_note: CAIS publishes no public OAuth scopes reference page as of this probe.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cais/refs/heads/main/scopes/cais-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Company
- Alternative Investments
- Wealth Management
- Financial-Services
- Fintech
- Private Markets
- Asset Management
- Structured Products
- Investment Platform
- Artificial Intelligence
token_urls:
- https://mcp.caisgroup.com/token
---
