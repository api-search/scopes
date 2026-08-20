---
api_specs:
- filename: blueshift-openapi.yml
  format: yaml
  label: Blueshift REST API
  slug: blueshift-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshift/refs/heads/main/openapi/blueshift-openapi.yml
authorization_urls: []
description: Blueshift declares eight OAuth 2.0 scopes, published in machine-readable form in both its RFC 8414 authorization-server metadata and its RFC 9728 protected-resource metadata, on all four API/app hosts (US and EU). They apply to the MCP server, not the REST API — the REST API has no OAuth at all. The scope set is a clean read/write pair over four domains, which is materially better granularity than the two all-or-nothing API keys the REST API offers. Descriptions below are derived from the scope names and the corresponding MCP tool categories; Blueshift publishes the scope strings but no scope reference page, so no description here is quoted from Blueshift.
docs: https://help.blueshift.com/hc/en-us/articles/49713147943187-The-Blueshift-MCP-Server-Beta
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Blueshift Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Blueshift uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blueshift
provider_slug: blueshift
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: blueshift-scopes
source_filename: blueshift-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://api.getblueshift.com/.well-known/oauth-authorization-server and\n  https://app.getblueshift.com/.well-known/oauth-protected-resource — fetched\n  anonymously 2026-08-12, both HTTP 200.\ndocs: https://help.blueshift.com/hc/en-us/articles/49713147943187-The-Blueshift-MCP-Server-Beta\ndescription: >-\n  Blueshift declares eight OAuth 2.0 scopes, published in machine-readable form\n  in both its RFC 8414 authorization-server metadata and its RFC 9728\n  protected-resource metadata, on all four API/app hosts (US and EU). They apply\n  to the MCP server, not the REST API — the REST API has no OAuth at all. The\n  scope set is a clean read/write pair over four domains, which is materially\n  better granularity than the two all-or-nothing API keys the REST API offers.\n  Descriptions below are derived from the scope names and the corresponding MCP\n  tool categories; Blueshift publishes the scope strings but no scope reference\n\
  \  page, so no description here is quoted from Blueshift.\n\napplies_to: Blueshift MCP Server\nnot_applicable_to: >-\n  Blueshift REST API — authenticates with HTTP Basic and an API key, and\n  declares no oauth2 securityScheme in its OpenAPI.\n\nauthorization_server: https://app.getblueshift.com\nauthorization_endpoint: https://app.getblueshift.com/oauth/authorize\ntoken_endpoint: https://app.getblueshift.com/oauth/token\nregistration_endpoint: https://app.getblueshift.com/oauth/register\ngrant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\nresponse_types:\n  - code\ncode_challenge_methods:\n  - S256\ntoken_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  - client_secret_post\n\nscope_count: 8\nscopes:\n  - name: campaigns:read\n    access: read\n    domain: Campaigns\n    description: >-\n      Read campaigns, their configuration, schedules and performance statistics.\n    description_source: derived\n  - name: campaigns:write\n    access: write\n\
  \    domain: Campaigns\n    description: >-\n      Create and modify campaigns, including schedule changes and lifecycle\n      transitions.\n    description_source: derived\n  - name: segments:read\n    access: read\n    domain: Segments\n    description: Read segment definitions and audience membership counts.\n    description_source: derived\n  - name: segments:write\n    access: write\n    domain: Segments\n    description: Create and modify segments.\n    description_source: derived\n  - name: templates:read\n    access: read\n    domain: Templates\n    description: >-\n      Read email, push and SMS templates and their shared assets.\n    description_source: derived\n  - name: templates:write\n    access: write\n    domain: Templates\n    description: Create and modify templates.\n    description_source: derived\n  - name: customers:read\n    access: read\n    domain: Customer profiles\n    description: >-\n      Read customer profiles, events, transactions and campaign activity.\
  \ This\n      is the scope that reaches personal data.\n    description_source: derived\n  - name: customers:write\n    access: write\n    domain: Customer profiles\n    description: Create and modify customer profiles and their attributes.\n    description_source: derived\n\nobservations:\n  - >-\n    The scope set does NOT cover every MCP tool category. Reporting and\n    dashboards, schema discovery, recommendations, the AI campaign optimizer,\n    pages and scripts, image management and marketing insights all appear in\n    Blueshift's published tool catalogue with no corresponding scope, so either\n    those tools fall under an existing scope by association or the scope model\n    has not caught up with the tool surface. Blueshift publishes nothing that\n    resolves this, and it is not inferred here.\n  - >-\n    Dynamic client registration is open (registration_endpoint present,\n    token_endpoint_auth_methods includes \"none\"), which is what lets an MCP\n    client connect with\
  \ only a URL.\n  - >-\n    The same eight scopes are served identically from api.getblueshift.com,\n    api.eu.getblueshift.com, app.getblueshift.com and app.eu.getblueshift.com.\n\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n    - url: https://api.getblueshift.com/.well-known/oauth-authorization-server\n      status: 200\n      file: well-known/blueshift-oauth-authorization-server.json\n    - url: https://api.getblueshift.com/.well-known/oauth-protected-resource\n      status: 200\n      file: well-known/blueshift-oauth-protected-resource.json\n    - url: https://app.getblueshift.com/.well-known/oauth-authorization-server\n      status: 200\n      file: well-known/blueshift-app-oauth-authorization-server.json\n    - url: https://app.getblueshift.com/.well-known/oauth-protected-resource\n      status: 200\n      file: well-known/blueshift-app-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueshift/refs/heads/main/scopes/blueshift-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Customer Data Platform
- Customer Engagement
- Marketing Automation
- Cross-Channel Messaging
- Email
- SMS
- Push Notifications
- Segmentation
- Personalization
- Product Recommendations
- Event Tracking
- Product Catalog
- MarTech
- MCP
- agent-native
token_urls: []
---
