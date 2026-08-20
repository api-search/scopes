---
api_specs:
- filename: omnisend-analytics-api-openapi.yml
  format: yaml
  label: Omnisend Analytics API
  slug: omnisend-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-analytics-api-openapi.yml
- filename: omnisend-batches-api-openapi.yml
  format: yaml
  label: Omnisend Batches API
  slug: omnisend-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-batches-api-openapi.yml
- filename: omnisend-brands-api-openapi.yml
  format: yaml
  label: Omnisend Brands API
  slug: omnisend-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-brands-api-openapi.yml
- filename: omnisend-campaigns-api-openapi.yml
  format: yaml
  label: Omnisend Campaigns API
  slug: omnisend-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-campaigns-api-openapi.yml
- filename: omnisend-contacts-api-openapi.yml
  format: yaml
  label: Omnisend Contacts API
  slug: omnisend-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-contacts-api-openapi.yml
- filename: omnisend-emailcontent-api-openapi.yml
  format: yaml
  label: Omnisend EmailContent API
  slug: omnisend-emailcontent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-emailcontent-api-openapi.yml
- filename: omnisend-emailtemplates-api-openapi.yml
  format: yaml
  label: Omnisend EmailTemplates API
  slug: omnisend-emailtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-emailtemplates-api-openapi.yml
- filename: omnisend-emailuniversallayouts-api-openapi.yml
  format: yaml
  label: Omnisend EmailUniversalLayouts API
  slug: omnisend-emailuniversallayouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-emailuniversallayouts-api-openapi.yml
- filename: omnisend-events-api-openapi.yml
  format: yaml
  label: Omnisend Events API
  slug: omnisend-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-events-api-openapi.yml
- filename: omnisend-images-api-openapi.yml
  format: yaml
  label: Omnisend Images API
  slug: omnisend-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-images-api-openapi.yml
- filename: omnisend-productcategories-api-openapi.yml
  format: yaml
  label: Omnisend ProductCategories API
  slug: omnisend-productcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-productcategories-api-openapi.yml
- filename: omnisend-products-api-openapi.yml
  format: yaml
  label: Omnisend Products API
  slug: omnisend-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-products-api-openapi.yml
- filename: omnisend-segments-api-openapi.yml
  format: yaml
  label: Omnisend Segments API
  slug: omnisend-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-segments-api-openapi.yml
- filename: omnisend-automations-api-openapi.yml
  format: yaml
  label: Omnisend Automations API
  slug: omnisend-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-automations-api-openapi.yml
- filename: omnisend-event-metadata-api-openapi.yml
  format: yaml
  label: Omnisend Event Metadata API
  slug: omnisend-event-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-event-metadata-api-openapi.yml
authorization_urls: []
description: 'OAuth 2.0 scopes for Omnisend. The authoritative list is the provider''s own RFC 8414 authorization server metadata, which declares 26 scopes — six more than any OpenAPI contract exposes. The RFC 9728 protected-resource metadata on the MCP host declares a 22-scope subset: the four missing there (accounts.write, sessions.write, reports.read, brand-assets.write) are account-level scopes the MCP agent surface deliberately does not offer. Scope names are resource.action and map cleanly onto the API resources.'
docs: https://api-docs.omnisend.com/reference/oauth
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Omnisend Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Omnisend publishes 20 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Omnisend API on a user''s behalf.


  Tokens are issued from https://app.omnisend.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Omnisend
provider_slug: omnisend
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-analytics-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-automations-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-batches-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-brands-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-campaigns-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-contacts-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-emailcontent-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-emailtemplates-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-emailuniversallayouts-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-event-metadata-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-events-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-images-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-productcategories-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-products-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.omnisend.com/oauth2/token
  name: Bearer
  source: openapi/omnisend-segments-api-openapi.yml
scope_count: 20
scope_names:
- analytics.read
- automations.read
- automations.write
- brands.read
- brands.write
- campaigns.read
- campaigns.write
- contacts.read
- contacts.write
- email-templates.read
- email-templates.write
- events.read
- events.write
- images.read
- images.write
- none
- products.read
- products.write
- segments.read
- segments.write
scopes:
- description: ''
  flows: []
  scope: analytics.read
- description: Read access to automations
  flows:
  - clientCredentials
  scope: automations.read
- description: Write access to automations
  flows:
  - clientCredentials
  scope: automations.write
- description: ''
  flows: []
  scope: brands.read
- description: ''
  flows: []
  scope: brands.write
- description: Read access to campaigns
  flows:
  - clientCredentials
  scope: campaigns.read
- description: Write access to campaigns
  flows:
  - clientCredentials
  scope: campaigns.write
- description: Read contacts
  flows:
  - clientCredentials
  scope: contacts.read
- description: Create, update and delete contacts
  flows:
  - clientCredentials
  scope: contacts.write
- description: Allows reading email templates and universal layouts
  flows:
  - clientCredentials
  scope: email-templates.read
- description: Allows create, update, delete email templates and universal layouts
  flows:
  - clientCredentials
  scope: email-templates.write
- description: ''
  flows: []
  scope: events.read
- description: ''
  flows: []
  scope: events.write
- description: Allows reading images
  flows:
  - clientCredentials
  scope: images.read
- description: Allows uploading and deleting images
  flows:
  - clientCredentials
  scope: images.write
- description: No scopes required — authorization is not enforced via OAuth2 scopes
  flows:
  - clientCredentials
  scope: none
- description: Grants read access to product data
  flows:
  - clientCredentials
  scope: products.read
- description: Grants write access to product data
  flows:
  - clientCredentials
  scope: products.write
- description: Read segments
  flows:
  - clientCredentials
  scope: segments.read
- description: Create, update and delete segments
  flows:
  - clientCredentials
  scope: segments.write
slug: omnisend-scopes
source_filename: omnisend-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://mcp.omnisend.com/.well-known/oauth-authorization-server (RFC 8414 scopes_supported), https://mcp.omnisend.com/.well-known/oauth-protected-resource\n  (RFC 9728 scopes_supported), https://api-docs.omnisend.com/reference/oauth, per-operation \"Scopes:\" notes in https://api-docs.omnisend.com/llms.txt,\n  and openapi/omnisend-*-openapi.yml\nschemes:\n- name: Bearer\n  source: openapi/omnisend-analytics-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-automations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-batches-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-brands-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-campaigns-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-contacts-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-emailcontent-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-emailtemplates-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-emailuniversallayouts-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-event-metadata-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n  \
  \  tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-events-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-images-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-productcategories-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-products-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\n- name: Bearer\n  source: openapi/omnisend-segments-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.omnisend.com/oauth2/token\nscopes:\n- scope: analytics.read\n  sources:\n  - openapi/omnisend-analytics-api-openapi.yml\n- scope: automations.read\n  description: Read\
  \ access to automations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-automations-api-openapi.yml\n- scope: automations.write\n  description: Write access to automations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-automations-api-openapi.yml\n- scope: brands.read\n  sources:\n  - openapi/omnisend-brands-api-openapi.yml\n- scope: brands.write\n  sources:\n  - openapi/omnisend-brands-api-openapi.yml\n- scope: campaigns.read\n  description: Read access to campaigns\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-campaigns-api-openapi.yml\n- scope: campaigns.write\n  description: Write access to campaigns\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-campaigns-api-openapi.yml\n- scope: contacts.read\n  description: Read contacts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-batches-api-openapi.yml\n  - openapi/omnisend-contacts-api-openapi.yml\n- scope: contacts.write\n  description: Create,\
  \ update and delete contacts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-batches-api-openapi.yml\n  - openapi/omnisend-contacts-api-openapi.yml\n- scope: email-templates.read\n  description: Allows reading email templates and universal layouts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-emailcontent-api-openapi.yml\n  - openapi/omnisend-emailtemplates-api-openapi.yml\n  - openapi/omnisend-emailuniversallayouts-api-openapi.yml\n- scope: email-templates.write\n  description: Allows create, update, delete email templates and universal layouts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-emailcontent-api-openapi.yml\n  - openapi/omnisend-emailtemplates-api-openapi.yml\n  - openapi/omnisend-emailuniversallayouts-api-openapi.yml\n- scope: events.read\n  sources:\n  - openapi/omnisend-batches-api-openapi.yml\n- scope: events.write\n  sources:\n  - openapi/omnisend-batches-api-openapi.yml\n  - openapi/omnisend-events-api-openapi.yml\n\
  - scope: images.read\n  description: Allows reading images\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-images-api-openapi.yml\n- scope: images.write\n  description: Allows uploading and deleting images\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-images-api-openapi.yml\n- scope: none\n  description: No scopes required — authorization is not enforced via OAuth2 scopes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-event-metadata-api-openapi.yml\n- scope: products.read\n  description: Grants read access to product data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-batches-api-openapi.yml\n  - openapi/omnisend-productcategories-api-openapi.yml\n  - openapi/omnisend-products-api-openapi.yml\n- scope: products.write\n  description: Grants write access to product data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-batches-api-openapi.yml\n  - openapi/omnisend-productcategories-api-openapi.yml\n\
  \  - openapi/omnisend-products-api-openapi.yml\n- scope: segments.read\n  description: Read segments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-segments-api-openapi.yml\n- scope: segments.write\n  description: Create, update and delete segments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/omnisend-segments-api-openapi.yml\ndocs: https://api-docs.omnisend.com/reference/oauth\ndescription: 'OAuth 2.0 scopes for Omnisend. The authoritative list is the provider''s own RFC 8414 authorization\n  server metadata, which declares 26 scopes — six more than any OpenAPI contract exposes. The RFC 9728 protected-resource\n  metadata on the MCP host declares a 22-scope subset: the four missing there (accounts.write, sessions.write, reports.read,\n  brand-assets.write) are account-level scopes the MCP agent surface deliberately does not offer. Scope names are\n  resource.action and map cleanly onto the API resources.'\nauthorization_server:\n  issuer: https://app.omnisend.com\n\
  \  metadata: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n  authorization_endpoint: https://app.omnisend.com/oauth2/authorize\n  token_endpoint: https://app.omnisend.com/oauth2/token\n  registration_endpoint: https://app.omnisend.com/oauth2/register\n  revocation_endpoint: https://app.omnisend.com/oauth2/revoke\n  grant_types:\n  - authorization_code\n  - refresh_token\n  code_challenge_methods:\n  - S256\n  scope_delimiter: space\n  note: Requested with the `scope` query parameter on the authorize call. Omnisend's OAuth page writes the parameter\n    as `scopes` in its table and `scope` in its example — the RFC 6749 name is `scope`.\npublished_scopes:\n- scope: contacts.write\n  description: Create, update and delete contacts\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: contacts.read\n  description: Read contacts\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n\
  - scope: products.write\n  description: Create, update and delete product data and categories\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: products.read\n  description: Read product data\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: events.write\n  description: Send customer events and declare custom event metadata\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: events.read\n  description: Read customer events\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: accounts.write\n  description: Account-level write. Not offered on the MCP surface.\n  in_openapi: false\n  on_mcp: false\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: sessions.write\n  description: Session\
  \ write. Not offered on the MCP surface.\n  in_openapi: false\n  on_mcp: false\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: brands.write\n  description: Connect a store / write brand information (OAuth only)\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: brands.read\n  description: Read brand information\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: automations.read\n  description: Read automation workflows\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: automations.write\n  description: Create, update, enable, disable and delete automation workflows\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: campaigns.read\n  description: Read campaigns\n  in_openapi:\
  \ true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: campaigns.write\n  description: Create, update, send, cancel, copy and delete campaigns\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: reports.read\n  description: Read reports. Not offered on the MCP surface.\n  in_openapi: false\n  on_mcp: false\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: analytics.read\n  description: Generate analytics reports and statistics\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: segments.read\n  description: Read segments and segment statistics\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: segments.write\n  description: Create, update and delete segments\n  in_openapi: true\n  on_mcp: true\n\
  \  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: email-templates.read\n  description: Read email templates, email content and universal layouts\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: email-templates.write\n  description: Create, update, delete and render email templates, content and universal layouts\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: images.read\n  description: Read images\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: images.write\n  description: Upload and delete images\n  in_openapi: true\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: forms.read\n  description: Read sign-up forms and form reports\n  in_openapi: false\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n\
  - scope: forms.write\n  description: Create and update sign-up forms\n  in_openapi: false\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: brand-assets.read\n  description: Read brand assets\n  in_openapi: false\n  on_mcp: true\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\n- scope: brand-assets.write\n  description: Write brand assets. Not offered on the MCP surface.\n  in_openapi: false\n  on_mcp: false\n  source: https://mcp.omnisend.com/.well-known/oauth-authorization-server\nscope_count: 26\nnotes:\n- The OpenAPI contracts declare only contacts.read and contacts.write inside the Bearer securityScheme; every other\n  scope requirement is stated in prose in the per-operation description (\"**Scopes:** `campaigns.write`\"), not in\n  the machine-readable security block.\n- The Event Metadata API operations declare no scope in the spec at all — the derived entry \"none\" below is an artifact\n  of that omission,\
  \ not a claim that the operations are unauthenticated. The docs state events.write for create/update.\n- forms.read / forms.write and brand-assets.* have no published OpenAPI at all; the Forms surface is reachable only\n  through the MCP server.\n- Client credentials are not self-serve — the OAuth page asks integrators to submit a Google Form and promises credentials\n  in 1-3 business days. The MCP hosts advertise RFC 7591 dynamic client registration, which is a different and faster\n  path.\n- Access tokens are documented as effectively non-expiring (expires_in 9223372036) unless revoked.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/scopes/omnisend-scopes.yml
summary_line: 20 scopes · clientCredentials
tags:
- Email Marketing
- Marketing Automation
- E-Commerce
- SMS Marketing
- Customer Engagement
- Segmentation
- Campaigns
- Forms
- Popups
- Web Push
- Automation Workflows
- Analytics
- MCP
- Agent Ready
- Transactional Messaging
token_urls:
- https://app.omnisend.com/oauth2/token
---
