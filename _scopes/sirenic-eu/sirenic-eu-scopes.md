---
api_specs:
- filename: sirenic-eu-openapi.yml
  format: yaml
  label: Sirenic API
  slug: sirenic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirenic-eu/refs/heads/main/openapi/sirenic-eu-openapi.yml
authorization_urls: []
description: ''
docs: https://api.sirenic.eu/confidentialite (section "Le connecteur MCP et l'autorisation OAuth")
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Sirenic Eu Scopes
name_suffix: OAuth Scopes
note: 'OAuth 2.0 exists for ONE surface: the MCP connector at https://api.sirenic.eu/mcp/connecteur used by Gemini CLI / Claude / ChatGPT style assistants. The REST API itself is not OAuth — it is x402 pay-per-call or an X-Api-Key. The OpenAPI declares no oauth2 securityScheme, so derive-oauth-scopes.py produced nothing; this file is read from the live discovery documents.'
overview: 'Sirenic uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sirenic
provider_slug: sirenic-eu
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: sirenic-eu-scopes
source_filename: sirenic-eu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://api.sirenic.eu/.well-known/oauth-authorization-server (RFC 8414) and /.well-known/oauth-protected-resource\n  (RFC 9728)\ndocs: https://api.sirenic.eu/confidentialite (section \"Le connecteur MCP et l'autorisation OAuth\")\nnote: 'OAuth 2.0 exists for ONE surface: the MCP connector at https://api.sirenic.eu/mcp/connecteur used by Gemini\n  CLI / Claude / ChatGPT style assistants. The REST API itself is not OAuth — it is x402 pay-per-call or an X-Api-Key.\n  The OpenAPI declares no oauth2 securityScheme, so derive-oauth-scopes.py produced nothing; this file is read from\n  the live discovery documents.'\nauthorization_server:\n  issuer: https://api.sirenic.eu\n  authorization_endpoint: https://api.sirenic.eu/compte/connecteur\n  token_endpoint: https://api.sirenic.eu/oauth/jeton\n  registration_endpoint: https://api.sirenic.eu/oauth/enregistrement\n  revocation_endpoint: https://api.sirenic.eu/oauth/revoquer\n  grant_types_supported:\n\
  \  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - private_key_jwt\n  - none\n  - client_secret_post\n  - client_secret_basic\n  client_id_metadata_document_supported: true\n  dynamic_client_registration: true\nprotected_resource:\n  resource: https://api.sirenic.eu\n  resource_name: Sirenic MCP\n  authorization_servers:\n  - https://api.sirenic.eu\n  bearer_methods_supported:\n  - header\ntoken_lifetimes:\n  access_token: 1 hour\n  refresh_token: expires after 90 days without use\n  source: https://api.sirenic.eu/confidentialite\nscopes:\n- name: mcp\n  description: Call the data routes on behalf of the account holder, against the account's free monthly quota then\n    its prepaid credit balance. Does NOT grant the e-mail address, invoices, or the right to top up or close the\n    account (privacy policy, MCP connector section). The only scope the authorization\
  \ server advertises.\n  source: scopes_supported in both discovery documents\nscope_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sirenic-eu/refs/heads/main/scopes/sirenic-eu-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company Data
- Business Registry
- KYB
- Sanctions Screening
- Financial Data
- Credit Risk
- VAT Validation
- IBAN Validation
- E-Invoicing
- Public Procurement
- Open Data
- France
- Europe
- x402
- Agentic Commerce
- MCP
- A2A
- Company
token_urls: []
---
