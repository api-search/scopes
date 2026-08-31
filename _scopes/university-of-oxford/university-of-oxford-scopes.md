---
api_specs:
- filename: university-of-oxford-iiif-api-openapi.yml
  format: yaml
  label: University of Oxford IIIF API
  slug: university-of-oxford-iiif-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-oxford/refs/heads/main/openapi/university-of-oxford-iiif-api-openapi.yml
- filename: university-of-oxford-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Oxford OAI PMH API
  slug: university-of-oxford-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-oxford/refs/heads/main/openapi/university-of-oxford-oai-pmh-api-openapi.yml
- filename: university-of-oxford-repository-api-openapi.yml
  format: yaml
  label: University of Oxford Repository API
  slug: university-of-oxford-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-oxford/refs/heads/main/openapi/university-of-oxford-repository-api-openapi.yml
- filename: university-of-oxford-textarchive-api-openapi.yml
  format: yaml
  label: University of Oxford Text Archive API
  slug: university-of-oxford-textarchive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-oxford/refs/heads/main/openapi/university-of-oxford-textarchive-api-openapi.yml
authorization_urls: []
description: There are none, and the absence is the finding rather than a gap in our research. No institution-operated Oxford API uses OAuth, OIDC or any token-based authorization, so there is no scope vocabulary to record. This file exists so that a reader does not have to wonder whether scopes were simply never looked for.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Oxford Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Oxford uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Oxford
provider_slug: university-of-oxford
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-oxford-scopes
source_filename: university-of-oxford-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: University of Oxford — authorization scopes\ndescription: >-\n  There are none, and the absence is the finding rather than a gap in our research. No\n  institution-operated Oxford API uses OAuth, OIDC or any token-based authorization, so there\n  is no scope vocabulary to record. This file exists so that a reader does not have to wonder\n  whether scopes were simply never looked for.\ngenerated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes of every surface in apis.yml. No .well-known/oauth-authorization-server,\n  .well-known/openid-configuration, token endpoint or client-registration page was found on\n  any ox.ac.uk host examined.\nscopes: []\nnotes:\n  - >-\n    The nearest equivalent to authorization at Oxford is SAML attribute release through the\n    Shibboleth IdP to 35 federated service providers. SAML attribute bundles are not API\n    scopes and are deliberately not recorded as such here.\n  - >-\n    The tenant surfaces in apis.yml (Figshare, Ex\
  \ Libris Primo VE, Instructure Canvas, CoreHR)\n    do have OAuth scope vocabularies. Those belong to the vendors' own catalog entries, not to\n    Oxford, and are not reproduced here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-oxford/refs/heads/main/scopes/university-of-oxford-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Research
- United Kingdom
- Russell Group
- Research Repository
- Library
- Digital Collections
- IIIF
- OAI-PMH
- Identity Federation
- Open Access
- Research Computing
token_urls: []
---
