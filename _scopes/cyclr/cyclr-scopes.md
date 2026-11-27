---
api_specs:
- filename: cyclr-account-connector-custom-categories-api-openapi.yml
  format: yaml
  label: Cyclr Account Connector Custom Categories API
  slug: cyclr-account-connector-custom-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-connector-custom-categories-api-openapi.yml
- filename: cyclr-account-connector-properties-api-openapi.yml
  format: yaml
  label: Cyclr Account Connector Properties API
  slug: cyclr-account-connector-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-connector-properties-api-openapi.yml
- filename: cyclr-account-connectors-api-openapi.yml
  format: yaml
  label: Cyclr Account Connectors API
  slug: cyclr-account-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-connectors-api-openapi.yml
- filename: cyclr-account-custom-connectors-api-openapi.yml
  format: yaml
  label: Cyclr Account Custom Connectors API
  slug: cyclr-account-custom-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-account-custom-connectors-api-openapi.yml
- filename: cyclr-accounts-api-openapi.yml
  format: yaml
  label: Cyclr Accounts API
  slug: cyclr-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-accounts-api-openapi.yml
- filename: cyclr-authentication-api-openapi.yml
  format: yaml
  label: Cyclr Authentication API
  slug: cyclr-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-authentication-api-openapi.yml
- filename: cyclr-connectors-api-openapi.yml
  format: yaml
  label: Cyclr Connectors API
  slug: cyclr-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-connectors-api-openapi.yml
- filename: cyclr-custom-fields-api-openapi.yml
  format: yaml
  label: Cyclr Custom Fields API
  slug: cyclr-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-custom-fields-api-openapi.yml
- filename: cyclr-cycles-api-openapi.yml
  format: yaml
  label: Cyclr Cycles API
  slug: cyclr-cycles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-cycles-api-openapi.yml
- filename: cyclr-edges-api-openapi.yml
  format: yaml
  label: Cyclr Edges API
  slug: cyclr-edges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-edges-api-openapi.yml
- filename: cyclr-mcp-servers-api-openapi.yml
  format: yaml
  label: Cyclr MCP Servers API
  slug: cyclr-mcp-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-mcp-servers-api-openapi.yml
- filename: cyclr-methods-api-openapi.yml
  format: yaml
  label: Cyclr Methods API
  slug: cyclr-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-methods-api-openapi.yml
- filename: cyclr-steps-api-openapi.yml
  format: yaml
  label: Cyclr Steps API
  slug: cyclr-steps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-steps-api-openapi.yml
- filename: cyclr-templates-api-openapi.yml
  format: yaml
  label: Cyclr Templates API
  slug: cyclr-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-templates-api-openapi.yml
- filename: cyclr-transactions-api-openapi.yml
  format: yaml
  label: Cyclr Transactions API
  slug: cyclr-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-transactions-api-openapi.yml
- filename: cyclr-users-api-openapi.yml
  format: yaml
  label: Cyclr Users API
  slug: cyclr-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cyclr/openapi/cyclr-users-api-openapi.yml
authorization_urls: []
description: ''
docs: https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Cyclr Scopes
name_suffix: OAuth Scopes
note: The Cyclr OpenAPI document declares an OAuth 2.0 clientCredentials flow with no scopes[] list. The Cyclr docs describe two scope mechanisms. Account-level Client Credentials carry an "OAuth Client Scope" that must be chosen when the credentials are created (Webhook, MCP, or Data On Demand). Console-level Client Credentials additionally accept an optional scope=account:{API_ID} parameter on the token request to restrict the resulting Access Token to a single Cyclr Account. No finer-grained per-operation scopes are published.
overview: 'Cyclr publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cyclr API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cyclr
provider_slug: cyclr
schemes: []
scope_count: 4
scope_names:
- Webhook
- MCP
- Data On Demand
- account:{API_ID}
scopes:
- description: Access Tokens generated by these Client Credentials are only valid for use with Cyclr Webhooks within the Account they were created in.
  flows: []
  scope: Webhook
- description: Access Tokens generated by these Client Credentials are only valid for use with Cyclr MCP Servers within the Account. MCP-scoped credentials can additionally hold one or more Sign-in Tokens so individual users can be identified when calling an MCP Server.
  flows: []
  scope: MCP
- description: Access Tokens generated by these Client Credentials are only valid when calling Cyclr API endpoints that execute Methods on Connectors installed in the Account (the Data on Demand feature).
  flows: []
  scope: Data On Demand
- description: When obtaining a token from Console-level Client Credentials, the optional scope=account:{API_ID} parameter restricts the issued Access Token to the specified Cyclr Account.
  flows: []
  scope: account:{API_ID}
slug: cyclr-scopes
source_filename: cyclr-scopes.yml
source_heading: OAuth Scopes
source_url: https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials
source_yaml: "generated: '2026-11-25'\nmethod: searched\nsource: https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials\ndocs: https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials\nsources:\n- https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials\n- https://community.cyclr.com/user-documentation/api/authentication\n- openapi/cyclr-platform-openapi.json\nflow: clientCredentials\nnote: >-\n  The Cyclr OpenAPI document declares an OAuth 2.0 clientCredentials flow with\n  no scopes[] list. The Cyclr docs describe two scope mechanisms. Account-level\n  Client Credentials carry an \"OAuth Client Scope\" that must be chosen when the\n  credentials are created (Webhook, MCP, or Data On Demand). Console-level\n  Client Credentials additionally accept an optional scope=account:{API_ID}\n  parameter on the token request to restrict the resulting Access Token to a\n  single Cyclr\
  \ Account. No finer-grained per-operation scopes are published.\nscopes:\n- name: Webhook\n  applies_to: account-level\n  description: Access Tokens generated by these Client Credentials are only valid\n    for use with Cyclr Webhooks within the Account they were created in.\n  source: https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials\n- name: MCP\n  applies_to: account-level\n  description: Access Tokens generated by these Client Credentials are only valid\n    for use with Cyclr MCP Servers within the Account. MCP-scoped credentials\n    can additionally hold one or more Sign-in Tokens so individual users can be\n    identified when calling an MCP Server.\n  source: https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials\n- name: Data On Demand\n  applies_to: account-level\n  description: Access Tokens generated by these Client Credentials are only valid\n    when calling Cyclr API endpoints that execute\
  \ Methods on Connectors installed\n    in the Account (the Data on Demand feature).\n  source: https://community.cyclr.com/user-documentation/accounts/account-level-oauth-client-credentials\n- name: account:{API_ID}\n  applies_to: console-level\n  description: When obtaining a token from Console-level Client Credentials, the\n    optional scope=account:{API_ID} parameter restricts the issued Access Token\n    to the specified Cyclr Account.\n  source: https://community.cyclr.com/user-documentation/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/cyclr/scopes/cyclr-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Connectors
- Custom Connectors
- Data Synchronization
- Embedded iPaaS
- Embedded SaaS Integration
- Embedded UI
- Integration Platform
- Integration
- Marketplace
- Authentication
- REST API
- Software-as-a-Service
- Templates
- Webhook
- White Label
- Workflows
token_bound: false
token_urls: []
---
