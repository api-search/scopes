---
api_specs:
- filename: flock-safety-openapi-original.yml
  format: yaml
  label: Flock Safety API Platform (v3)
  slug: flock-safety-api-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-openapi-original.yml
authorization_urls: []
description: ''
docs: https://docs.flocksafety.com/developer-hub/docs/client-credentials
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Flock Safety Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Flock Safety publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flock Safety API on a user''s behalf.


  Tokens are issued from https://api.flocksafety.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flock Safety
provider_slug: flock-safety
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.flocksafety.com/oauth/token
  name: oauth2Auth
  source: openapi/flock-safety-openapi-original.yml
- description: OAuth 2 with the client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.flocksafety.com/oauth/token
  name: FlockOAuth
  source: openapi/flock-safety-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.flocksafety.com/oauth/token
  name: oauth2
  source: openapi/flock-safety-openapi-original.yml
scope_count: 5
scope_names:
- custom-hotlists:read
- custom-hotlists:write
- custom-holists:read
- custom-holists:write
- plate-reads:lookup
scopes:
- description: Read access to custom hotlists (canonical spelling used in operation security requirements).
  flows:
  - clientCredentials
  scope: custom-hotlists:read
- description: Write access to custom hotlists (canonical spelling used in operation security requirements).
  flows:
  - clientCredentials
  scope: custom-hotlists:write
- description: Read access to custom hotlists (verbatim from oauth2Auth scheme; note the source typo "holists").
  flows:
  - clientCredentials
  scope: custom-holists:read
- description: Write access to custom hotlists (verbatim from oauth2Auth scheme; note the source typo "holists").
  flows:
  - clientCredentials
  scope: custom-holists:write
- description: Access to perform lookups on license plate reads.
  flows:
  - clientCredentials
  scope: plate-reads:lookup
slug: flock-safety-scopes
source_filename: flock-safety-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/flock-safety-openapi-original.yml\ndocs: https://docs.flocksafety.com/developer-hub/docs/client-credentials\nnotes: >-\n  Scopes are declared per OAuth application when Flock registers an integration; they govern what a\n  Flock App can access. The oauth2Auth scheme in the spec spells the hotlist scopes 'custom-holists:*'\n  (a source typo, missing a 't'), while operation security requirements use 'custom-hotlists:*'. Both\n  spellings are preserved below; treat 'custom-hotlists:*' as canonical.\nschemes:\n- name: oauth2Auth\n  source: openapi/flock-safety-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.flocksafety.com/oauth/token\n- name: FlockOAuth\n  source: openapi/flock-safety-openapi-original.yml\n  description: OAuth 2 with the client credentials flow\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.flocksafety.com/oauth/token\n- name: oauth2\n  source:\
  \ openapi/flock-safety-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.flocksafety.com/oauth/token\nscopes:\n- scope: custom-hotlists:read\n  description: Read access to custom hotlists (canonical spelling used in operation security requirements).\n  flows: [clientCredentials]\n  sources: [openapi/flock-safety-openapi-original.yml]\n- scope: custom-hotlists:write\n  description: Write access to custom hotlists (canonical spelling used in operation security requirements).\n  flows: [clientCredentials]\n  sources: [openapi/flock-safety-openapi-original.yml]\n- scope: custom-holists:read\n  description: 'Read access to custom hotlists (verbatim from oauth2Auth scheme; note the source typo \"holists\").'\n  flows: [clientCredentials]\n  sources: [openapi/flock-safety-openapi-original.yml]\n- scope: custom-holists:write\n  description: 'Write access to custom hotlists (verbatim from oauth2Auth scheme; note the source typo \"holists\").'\n  flows: [clientCredentials]\n\
  \  sources: [openapi/flock-safety-openapi-original.yml]\n- scope: plate-reads:lookup\n  description: Access to perform lookups on license plate reads.\n  flows: [clientCredentials]\n  sources: [openapi/flock-safety-openapi-original.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/scopes/flock-safety-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Company
- American Dynamism
- Public Safety
- Law Enforcement
- License Plate Recognition
- LPR
- Physical Security
- Surveillance
- Computer Vision
- Webhooks
- Geolocation
- CAD
token_urls:
- https://api.flocksafety.com/oauth/token
---
