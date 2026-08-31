---
api_specs:
- filename: university-of-melbourne-core-api-openapi.yml
  format: yaml
  label: University of Melbourne Core API
  slug: university-of-melbourne-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/openapi/university-of-melbourne-core-api-openapi.yml
- filename: university-of-melbourne-datasets-api-openapi.yml
  format: yaml
  label: University of Melbourne Datasets API
  slug: university-of-melbourne-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/openapi/university-of-melbourne-datasets-api-openapi.yml
- filename: university-of-melbourne-discovery-api-openapi.yml
  format: yaml
  label: University of Melbourne Discovery API
  slug: university-of-melbourne-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/openapi/university-of-melbourne-discovery-api-openapi.yml
- filename: university-of-melbourne-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Melbourne OAI PMH API
  slug: university-of-melbourne-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/openapi/university-of-melbourne-oai-pmh-api-openapi.yml
authorization_urls: []
description: 'The only enumerable scope set on any University of Melbourne surface. It comes from the OpenID Connect discovery document served by the University''s Okta tenancy at sso.unimelb.edu.au. The operator is `tenant`: Okta defines and implements these scopes, the University configures and hosts them under its own name. Nothing derived from this document is credited to the institution''s engineering.

  The University''s two publicly callable APIs — SUDO and Minerva Access — are unauthenticated for read and publish no scope model at all.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Melbourne Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Melbourne uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Melbourne
provider_slug: university-of-melbourne
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-melbourne-scopes
source_filename: university-of-melbourne-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: https://sso.unimelb.edu.au/.well-known/openid-configuration (HTTP 200, 2026-08-19)\nx-operator: tenant\ndescription: >-\n  The only enumerable scope set on any University of Melbourne surface. It\n  comes from the OpenID Connect discovery document served by the University's\n  Okta tenancy at sso.unimelb.edu.au. The operator is `tenant`: Okta defines\n  and implements these scopes, the University configures and hosts them under\n  its own name. Nothing derived from this document is credited to the\n  institution's engineering.\n\n  The University's two publicly callable APIs — SUDO and Minerva Access — are\n  unauthenticated for read and publish no scope model at all.\nscopes:\n  - name: openid\n    description: Required OIDC scope; requests an ID token.\n  - name: profile\n    description: Basic profile claims.\n  - name: email\n    description: Email address claims.\n  - name: address\n    description: Postal address claim.\n\
  \  - name: phone\n    description: Phone number claims.\n  - name: offline_access\n    description: Requests a refresh token.\n  - name: groups\n    description: >-\n      Okta group membership claim. In a university deployment this is the claim\n      that typically carries staff/student/faculty affiliation to downstream\n      applications.\ngrant_types_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  - 'urn:openid:params:grant-type:ciba'\n  - 'urn:okta:params:oauth:grant-type:otp'\n  - 'urn:okta:params:oauth:grant-type:oob'\n  - 'http://auth0.com/oauth/grant-type/mfa-otp'\n  - 'http://auth0.com/oauth/grant-type/mfa-oob'\nnotes: >-\n  The presence of the `password` (Resource Owner Password Credentials) grant in\n  a 2026 discovery document is worth recording; OAuth 2.1 removes it. It is\n  offered by the platform here, which is not the same as the University\n  enabling it for any given application.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-melbourne/refs/heads/main/scopes/university-of-melbourne-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Australia
- Group of Eight
- Research
- Research Data
- Research Repository
- Open Data
- Geospatial
- Identity Federation
- Library
token_urls: []
---
