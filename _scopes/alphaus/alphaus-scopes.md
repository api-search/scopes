---
api_specs:
- filename: alphaus-blueapi-openapi-original.json
  format: json
  label: Blue API
  slug: blue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/openapi/alphaus-blueapi-openapi-original.json
authorization_urls: []
description: ''
docs: https://labs.alphaus.cloud/docs/blueapi/authentication/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Alphaus Scopes
name_suffix: OAuth Scopes
note: Blue API uses OAuth2 client credentials with a single openid scope; authorization granularity is handled by RBAC (Iam service), not a published OAuth scope catalog.
overview: 'Alphaus publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alphaus API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alphaus
provider_slug: alphaus
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  token_urls:
  - https://login.alphaus.cloud/ripple/access_token
  - https://login.alphaus.cloud/access_token
scope_count: 1
scope_names:
- openid
scopes:
- description: OpenID Connect scope requested in the client_credentials token exchange. Blue API documents scope=openid for the access-token request; fine-grained authorization beyond the token is enforced by the Iam service (RBAC roles/permissions), not by additional OAuth scopes.
  flows:
  - clientCredentials
  scope: openid
slug: alphaus-scopes
source_filename: alphaus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://labs.alphaus.cloud/docs/blueapi/authentication/\ndocs: https://labs.alphaus.cloud/docs/blueapi/authentication/\nschemes:\n  - name: OAuth2ClientCredentials\n    flow: clientCredentials\n    token_urls:\n      - https://login.alphaus.cloud/ripple/access_token\n      - https://login.alphaus.cloud/access_token\nscopes:\n  - scope: openid\n    description: >-\n      OpenID Connect scope requested in the client_credentials token exchange. Blue API documents\n      scope=openid for the access-token request; fine-grained authorization beyond the token is\n      enforced by the Iam service (RBAC roles/permissions), not by additional OAuth scopes.\n    flows: [clientCredentials]\n    sources: [https://labs.alphaus.cloud/docs/blueapi/authentication/]\nnote: >-\n  Blue API uses OAuth2 client credentials with a single openid scope; authorization granularity is\n  handled by RBAC (Iam service), not a published OAuth scope catalog.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphaus/refs/heads/main/scopes/alphaus-scopes.yml
summary_line: 1 scope
tags:
- Company
- FinOps
- Cloud Cost Management
- Cloud
- Billing
- Multi-Cloud
- Azure
- GCP
- gRPC
- Cost Optimization
- Reseller Billing
- API
token_urls: []
---
