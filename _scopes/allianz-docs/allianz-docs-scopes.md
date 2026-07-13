---
api_specs:
- filename: allianz-api-connect.yaml
  format: yaml
  label: Allianz API Connect
  slug: allianz-api-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/openapi/allianz-api-connect.yaml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Allianz Docs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Allianz publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allianz API on a user''s behalf.


  Tokens are issued from https://api.allianz.com.au/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allianz
provider_slug: allianz-docs
schemes:
- description: OAuth2 client credentials flow for partner API access
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.allianz.com.au/oauth2/token
  name: OAuth2
  source: openapi/allianz-api-connect.yaml
scope_count: 4
scope_names:
- certificates
- lead_referral
- policy_details
- price_estimate
scopes:
- description: Access to certificate retrieval APIs
  flows:
  - clientCredentials
  scope: certificates
- description: Access to lead referral APIs
  flows:
  - clientCredentials
  scope: lead_referral
- description: Access to policy detail APIs
  flows:
  - clientCredentials
  scope: policy_details
- description: Access to price estimation APIs
  flows:
  - clientCredentials
  scope: price_estimate
slug: allianz-docs-scopes
source_filename: allianz-docs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/allianz-api-connect.yaml\nschemes:\n- name: OAuth2\n  source: openapi/allianz-api-connect.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.allianz.com.au/oauth2/token\n  description: OAuth2 client credentials flow for partner API access\nscopes:\n- scope: certificates\n  description: Access to certificate retrieval APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-api-connect.yaml\n- scope: lead_referral\n  description: Access to lead referral APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-api-connect.yaml\n- scope: policy_details\n  description: Access to policy detail APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-api-connect.yaml\n- scope: price_estimate\n  description: Access to price estimation APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-api-connect.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/scopes/allianz-docs-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Financial Services
- Insurance
- Asset Management
token_urls:
- https://api.allianz.com.au/oauth2/token
---
