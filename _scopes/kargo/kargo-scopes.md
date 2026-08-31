---
api_specs:
- filename: kargo-public-graphql.postman_collection.json
  format: json
  label: Kargo Public GraphQL API
  slug: kargo-public-graphql-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/kargo/refs/heads/main/postman/kargo-public-graphql.postman_collection.json
- filename: kargo-documents-api-openapi.yml
  format: yaml
  label: Kargo Documents API
  slug: kargo-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kargo/refs/heads/main/openapi/kargo-documents-api-openapi.yml
- filename: kargo-sku-master-api-openapi.yml
  format: yaml
  label: Kargo SKU Master API
  slug: kargo-sku-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kargo/refs/heads/main/openapi/kargo-sku-master-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.kargo.ai/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Kargo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kargo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://mykargo.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kargo
provider_slug: kargo
schemes:
- flows:
  - audience: https://api.kargo.zone/public_graphql
    flow: clientCredentials
    tokenUrl: https://mykargo.us.auth0.com/oauth/token
  name: auth0-client-credentials
  source: https://docs.kargo.ai/authentication
scope_count: 0
scope_names: []
scopes: []
slug: kargo-scopes
source_filename: kargo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://mykargo.us.auth0.com/.well-known/openid-configuration\ndocs: https://docs.kargo.ai/authentication\nsummary:\n  api_scopes_published: false\n  note: 'Kargo''s public API uses the OAuth 2.0 client-credentials grant with an\n    `audience` of https://api.kargo.zone/public_graphql and no `scope` parameter.\n    Kargo publishes no scope or permission reference for the API audience, so there\n    are no API scopes to record. Authorization is enforced per business/facility on\n    the token (the OpenAPI documents a 403 \"Token lacks permission for the given\n    business/facility\"), not by scope.'\nschemes:\n- name: auth0-client-credentials\n  source: https://docs.kargo.ai/authentication\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://mykargo.us.auth0.com/oauth/token\n    audience: https://api.kargo.zone/public_graphql\nscopes: []\nauthorization_server_scopes_supported:\n  note: 'These are the OIDC scopes advertised\
  \ by Kargo''s Auth0 tenant discovery\n    document for interactive sign-in to the Kargo dashboard. They are Auth0 standard\n    OIDC scopes and do NOT gate the public API audience.'\n  values:\n  - openid\n  - profile\n  - offline_access\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n  - identities\n  - phone\n  - address\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kargo/refs/heads/main/scopes/kargo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Logistics
- Supply Chain
- Warehouse
- Computer Vision
- Artificial Intelligence
- Shipping
- Inventory
- Industrial Automation
- Freight
- GraphQL
- Webhooks
token_urls:
- https://mykargo.us.auth0.com/oauth/token
---
