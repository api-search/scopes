---
api_specs:
- filename: simon-data-event-ingestion-openapi.yml
  format: yaml
  label: Simon Data Event Ingestion API
  slug: simon-data-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-event-ingestion-openapi.yml
- filename: simon-data-contact-openapi.yml
  format: yaml
  label: Simon Data Contact API
  slug: simon-data-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-contact-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.simondata.com/reference/getting-started
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Simon Data Scopes
name_suffix: OAuth Scopes
note: Simon Data does not publish OAuth scopes; its Audience/Contact API uses bearer tokens issued by a Client Solutions Manager and the Signal event API uses a shared partner secret, with OAuth 2.0 only referenced for outbound integrations to third-party systems (https://docs.simondata.com/reference/getting-started).
overview: 'Simon Data uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.simondata.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Simon Data
provider_slug: simon-data
schemes:
- description: OAuth 2.0 authentication required for all endpoints.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.simondata.com/oauth/token
  name: oauth2
  source: openapi/simon-data-contact-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: simon-data-scopes
source_filename: simon-data-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/simon-data-contact-openapi.yml\ndocs: https://docs.simondata.com/reference/getting-started\nnote: Simon Data does not publish OAuth scopes; its Audience/Contact API uses bearer\n  tokens issued by a Client Solutions Manager and the Signal event API uses a shared\n  partner secret, with OAuth 2.0 only referenced for outbound integrations to third-party\n  systems (https://docs.simondata.com/reference/getting-started).\nschemes:\n- name: oauth2\n  source: openapi/simon-data-contact-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.simondata.com/oauth/token\n  description: OAuth 2.0 authentication required for all endpoints.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/scopes/simon-data-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Customer Data Platform
- CDP
- Marketing Automation
- Audience Segmentation
- Event Tracking
- Data Ingestion
- Personalization
- Marketing Technology
token_urls:
- https://api.simondata.com/oauth/token
---
