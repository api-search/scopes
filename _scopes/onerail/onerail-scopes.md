---
api_specs:
- filename: onerail-delivery-api-openapi.yml
  format: yaml
  label: OneRail Delivery API
  slug: onerail-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onerail/refs/heads/main/openapi/onerail-delivery-api-openapi.yml
- filename: onerail-operations-api-openapi.yml
  format: yaml
  label: OneRail Operations API
  slug: onerail-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onerail/refs/heads/main/openapi/onerail-operations-api-openapi.yml
authorization_urls:
- https://dummy-unused-url.com
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Onerail Scopes
name_suffix: OAuth Scopes
note: 'The Operations API declares an oauth2 securityScheme but publishes ZERO scopes: the flow object is empty and no operation carries an oauth2 security requirement with scopes. The spec itself states the authorizationUrl and tokenUrl values ("https://dummy-unused-url.com") are placeholders present only to satisfy the OpenAPI schema - OneRail validates access tokens minted by the customer''s own IdP (e.g. Okta) and the real IdP URLs are configured out of band per deployment. No scopes or permissions reference page exists on the OneRail Developer Hub. The practical authorization model is the organization App ID / API Key pair plus platform roles (Location/Ops User, View Only, Global Admin) assigned in the UI - see authentication/onerail-authentication.yml.'
overview: 'OneRail uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://dummy-unused-url.com.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OneRail
provider_slug: onerail
schemes:
- description: 'OAuth 2.0 access token validated by the Operations service (e.g. Okta-backed

    integrations). Clients obtain tokens from their own IdP outside of this API

    and call endpoints with `Authorization: OAuth <access_token>`. The

    `authorizationUrl` and `tokenUrl` values below are placeholders only to

    satisfy the OpenAPI schema; this service does not call them directly and the

    real IdP URLs are configured via environment and introspection logic in code.'
  flows:
  - authorizationUrl: https://dummy-unused-url.com
    flow: authorizationCode
    tokenUrl: https://dummy-unused-url.com
  name: OAuth
  source: openapi/onerail-operations-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: onerail-scopes
source_filename: onerail-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/onerail-operations-api-openapi.yml\nschemes:\n- name: OAuth\n  source: openapi/onerail-operations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dummy-unused-url.com\n    tokenUrl: https://dummy-unused-url.com\n  description: 'OAuth 2.0 access token validated by the Operations service (e.g. Okta-backed\n\n    integrations). Clients obtain tokens from their own IdP outside of this API\n\n    and call endpoints with `Authorization: OAuth <access_token>`. The\n\n    `authorizationUrl` and `tokenUrl` values below are placeholders only to\n\n    satisfy the OpenAPI schema; this service does not call them directly and the\n\n    real IdP URLs are configured via environment and introspection logic in code.'\nscopes: []\ndocs: null\nnote: 'The Operations API declares an oauth2 securityScheme but publishes ZERO scopes: the flow object\n  is empty and no operation carries an oauth2 security\
  \ requirement with scopes. The spec itself states\n  the authorizationUrl and tokenUrl values (\"https://dummy-unused-url.com\") are placeholders present only\n  to satisfy the OpenAPI schema - OneRail validates access tokens minted by the customer''s own IdP (e.g.\n  Okta) and the real IdP URLs are configured out of band per deployment. No scopes or permissions reference\n  page exists on the OneRail Developer Hub. The practical authorization model is the organization App\n  ID / API Key pair plus platform roles (Location/Ops User, View Only, Global Admin) assigned in the UI\n  - see authentication/onerail-authentication.yml.'\nplaceholder_urls: true\nsearched: https://developer.onerail.io/hc/en-us - no scopes/permissions reference published\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onerail/refs/heads/main/scopes/onerail-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- last-mile-delivery
- delivery-orchestration
- logistics
- supply-chain
- route-optimization
- courier-network
- shipping
- fleet-management
- transportation
- order-management
- webhooks
- final-mile
token_urls:
- https://dummy-unused-url.com
---
