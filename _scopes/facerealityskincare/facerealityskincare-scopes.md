---
authorization_urls: []
description: OAuth 2.0 scopes advertised by the Shopify Customer Account API discovery document for Face Reality Skincare (scopes_supported). openid/email are standard OIDC scopes; the customer-account-api and customer-account-mcp-api full scopes gate access to the customer account GraphQL API and its MCP surface respectively.
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Facerealityskincare Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Face Reality Skincare publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Face Reality Skincare API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Face Reality Skincare
provider_slug: facerealityskincare
schemes:
- authorizationUrl: https://account.facerealityskincare.com/authentication/oauth/authorize
  name: shopifyCustomerAccountOAuth
  tokenUrl: https://account.facerealityskincare.com/authentication/oauth/token
  type: oauth2
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; returns an ID token identifying the customer.
  flows: []
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-account MCP surface on behalf of the signed-in customer.
  flows: []
  scope: customer-account-mcp-api:full
slug: facerealityskincare-scopes
source_filename: facerealityskincare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://facerealityskincare.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\ndescription: >-\n  OAuth 2.0 scopes advertised by the Shopify Customer Account API discovery\n  document for Face Reality Skincare (scopes_supported). openid/email are\n  standard OIDC scopes; the customer-account-api and customer-account-mcp-api\n  full scopes gate access to the customer account GraphQL API and its MCP\n  surface respectively.\nschemes:\n- name: shopifyCustomerAccountOAuth\n  type: oauth2\n  authorizationUrl: https://account.facerealityskincare.com/authentication/oauth/authorize\n  tokenUrl: https://account.facerealityskincare.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; returns an ID token identifying the customer.\n  schemes:\n  - shopifyCustomerAccountOAuth\n- scope: email\n  description: Access to the customer's email address and email_verified\
  \ claim.\n  schemes:\n  - shopifyCustomerAccountOAuth\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  schemes:\n  - shopifyCustomerAccountOAuth\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP surface on behalf of the signed-in customer.\n  schemes:\n  - shopifyCustomerAccountOAuth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facerealityskincare/refs/heads/main/scopes/facerealityskincare-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Skincare
- Beauty
- Cosmetics
- Ecommerce
- Shopify
- Commerce
- Agent Commerce
- MCP
token_urls: []
---
