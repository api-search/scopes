---
api_specs:
- filename: renaissance-lexile-api-openapi.yml
  format: yaml
  label: Lexile API
  slug: lexile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-lexile-api-openapi.yml
- filename: renaissance-classes-api-openapi.yml
  format: yaml
  label: Renaissance Classes API
  slug: renaissance-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-classes-api-openapi.yml
- filename: renaissance-events-api-openapi.yml
  format: yaml
  label: Renaissance Events API
  slug: renaissance-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-events-api-openapi.yml
- filename: renaissance-health-api-openapi.yml
  format: yaml
  label: Renaissance Health API
  slug: renaissance-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-health-api-openapi.yml
- filename: renaissance-pathway-api-openapi.yml
  format: yaml
  label: Renaissance Pathway API
  slug: renaissance-pathway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-pathway-api-openapi.yml
- filename: renaissance-predictions-api-openapi.yml
  format: yaml
  label: Renaissance Predictions API
  slug: renaissance-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-predictions-api-openapi.yml
- filename: renaissance-reading-level-api-openapi.yml
  format: yaml
  label: Renaissance Reading Level API
  slug: renaissance-reading-level-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-reading-level-api-openapi.yml
- filename: renaissance-skills-api-openapi.yml
  format: yaml
  label: Renaissance Skills API
  slug: renaissance-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-skills-api-openapi.yml
- filename: renaissance-utility-api-openapi.yml
  format: yaml
  label: Renaissance Utility API
  slug: renaissance-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-utility-api-openapi.yml
authorization_urls: []
description: ''
docs: https://auth.renaissance.com/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Renaissance Scopes
name_suffix: OAuth Scopes
note: Renaissance publishes no scope reference page. None of the three OpenAPI contracts declares an oauth2 securityScheme with a flows/scopes block, so nothing could be derived from the specs by derive-oauth-scopes.py (it reported 0 providers with oauth2). What IS published is the authorization server's own scopes_supported list plus one product scope named in prose inside the Lexile API securityScheme description. Both are recorded below with their exact evidence. The full product scope namespace is not public and would require authenticated client registration to enumerate.
overview: 'Renaissance uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Renaissance
provider_slug: renaissance
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: renaissance-scopes
source_filename: renaissance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://auth.renaissance.com/.well-known/openid-configuration\ndocs: https://auth.renaissance.com/.well-known/openid-configuration\nnote: >-\n  Renaissance publishes no scope reference page. None of the three OpenAPI contracts declares an\n  oauth2 securityScheme with a flows/scopes block, so nothing could be derived from the specs by\n  derive-oauth-scopes.py (it reported 0 providers with oauth2). What IS published is the\n  authorization server's own scopes_supported list plus one product scope named in prose inside the\n  Lexile API securityScheme description. Both are recorded below with their exact evidence. The full\n  product scope namespace is not public and would require authenticated client registration to\n  enumerate.\nauthorization_server: https://auth.renaissance.com\nscope_count: 4\nscopes:\n  - name: openid\n    description: Standard OpenID Connect scope, advertised in the authorization server discovery document.\n\
  \    source: https://auth.renaissance.com/.well-known/openid-configuration\n  - name: offline\n    description: Advertised in the authorization server discovery document.\n    source: https://auth.renaissance.com/.well-known/openid-configuration\n  - name: offline_access\n    description: Refresh-token scope, advertised in the authorization server discovery document.\n    source: https://auth.renaissance.com/.well-known/openid-configuration\n  - name: ren.lexile.read\n    description: >-\n      Read access to Lexile book data by ISBN-13. Enforced by the API Gateway in front of\n      api.proxile.renaissance.com; the token audience must match the API URL.\n    api: Lexile API\n    source: openapi/renaissance-lexile-api-openapi.yml\ngaps:\n  - The `ren.` prefix implies a product scope namespace; only ren.lexile.read is publicly named.\n  - The Student Proficiency Service and Student Pathway Event Proxy declare a bare HTTP bearer scheme\n    and name no scope at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/scopes/renaissance-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- EdTech
- K-12
- Assessment
- Learning Analytics
- Student Data
- OneRoster
- LTI
- Ed-Fi
- Rostering
- Interoperability
- Machine Learning
token_urls: []
---
