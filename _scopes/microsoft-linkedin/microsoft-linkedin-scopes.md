---
api_specs:
- filename: microsoft-linkedin-openapi.yml
  format: yaml
  label: LinkedIn Marketing API
  slug: marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-openapi.yml
authorization_urls:
- https://www.linkedin.com/oauth/v2/authorization
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Linkedin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft LinkedIn publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft LinkedIn API on a user''s behalf.


  Tokens are issued from https://www.linkedin.com/oauth/v2/accessToken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft LinkedIn
provider_slug: microsoft-linkedin
schemes:
- description: LinkedIn OAuth 2.0 (3-legged or 2-legged)
  flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: oauth2
  source: openapi/microsoft-linkedin-openapi.yml
scope_count: 5
scope_names:
- r_ads
- r_ads_reporting
- r_organization_social
- rw_ads
- w_organization_social
scopes:
- description: Read LinkedIn ads data
  flows:
  - authorizationCode
  scope: r_ads
- description: Read LinkedIn ads reporting
  flows:
  - authorizationCode
  scope: r_ads_reporting
- description: Read organization social actions
  flows:
  - authorizationCode
  scope: r_organization_social
- description: Read and write LinkedIn ads data
  flows:
  - authorizationCode
  scope: rw_ads
- description: Write organization social actions
  flows:
  - authorizationCode
  scope: w_organization_social
slug: microsoft-linkedin-scopes
source_filename: microsoft-linkedin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-linkedin-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-linkedin-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n  description: LinkedIn OAuth 2.0 (3-legged or 2-legged)\nscopes:\n- scope: r_ads\n  description: Read LinkedIn ads data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-linkedin-openapi.yml\n- scope: r_ads_reporting\n  description: Read LinkedIn ads reporting\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-linkedin-openapi.yml\n- scope: r_organization_social\n  description: Read organization social actions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-linkedin-openapi.yml\n- scope: rw_ads\n  description: Read and write LinkedIn ads data\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/microsoft-linkedin-openapi.yml\n- scope: w_organization_social\n  description: Write organization social actions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-linkedin-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/scopes/microsoft-linkedin-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Marketing
- Microsoft
- Professional Networking
- Recruiting
- Social Network
token_urls:
- https://www.linkedin.com/oauth/v2/accessToken
---
