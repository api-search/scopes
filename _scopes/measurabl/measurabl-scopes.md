---
api_specs:
- filename: measurabl-core-openapi.yml
  format: yaml
  label: Measurabl Core API
  slug: measurabl-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-core-openapi.yml
- filename: measurabl-esgx-buildings-openapi.yml
  format: yaml
  label: Measurabl ESGx Buildings API
  slug: measurabl-esgx-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-esgx-buildings-openapi.yml
- filename: measurabl-esgx-securities-openapi.yml
  format: yaml
  label: Measurabl ESGx Securities API
  slug: measurabl-esgx-securities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-esgx-securities-openapi.yml
- filename: measurabl-esgx-securities-compliance-files-openapi.yml
  format: yaml
  label: Measurabl ESGx Securities Compliance Files API
  slug: measurabl-esgx-securities-compliance-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-esgx-securities-compliance-files-openapi.yml
- filename: measurabl-partners-openapi.yml
  format: yaml
  label: Measurabl Partner API
  slug: measurabl-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-partners-openapi.yml
authorization_urls: []
description: ''
docs: https://support.measurabl.com/hc/en-us/articles/15889532915085-How-do-I-authenticate-with-Measurabl-s-Core-API-
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Measurabl Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Measurabl uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.measurabl.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Measurabl
provider_slug: measurabl
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.measurabl.com/token
  name: OAuth2
  source: openapi/measurabl-core-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.measurabl.com/token
  name: OAuth2
  source: openapi/measurabl-esgx-buildings-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.measurabl.com/token
  name: OAuth2
  source: openapi/measurabl-esgx-securities-compliance-files-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.measurabl.com/token
  name: OAuth2
  source: openapi/measurabl-esgx-securities-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.measurabl.com/token
  name: OAuth2
  source: openapi/measurabl-partners-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: measurabl-scopes
source_filename: measurabl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/measurabl-core-openapi.yml, openapi/measurabl-esgx-buildings-openapi.yml, openapi/measurabl-esgx-securities-compliance-files-openapi.yml,\n  openapi/measurabl-esgx-securities-openapi.yml, openapi/measurabl-partners-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/measurabl-core-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.measurabl.com/token\n- name: OAuth2\n  source: openapi/measurabl-esgx-buildings-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.measurabl.com/token\n- name: OAuth2\n  source: openapi/measurabl-esgx-securities-compliance-files-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.measurabl.com/token\n- name: OAuth2\n  source: openapi/measurabl-esgx-securities-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.measurabl.com/token\n- name: OAuth2\n  source: openapi/measurabl-partners-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.measurabl.com/token\nscopes: []\ndocs: https://support.measurabl.com/hc/en-us/articles/15889532915085-How-do-I-authenticate-with-Measurabl-s-Core-API-\nsummary: 'Measurabl declares an OAuth 2.0 clientCredentials scheme in all five specs but its scopes map is EMPTY\n  in every one, and no scope, permission or role reference page exists in the public documentation. This is a recorded\n  negative, not a search gap: Measurabl has no scope surface. Authorization is entitlement-based per portfolio and\n  per dataset, enforced as 403 at request time.'\nscopes_found: 0\nauthorization_model: entitlement-based (no scopes)\nsearched:\n- https://api.measurabl.com/api-docs/ (all five OpenAPI documents)\n- https://www.measurabl.com/measurabl-api-faq/\n- Measurabl help center authentication and Core API FAQ articles (Cloudflare-gated to automated fetch)\ncross_links:\n  authentication: authentication/measurabl-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/scopes/measurabl-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- esg
- real-estate
- sustainability
- carbon-accounting
- energy-management
- building-performance
- climate-risk
- benchmarking
- compliance
- proptech
- utility-data
- capital-markets
token_urls:
- https://api.measurabl.com/token
---
