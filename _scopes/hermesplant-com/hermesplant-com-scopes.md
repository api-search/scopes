---
api_specs:
- filename: hermesplant-com-action-safety-api-openapi.yml
  format: yaml
  label: Hermes Plant Action Safety API
  slug: hermesplant-com-action-safety-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-action-safety-api-openapi.yml
- filename: hermesplant-com-agent-commerce-assurance-api-openapi.yml
  format: yaml
  label: Hermes Plant Agent Commerce Assurance API
  slug: hermesplant-com-agent-commerce-assurance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-agent-commerce-assurance-api-openapi.yml
- filename: hermesplant-com-agent-safety-api-openapi.yml
  format: yaml
  label: Hermes Plant Agent Safety API
  slug: hermesplant-com-agent-safety-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-agent-safety-api-openapi.yml
- filename: hermesplant-com-agent-spend-api-openapi.yml
  format: yaml
  label: Hermes Plant Agent Spend API
  slug: hermesplant-com-agent-spend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-agent-spend-api-openapi.yml
- filename: hermesplant-com-assurance-api-openapi.yml
  format: yaml
  label: Hermes Plant Assurance API
  slug: hermesplant-com-assurance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-assurance-api-openapi.yml
- filename: hermesplant-com-billing-portal-api-openapi.yml
  format: yaml
  label: Hermes Plant Billing Portal API
  slug: hermesplant-com-billing-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-billing-portal-api-openapi.yml
- filename: hermesplant-com-catalog-api-openapi.yml
  format: yaml
  label: Hermes Plant Catalog API
  slug: hermesplant-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-catalog-api-openapi.yml
- filename: hermesplant-com-checkout-api-openapi.yml
  format: yaml
  label: Hermes Plant Checkout API
  slug: hermesplant-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-checkout-api-openapi.yml
- filename: hermesplant-com-content-api-openapi.yml
  format: yaml
  label: Hermes Plant Content API
  slug: hermesplant-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-content-api-openapi.yml
- filename: hermesplant-com-email-api-openapi.yml
  format: yaml
  label: Hermes Plant Email API
  slug: hermesplant-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-email-api-openapi.yml
- filename: hermesplant-com-finance-api-openapi.yml
  format: yaml
  label: Hermes Plant Finance API
  slug: hermesplant-com-finance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-finance-api-openapi.yml
- filename: hermesplant-com-health-api-openapi.yml
  format: yaml
  label: Hermes Plant Health API
  slug: hermesplant-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-health-api-openapi.yml
- filename: hermesplant-com-investment-analysis-api-openapi.yml
  format: yaml
  label: Hermes Plant Investment Analysis API
  slug: hermesplant-com-investment-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-investment-analysis-api-openapi.yml
- filename: hermesplant-com-mcp-api-openapi.yml
  format: yaml
  label: Hermes Plant MCP API
  slug: hermesplant-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-mcp-api-openapi.yml
- filename: hermesplant-com-portfolio-risk-analysis-api-openapi.yml
  format: yaml
  label: Hermes Plant Portfolio Risk Analysis API
  slug: hermesplant-com-portfolio-risk-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-portfolio-risk-analysis-api-openapi.yml
- filename: hermesplant-com-purchase-api-openapi.yml
  format: yaml
  label: Hermes Plant Purchase API
  slug: hermesplant-com-purchase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-purchase-api-openapi.yml
- filename: hermesplant-com-wallet-risk-scoring-api-openapi.yml
  format: yaml
  label: Hermes Plant Wallet Risk Scoring API
  slug: hermesplant-com-wallet-risk-scoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-wallet-risk-scoring-api-openapi.yml
- filename: hermesplant-com-x402-api-openapi.yml
  format: yaml
  label: Hermes Plant X402 API
  slug: hermesplant-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hermesplant-com/openapi/hermesplant-com-x402-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Hermes Plant Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hermes Plant publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hermes Plant API on a user''s behalf.


  Tokens are issued from https://hermesplant.com/api/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hermes Plant
provider_slug: hermesplant-com
schemes:
- description: Register at POST /api/auth/register, then obtain a token from POST /api/auth/token using client_credentials.
  flows:
  - flow: clientCredentials
    tokenUrl: https://hermesplant.com/api/auth/token
  name: oauth2
  source: openapi/hermesplant-com-openapi.json
scope_count: 3
scope_names:
- billing:manage
- catalog:read
- checkout:create
scopes:
- description: Open Stripe billing portal for subscribers
  flows:
  - clientCredentials
  scope: billing:manage
- description: Read the product catalog
  flows:
  - clientCredentials
  scope: catalog:read
- description: Start checkout sessions
  flows:
  - clientCredentials
  scope: checkout:create
slug: hermesplant-com-scopes
source_filename: hermesplant-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hermesplant-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/hermesplant-com-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://hermesplant.com/api/auth/token\n  description: Register at POST /api/auth/register, then obtain a token from POST /api/auth/token\n    using client_credentials.\nscopes:\n- scope: billing:manage\n  description: Open Stripe billing portal for subscribers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/hermesplant-com-openapi.json\n- scope: catalog:read\n  description: Read the product catalog\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/hermesplant-com-openapi.json\n- scope: checkout:create\n  description: Start checkout sessions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/hermesplant-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hermesplant-com/scopes/hermesplant-com-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Company
- Artificial Intelligence
- Agent Safety
- Finance
- Compliance
- Automation
token_bound: false
token_urls:
- https://hermesplant.com/api/auth/token
---
