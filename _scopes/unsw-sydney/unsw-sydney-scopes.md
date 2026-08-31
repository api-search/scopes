---
api_specs:
- filename: unsw-sydney-core-api-openapi.yml
  format: yaml
  label: University of New South Wales Core API
  slug: unsw-sydney-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unsw-sydney/refs/heads/main/openapi/unsw-sydney-core-api-openapi.yml
- filename: unsw-sydney-discover-api-openapi.yml
  format: yaml
  label: University of New South Wales Discover API
  slug: unsw-sydney-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unsw-sydney/refs/heads/main/openapi/unsw-sydney-discover-api-openapi.yml
- filename: unsw-sydney-oai-pmh-api-openapi.yml
  format: yaml
  label: University of New South Wales Oai Pmh API
  slug: unsw-sydney-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unsw-sydney/refs/heads/main/openapi/unsw-sydney-oai-pmh-api-openapi.yml
- filename: unsw-sydney-root-api-openapi.yml
  format: yaml
  label: University of New South Wales Root API
  slug: unsw-sydney-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unsw-sydney/refs/heads/main/openapi/unsw-sydney-root-api-openapi.yml
authorization_urls: []
description: UNSW publishes no OAuth scope vocabulary on any surface reachable without credentials. This file records that absence explicitly so it is not mistaken for an unexamined gap.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Unsw Sydney Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of New South Wales uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of New South Wales
provider_slug: unsw-sydney
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: unsw-sydney-scopes
source_filename: unsw-sydney-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\nname: UNSW Sydney — OAuth scopes\naid: unsw-sydney\ngenerated: '2026-08-19'\nmethod: probed\nsource:\n  - https://apideveloper.unsw.edu.au/getting-started\n  - https://unsworks.unsw.edu.au/server/api\n  - https://moodle.telt.unsw.edu.au/mod/lti/certs.php\ndescription: >-\n  UNSW publishes no OAuth scope vocabulary on any surface reachable without credentials. This file\n  records that absence explicitly so it is not mistaken for an unexamined gap.\nscopes: []\nabsence:\n  state: none\n  reason: no_public_scope_vocabulary\n  detail: >-\n    The Enterprise API Gateway uses Azure API Management subscription keys issued after a manual\n    authorisation process, and its API catalogue is not visible before sign-in, so no scope names\n    are publicly readable. The UNSWorks DSpace REST API and OAI-PMH endpoint are anonymous-read\n    and define no scopes. The only OAuth 2.0 surface found is the LTI 1.3 token endpoint on the\n    tenant-operated Moodle host, whose scopes are\
  \ defined by the 1EdTech LTI Advantage\n    specification and by Moodle, not by UNSW.\n  evidence:\n    - url: https://apideveloper.unsw.edu.au/apis\n      status: 404\n    - url: https://apideveloper.unsw.edu.au/getting-started\n      status: 200\n    - url: https://unsworks.unsw.edu.au/server/api\n      status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unsw-sydney/refs/heads/main/scopes/unsw-sydney-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Research
- Australia
- Group of Eight
- Sydney
- Research Repository
- Identity Federation
- Course Catalog
- Library
- Open Repository
token_urls: []
---
