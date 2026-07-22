---
authorization_urls:
- https://shopify.com/authentication/50476449942/oauth/authorize
description: OAuth scopes advertised by the Shopify customer-accounts authorization server backing Urban Revivo's global storefront, taken verbatim from the scopes_supported list in the live OIDC discovery document (saved at well-known/urban-revivo-openid-configuration.json).
docs: https://global.urbanrevivo.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Urban Revivo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Urban Revivo publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Urban Revivo API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/50476449942/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Urban Revivo
provider_slug: urban-revivo
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/50476449942/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/50476449942/oauth/token
  name: shopify-customer-accounts-oidc
  source: well-known/urban-revivo-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication (ID token issuance).
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify customer-account MCP API surface (agentic access on behalf of the authenticated customer).
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: urban-revivo-scopes
source_filename: urban-revivo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://global.urbanrevivo.com/.well-known/openid-configuration\ndocs: https://global.urbanrevivo.com/.well-known/openid-configuration\ndescription: >-\n  OAuth scopes advertised by the Shopify customer-accounts authorization\n  server backing Urban Revivo's global storefront, taken verbatim from the\n  scopes_supported list in the live OIDC discovery document (saved at\n  well-known/urban-revivo-openid-configuration.json).\nschemes:\n  - name: shopify-customer-accounts-oidc\n    source: well-known/urban-revivo-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/50476449942/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/50476449942/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication (ID token issuance).\n    flows: [authorizationCode]\n    sources: [well-known/urban-revivo-openid-configuration.json]\n\
  \  - scope: email\n    description: Access to the customer's email address claim.\n    flows: [authorizationCode]\n    sources: [well-known/urban-revivo-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API for the authenticated customer.\n    flows: [authorizationCode]\n    sources: [well-known/urban-revivo-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Shopify customer-account MCP API surface (agentic access on behalf of the authenticated customer).\n    flows: [authorizationCode]\n    sources: [well-known/urban-revivo-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-revivo/refs/heads/main/scopes/urban-revivo-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Fashion
- Retail
- eCommerce
- Apparel
- Agentic Commerce
token_urls:
- https://shopify.com/authentication/50476449942/oauth/token
---
