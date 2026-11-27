---
api_specs:
- filename: comos-portal-com-openapi.yml
  format: yaml
  label: ComOS Federation Gateway
  slug: comos-federation-gateway
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comos-portal-com/openapi/comos-portal-com-openapi.yml
authorization_urls: []
description: ''
docs: https://comos-portal.com/.well-known/mcp/server-card.json
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: ComOS Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares no securitySchemes; scopes are published in the RFC 8414 authorization-server metadata (scopes_supported) and described in the MCP server card. Scopes marked (irreversible) are so labelled by the provider.
overview: 'ComOS publishes 72 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the ComOS API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ComOS
provider_slug: comos-portal-com
schemes: []
scope_count: 72
scope_names:
- orders:read
- orders:write
- catalog:write
- catalog:read
- orders:refund
- agents:read
- agents:admin
- agents:tenant-operator:read
- agents:tenant-operator:run
- introspection:read
- introspection:generate
- tenants:write
- managers:write
- managers:admin
- federation:apply
- nodes:write
- coms:redeem
- wallet:bind
- processor:connect
- storefront:write
- booking_page:write
- tenant_style:write
- workflows:write
- workflows:read
- workflows:run
- marketing:read
- marketing:write
- marketing:send
- rentals:read
- rentals:assets:write
- rentals:rent
- services:read
- services:quote
- services:job
- digital:read
- digital:licenses:write
- digital:grant
- storage:read
- storage:write
- rendering:read
- rendering:write
- rendering:prove
- bookings:write
- bookings:read
- shipping:write
- email:send
- email:templates:write
- reviews:write
- reviews:moderate
- prompts:submit
- support:write
- loyalty:write
- offer:publish
- offer:subscribe
- customer:write
- customer:read
- recommendations:write
- consent:write
- integration:write
- tax:nexus:write
- tax:nexus:read
- governance:read
- governance:write
- policies:write
- knowledge:write
- voice:write
- journal:write
- journal:read
- notifications:read
- notifications:write
- cohort:email:send
- llm:author
scopes:
- description: Read your orders and their status
  flows: []
  scope: orders:read
- description: Place and update orders on your behalf
  flows: []
  scope: orders:write
- description: Create and edit catalog content (products, collections, prices)
  flows: []
  scope: catalog:write
- description: Read your own full catalog and collections, including drafts
  flows: []
  scope: catalog:read
- description: Refund and cancel paid orders — money goes back to the buyer (irreversible)
  flows: []
  scope: orders:refund
- description: List agents and read their run history
  flows: []
  scope: agents:read
- description: Run and administer autonomous agents
  flows: []
  scope: agents:admin
- description: Read tenant-operator agent runs
  flows: []
  scope: agents:tenant-operator:read
- description: Trigger tenant-operator agent runs
  flows: []
  scope: agents:tenant-operator:run
- description: Read system introspection (confidence, coverage, corpus)
  flows: []
  scope: introspection:read
- description: Generate introspection content for review
  flows: []
  scope: introspection:generate
- description: Create, update, and suspend tenants
  flows: []
  scope: tenants:write
- description: Create manager accountability roots
  flows: []
  scope: managers:write
- description: Read the manager tree and perform manager operations
  flows: []
  scope: managers:admin
- description: Apply to the federation as a manager root (self-admission)
  flows: []
  scope: federation:apply
- description: Register your own computers as nodes on the network, and remove them
  flows: []
  scope: nodes:write
- description: Redeem Coms — move treasury value out (irreversible)
  flows: []
  scope: coms:redeem
- description: Bind the wallet your redemptions are paid to (you sign to prove you control it)
  flows: []
  scope: wallet:bind
- description: Connect your own card-processor account so your card sales settle there (you complete the processor’s onboarding)
  flows: []
  scope: processor:connect
- description: Author and publish your storefront page from your experience prompt
  flows: []
  scope: storefront:write
- description: Author, publish and configure your booking page from your experience prompt
  flows: []
  scope: booking_page:write
- description: Store and remove your tenant's own stylesheet and its images
  flows: []
  scope: tenant_style:write
- description: Author and deploy automation workflows
  flows: []
  scope: workflows:write
- description: Read workflow definitions and run history
  flows: []
  scope: workflows:read
- description: Trigger workflow runs (priced acts)
  flows: []
  scope: workflows:run
- description: Read campaigns, segments, and send history
  flows: []
  scope: marketing:read
- description: Create and edit campaigns and segments
  flows: []
  scope: marketing:write
- description: Send a marketing campaign to a segment (irreversible)
  flows: []
  scope: marketing:send
- description: Read rental availability, asset condition, and your rentals with each renter's contact
  flows: []
  scope: rentals:read
- description: List and update returnable rental assets
  flows: []
  scope: rentals:assets:write
- description: Check out, return, and cancel rentals
  flows: []
  scope: rentals:rent
- description: Read service capabilities and job status
  flows: []
  scope: services:read
- description: Request, submit, and negotiate service quotes
  flows: []
  scope: services:quote
- description: Manage service jobs and milestones
  flows: []
  scope: services:job
- description: Read digital licenses and entitlements
  flows: []
  scope: digital:read
- description: List and update digital goods
  flows: []
  scope: digital:licenses:write
- description: Issue and revoke digital entitlements
  flows: []
  scope: digital:grant
- description: Read stored files and their metadata
  flows: []
  scope: storage:read
- description: Upload, replace, and delete stored files
  flows: []
  scope: storage:write
- description: Preview your own pages under any theme and renderer
  flows: []
  scope: rendering:read
- description: Register themes and renderers, and choose and publish how your pages look
  flows: []
  scope: rendering:write
- description: Record a theme proof run (ComOS's own prover; never granted to a person)
  flows: []
  scope: rendering:prove
- description: Create and manage bookings
  flows: []
  scope: bookings:write
- description: Read bookings, providers, and availability
  flows: []
  scope: bookings:read
- description: Buy labels and manage shipping configuration
  flows: []
  scope: shipping:write
- description: Send email on your behalf
  flows: []
  scope: email:send
- description: Create and edit email templates
  flows: []
  scope: email:templates:write
- description: Submit and edit product reviews
  flows: []
  scope: reviews:write
- description: Approve, reject, and flag reviews
  flows: []
  scope: reviews:moderate
- description: Submit prompts you wrote to the ComOS prompt library for review
  flows: []
  scope: prompts:submit
- description: Open and update support tickets
  flows: []
  scope: support:write
- description: Enroll members and adjust loyalty balances
  flows: []
  scope: loyalty:write
- description: Publish and withdraw offers
  flows: []
  scope: offer:publish
- description: Subscribe to and unsubscribe from offers
  flows: []
  scope: offer:subscribe
- description: Create and update customer records
  flows: []
  scope: customer:write
- description: Read your own customers and their consent
  flows: []
  scope: customer:read
- description: Set and clear recommendation rules
  flows: []
  scope: recommendations:write
- description: Record and revoke customer consent
  flows: []
  scope: consent:write
- description: Configure third-party integrations and credentials
  flows: []
  scope: integration:write
- description: Register and update tax nexus locations
  flows: []
  scope: tax:nexus:write
- description: Read tax nexus locations and applied rates
  flows: []
  scope: tax:nexus:read
- description: Read governance records, chains, and policies
  flows: []
  scope: governance:read
- description: Record governance decisions and attestations
  flows: []
  scope: governance:write
- description: Create and edit tenant policies
  flows: []
  scope: policies:write
- description: Add and edit knowledge-base content
  flows: []
  scope: knowledge:write
- description: Configure voice agents and prompts
  flows: []
  scope: voice:write
- description: Append entries to the tenant journal
  flows: []
  scope: journal:write
- description: Read the tenant journal
  flows: []
  scope: journal:read
- description: Read notifications and delivery status
  flows: []
  scope: notifications:read
- description: Send and manage notifications
  flows: []
  scope: notifications:write
- description: Send email on the cohort rail (irreversible)
  flows: []
  scope: cohort:email:send
- description: Run LLM authoring billed to your HQ
  flows: []
  scope: llm:author
slug: comos-portal-com-scopes
source_filename: comos-portal-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://comos-portal.com/.well-known/oauth-authorization-server\n- https://comos-portal.com/.well-known/mcp/server-card.json\ndocs: https://comos-portal.com/.well-known/mcp/server-card.json\nnote: The OpenAPI declares no securitySchemes; scopes are published in the RFC 8414 authorization-server metadata (scopes_supported) and described in the MCP server card. Scopes marked (irreversible) are so labelled by the provider.\nscopes:\n- name: orders:read\n  description: Read your orders and their status\n- name: orders:write\n  description: Place and update orders on your behalf\n- name: catalog:write\n  description: Create and edit catalog content (products, collections, prices)\n- name: catalog:read\n  description: Read your own full catalog and collections, including drafts\n- name: orders:refund\n  description: Refund and cancel paid orders — money goes back to the buyer (irreversible)\n- name: agents:read\n  description:\
  \ List agents and read their run history\n- name: agents:admin\n  description: Run and administer autonomous agents\n- name: agents:tenant-operator:read\n  description: Read tenant-operator agent runs\n- name: agents:tenant-operator:run\n  description: Trigger tenant-operator agent runs\n- name: introspection:read\n  description: Read system introspection (confidence, coverage, corpus)\n- name: introspection:generate\n  description: Generate introspection content for review\n- name: tenants:write\n  description: Create, update, and suspend tenants\n- name: managers:write\n  description: Create manager accountability roots\n- name: managers:admin\n  description: Read the manager tree and perform manager operations\n- name: federation:apply\n  description: Apply to the federation as a manager root (self-admission)\n- name: nodes:write\n  description: Register your own computers as nodes on the network, and remove them\n- name: coms:redeem\n  description: Redeem Coms — move treasury value\
  \ out (irreversible)\n- name: wallet:bind\n  description: Bind the wallet your redemptions are paid to (you sign to prove you control it)\n- name: processor:connect\n  description: Connect your own card-processor account so your card sales settle there (you complete the processor’s onboarding)\n- name: storefront:write\n  description: Author and publish your storefront page from your experience prompt\n- name: booking_page:write\n  description: Author, publish and configure your booking page from your experience prompt\n- name: tenant_style:write\n  description: Store and remove your tenant's own stylesheet and its images\n- name: workflows:write\n  description: Author and deploy automation workflows\n- name: workflows:read\n  description: Read workflow definitions and run history\n- name: workflows:run\n  description: Trigger workflow runs (priced acts)\n- name: marketing:read\n  description: Read campaigns, segments, and send history\n- name: marketing:write\n  description: Create and\
  \ edit campaigns and segments\n- name: marketing:send\n  description: Send a marketing campaign to a segment (irreversible)\n- name: rentals:read\n  description: Read rental availability, asset condition, and your rentals with each renter's contact\n- name: rentals:assets:write\n  description: List and update returnable rental assets\n- name: rentals:rent\n  description: Check out, return, and cancel rentals\n- name: services:read\n  description: Read service capabilities and job status\n- name: services:quote\n  description: Request, submit, and negotiate service quotes\n- name: services:job\n  description: Manage service jobs and milestones\n- name: digital:read\n  description: Read digital licenses and entitlements\n- name: digital:licenses:write\n  description: List and update digital goods\n- name: digital:grant\n  description: Issue and revoke digital entitlements\n- name: storage:read\n  description: Read stored files and their metadata\n- name: storage:write\n  description: Upload,\
  \ replace, and delete stored files\n- name: rendering:read\n  description: Preview your own pages under any theme and renderer\n- name: rendering:write\n  description: Register themes and renderers, and choose and publish how your pages look\n- name: rendering:prove\n  description: Record a theme proof run (ComOS's own prover; never granted to a person)\n- name: bookings:write\n  description: Create and manage bookings\n- name: bookings:read\n  description: Read bookings, providers, and availability\n- name: shipping:write\n  description: Buy labels and manage shipping configuration\n- name: email:send\n  description: Send email on your behalf\n- name: email:templates:write\n  description: Create and edit email templates\n- name: reviews:write\n  description: Submit and edit product reviews\n- name: reviews:moderate\n  description: Approve, reject, and flag reviews\n- name: prompts:submit\n  description: Submit prompts you wrote to the ComOS prompt library for review\n- name: support:write\n\
  \  description: Open and update support tickets\n- name: loyalty:write\n  description: Enroll members and adjust loyalty balances\n- name: offer:publish\n  description: Publish and withdraw offers\n- name: offer:subscribe\n  description: Subscribe to and unsubscribe from offers\n- name: customer:write\n  description: Create and update customer records\n- name: customer:read\n  description: Read your own customers and their consent\n- name: recommendations:write\n  description: Set and clear recommendation rules\n- name: consent:write\n  description: Record and revoke customer consent\n- name: integration:write\n  description: Configure third-party integrations and credentials\n- name: tax:nexus:write\n  description: Register and update tax nexus locations\n- name: tax:nexus:read\n  description: Read tax nexus locations and applied rates\n- name: governance:read\n  description: Read governance records, chains, and policies\n- name: governance:write\n  description: Record governance decisions\
  \ and attestations\n- name: policies:write\n  description: Create and edit tenant policies\n- name: knowledge:write\n  description: Add and edit knowledge-base content\n- name: voice:write\n  description: Configure voice agents and prompts\n- name: journal:write\n  description: Append entries to the tenant journal\n- name: journal:read\n  description: Read the tenant journal\n- name: notifications:read\n  description: Read notifications and delivery status\n- name: notifications:write\n  description: Send and manage notifications\n- name: cohort:email:send\n  description: Send email on the cohort rail (irreversible)\n- name: llm:author\n  description: Run LLM authoring billed to your HQ\n"
source_yaml_url: https://artifacts.apis.io/comos-portal-com/scopes/comos-portal-com-scopes.yml
summary_line: 72 scopes
tags:
- Company
- Commerce
- AI Agents
- Operating System
- Federation
- Payments
- Ledger
- Self-Hosted
- E-Commerce
- MCP
token_bound: false
token_urls: []
---
