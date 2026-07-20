---
authorization_urls:
- https://shopify.com/authentication/17555355/oauth/authorize
description: ''
docs: https://crowdmade.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Crowdmade Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CrowdMade publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CrowdMade API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/17555355/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CrowdMade
provider_slug: crowdmade
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/17555355/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/17555355/oauth/token
  name: ShopifyCustomerAccountsOIDC
  source: well-known/crowdmade-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for agent-driven customer operations.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: crowdmade-scopes
source_filename: crowdmade-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://crowdmade.com/.well-known/openid-configuration\ndocs: https://crowdmade.com/.well-known/oauth-authorization-server\nnotes: >-\n  OAuth/OIDC scopes advertised by the Shopify Customer Accounts authorization\n  server that fronts crowdmade.com. These are provider-published (Shopify)\n  scopes, not CrowdMade-specific, captured from the live discovery document.\nschemes:\n  - name: ShopifyCustomerAccountsOIDC\n    source: well-known/crowdmade-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://shopify.com/authentication/17555355/oauth/authorize\n        tokenUrl: https://shopify.com/authentication/17555355/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token.\n    flows: [authorizationCode]\n    sources: [well-known/crowdmade-openid-configuration.json]\n  - scope: email\n    description: Access the customer's email\
  \ address and verification status.\n    flows: [authorizationCode]\n    sources: [well-known/crowdmade-openid-configuration.json]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n    flows: [authorizationCode]\n    sources: [well-known/crowdmade-openid-configuration.json]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Shopify Customer Account MCP API for agent-driven customer operations.\n    flows: [authorizationCode]\n    sources: [well-known/crowdmade-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdmade/refs/heads/main/scopes/crowdmade-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Commerce
- E-Commerce
- Merchandise
- Creator Economy
- Shopify
- Agent Commerce
- MCP
- Universal Commerce Protocol
token_urls:
- https://shopify.com/authentication/17555355/oauth/token
---
