---
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by the Shopify Customer Account API OIDC discovery document served on the fitbody.mx host (/.well-known/openid-configuration, issuer https://shopify.com/authentication/24443367). The Fit Body Co publishes no first-party API; these scopes belong to Shopify's Customer Account API platform capability enabled for this shop. Captured verbatim from scopes_supported in the live discovery document. Notably includes a customer-account-mcp-api:full scope gating Shopify's Customer Account MCP API.
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: The Fit Body Co Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'The Fit Body Co publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the The Fit Body Co API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Fit Body Co
provider_slug: the-fit-body-co
schemes:
- docs: https://shopify.dev/docs/api/customer
  issuer: https://shopify.com/authentication/24443367
  name: shopifyCustomerAccountOIDC
  openIdConnectUrl: https://fitbody.mx/.well-known/openid-configuration
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token identifying the customer.
  flows: []
  scope: openid
- description: Access the customer's email address and email_verified claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer.
  flows: []
  scope: customer-account-mcp-api:full
slug: the-fit-body-co-scopes
source_filename: the-fit-body-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://fitbody.mx/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by the Shopify Customer Account\n  API OIDC discovery document served on the fitbody.mx host\n  (/.well-known/openid-configuration, issuer https://shopify.com/authentication/24443367).\n  The Fit Body Co publishes no first-party API; these scopes belong to Shopify's\n  Customer Account API platform capability enabled for this shop. Captured\n  verbatim from scopes_supported in the live discovery document. Notably includes\n  a customer-account-mcp-api:full scope gating Shopify's Customer Account MCP API.\nschemes:\n  - name: shopifyCustomerAccountOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://fitbody.mx/.well-known/openid-configuration\n    issuer: https://shopify.com/authentication/24443367\n    docs: https://shopify.dev/docs/api/customer\nscopes:\n\
  \  - scope: openid\n    description: OpenID Connect authentication; issue an ID token identifying the customer.\n    schemes: [shopifyCustomerAccountOIDC]\n  - scope: email\n    description: Access the customer's email address and email_verified claim.\n    schemes: [shopifyCustomerAccountOIDC]\n  - scope: customer-account-api:full\n    description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n    schemes: [shopifyCustomerAccountOIDC]\n  - scope: customer-account-mcp-api:full\n    description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer.\n    schemes: [shopifyCustomerAccountOIDC]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-fit-body-co/refs/heads/main/scopes/the-fit-body-co-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Sports Nutrition
- Dietary Supplements
- E-commerce
- Health and Wellness
- Consumer Products
- Mexico
- Shopify
token_urls: []
---
