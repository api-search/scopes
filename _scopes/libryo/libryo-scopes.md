---
authorization_urls: []
description: The OAuth 2.0 scopes Libryo documents for partner integrations. Libryo publishes no OpenAPI definition, so these are taken verbatim from the scope list in its public OAuth integration guide rather than derived from a spec. Scopes are requested as a space-delimited string on the authorization request and describe read access to the authorizing user's regulatory content.
docs: https://github.com/libryo/libryo-api-oauth-docs
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Libryo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Libryo publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Libryo API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Libryo
provider_slug: libryo
schemes:
- authorizationUrl: https://my.libryo.com/oauth/authorize
  docs: https://github.com/libryo/libryo-api-oauth-docs
  grant_types:
  - authorization_code
  name: libryoOAuth2
  notes: Scopes are passed space-delimited, e.g. scope=view-legal-report search-legislation list-libryos
  tokenUrl: https://api.libryo.com/api/v1/oauth/token
  type: oauth2
scope_count: 3
scope_names:
- view-legal-report
- search-legislation
- list-libryos
scopes:
- description: View the authorizing user's legal report — the compiled register of legal obligations applicable to their sites.
  flows: []
  scope: view-legal-report
- description: Search the Libryo legislation corpus on behalf of the authorizing user.
  flows: []
  scope: search-legislation
- description: List the "Libryos" available to the authorizing user. A Libryo is a site-specific, filtered stream of the legislation that applies to one operation or location.
  flows: []
  scope: list-libryos
slug: libryo-scopes
source_filename: libryo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/libryo/libryo-api-oauth-docs\ndocs: https://github.com/libryo/libryo-api-oauth-docs\ndescription: >-\n  The OAuth 2.0 scopes Libryo documents for partner integrations. Libryo publishes no\n  OpenAPI definition, so these are taken verbatim from the scope list in its public OAuth\n  integration guide rather than derived from a spec. Scopes are requested as a\n  space-delimited string on the authorization request and describe read access to the\n  authorizing user's regulatory content.\nschemes:\n- name: libryoOAuth2\n  type: oauth2\n  grant_types:\n  - authorization_code\n  authorizationUrl: https://my.libryo.com/oauth/authorize\n  tokenUrl: https://api.libryo.com/api/v1/oauth/token\n  docs: https://github.com/libryo/libryo-api-oauth-docs\n  notes: >-\n    Scopes are passed space-delimited, e.g.\n    scope=view-legal-report search-legislation list-libryos\nscopes:\n- scope: view-legal-report\n  description:\
  \ >-\n    View the authorizing user's legal report — the compiled register of legal obligations\n    applicable to their sites.\n  schemes:\n  - libryoOAuth2\n- scope: search-legislation\n  description: >-\n    Search the Libryo legislation corpus on behalf of the authorizing user.\n  schemes:\n  - libryoOAuth2\n- scope: list-libryos\n  description: >-\n    List the \"Libryos\" available to the authorizing user. A Libryo is a site-specific,\n    filtered stream of the legislation that applies to one operation or location.\n  schemes:\n  - libryoOAuth2\ncompleteness: >-\n  The public guide states these are \"the scopes that are currently available\", so this is\n  believed to be the full published scope surface as of the last commit to the docs repo.\n  Libryo may issue additional scopes to partners under agreement; no write scopes are\n  documented publicly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/libryo/refs/heads/main/scopes/libryo-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Regulatory Compliance
- Legal Tech
- Environmental Health and Safety
- Governance Risk and Compliance
- Legal Registers
- Regulatory Change Management
- Sustainability
- OAuth
token_urls: []
---
