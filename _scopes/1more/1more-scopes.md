---
authorization_urls:
- https://shopify.com/authentication/11404626/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: 1More Scopes
name_suffix: OAuth Scopes
note: These are the scopes advertised by the OAuth 2.0 / OpenID Connect authorization server that 1MORE's storefront points at for shopper accounts (Shopify customer accounts, issuer https://shopify.com/authentication/11404626, discovered from 1MORE's own host). They govern a logged-in shopper's own account, not any 1MORE developer programme - 1MORE publishes none. Descriptions below are the scope semantics as documented by the issuer's discovery document and Shopify's customer account model; no scope has been invented and none is asserted beyond the four strings the document returns in scopes_supported.
overview: '1MORE publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 1MORE API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/11404626/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 1MORE
provider_slug: 1more
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/11404626/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/11404626/oauth/token
  name: shopify-customer-account-oauth2
  source: well-known/1more-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the shopper.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the shopper's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the authenticated shopper's own customer account data (orders, addresses, profile) via the customer account API.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the authenticated shopper's own customer account data via the MCP transport of the customer account API.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: 1more-scopes
source_filename: 1more-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://usa.1more.com/.well-known/openid-configuration\nnote: >-\n  These are the scopes advertised by the OAuth 2.0 / OpenID Connect authorization\n  server that 1MORE's storefront points at for shopper accounts (Shopify customer\n  accounts, issuer https://shopify.com/authentication/11404626, discovered from\n  1MORE's own host). They govern a logged-in shopper's own account, not any 1MORE\n  developer programme - 1MORE publishes none. Descriptions below are the scope\n  semantics as documented by the issuer's discovery document and Shopify's customer\n  account model; no scope has been invented and none is asserted beyond the four\n  strings the document returns in scopes_supported.\nschemes:\n- name: shopify-customer-account-oauth2\n  source: well-known/1more-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/11404626/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/11404626/oauth/token\n\
  scope_count: 4\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the shopper.\n  flows: [authorizationCode]\n  sources: [well-known/1more-openid-configuration.json]\n- scope: email\n  description: Releases the shopper's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/1more-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the authenticated shopper's own customer account data (orders, addresses, profile) via the customer account API.\n  flows: [authorizationCode]\n  sources: [well-known/1more-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the authenticated shopper's own customer account data via the MCP transport of the customer account API.\n  flows: [authorizationCode]\n  sources: [well-known/1more-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1more/refs/heads/main/scopes/1more-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Electronics
- Audio
- Headphones
- Retail
- E-Commerce
- Agent Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
token_urls:
- https://shopify.com/authentication/11404626/oauth/token
---
