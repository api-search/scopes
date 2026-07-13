---
api_specs:
- filename: linkedin-ads-openapi.yml
  format: yaml
  label: LinkedIn Marketing API
  slug: marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-openapi.yml
authorization_urls:
- https://www.linkedin.com/oauth/v2/authorization
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Linkedin Ads Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LinkedIn Marketing API publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the LinkedIn Marketing API API on a user''s behalf.


  Tokens are issued from https://www.linkedin.com/oauth/v2/accessToken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LinkedIn Marketing API
provider_slug: linkedin-ads
schemes:
- description: OAuth 2.0 three-legged (authorization code) flow.
  flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2
  source: openapi/linkedin-ads-openapi.yml
scope_count: 4
scope_names:
- r_ads
- r_ads_reporting
- r_basicprofile
- rw_ads
scopes:
- description: Read ads accounts, campaigns, and creatives.
  flows:
  - authorizationCode
  scope: r_ads
- description: Read ad campaign reporting data.
  flows:
  - authorizationCode
  scope: r_ads_reporting
- description: Read basic profile.
  flows:
  - authorizationCode
  scope: r_basicprofile
- description: Read and write ads accounts, campaigns, and creatives.
  flows:
  - authorizationCode
  scope: rw_ads
slug: linkedin-ads-scopes
source_filename: linkedin-ads-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/linkedin-ads-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/linkedin-ads-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n  description: OAuth 2.0 three-legged (authorization code) flow.\nscopes:\n- scope: r_ads\n  description: Read ads accounts, campaigns, and creatives.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linkedin-ads-openapi.yml\n- scope: r_ads_reporting\n  description: Read ad campaign reporting data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linkedin-ads-openapi.yml\n- scope: r_basicprofile\n  description: Read basic profile.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linkedin-ads-openapi.yml\n- scope: rw_ads\n  description: Read and write ads accounts, campaigns, and creatives.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/linkedin-ads-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/scopes/linkedin-ads-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Advertising
- Marketing
- LinkedIn
- Lead Generation
- Audience Targeting
- Conversions API
- Social Marketing
token_urls:
- https://www.linkedin.com/oauth/v2/accessToken
---
