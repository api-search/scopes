---
authorization_urls:
- https://www.linkedin.com/oauth/v2/authorization
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Linkedin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LinkedIn publishes 7 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the LinkedIn API on a user''s behalf.


  Tokens are issued from https://www.linkedin.com/oauth/v2/accessToken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LinkedIn
provider_slug: linkedin
schemes:
- flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2Auth
  source: openapi/linkedin-compliance-events.yml
- flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2Auth
  source: openapi/linkedin-learning-activity-reports.yml
- flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2Auth
  source: openapi/linkedin-marketing-audience-insights.yml
- flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2Auth
  source: openapi/linkedin-marketing-audience.yml
- flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2Auth
  source: openapi/linkedin-marketing-campaigns.yml
- description: OAuth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2Auth
  source: openapi/linkedin-talent-job-posting.yml
- description: OAuth 2.0 authentication for partner applications
  flows:
  - flow: clientCredentials
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2Auth
  source: openapi/linkedin-talent-learning-parent-application.yml
- description: OAuth 2.0 authentication with 3-legged flow
  flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2Auth
  source: openapi/linkedin-talent-recruiter-system-connect.yml
scope_count: 7
scope_names:
- r_ads
- r_compliance
- r_liteprofile
- r_lms_learning
- rw_ads
- w_member_social
- w_organization_social
scopes:
- description: Read advertising data
  flows:
  - authorizationCode
  scope: r_ads
- description: Read compliance data
  flows:
  - authorizationCode
  scope: r_compliance
- description: Read basic profile data
  flows:
  - authorizationCode
  - clientCredentials
  scope: r_liteprofile
- description: Read learning management data
  flows:
  - authorizationCode
  scope: r_lms_learning
- description: Read and write advertising data
  flows:
  - authorizationCode
  scope: rw_ads
- description: Post, comment and like posts
  flows:
  - clientCredentials
  scope: w_member_social
- description: Write organization social content
  flows:
  - clientCredentials
  scope: w_organization_social
slug: linkedin-scopes
source_filename: linkedin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/linkedin-compliance-events.yml, openapi/linkedin-learning-activity-reports.yml,\n  openapi/linkedin-marketing-audience-insights.yml, openapi/linkedin-marketing-audience.yml,\n  openapi/linkedin-marketing-campaigns.yml, openapi/linkedin-talent-job-posting.yml, openapi/linkedin-talent-learning-parent-application.yml,\n  openapi/linkedin-talent-recruiter-system-connect.yml\nschemes:\n- name: OAuth2Auth\n  source: openapi/linkedin-compliance-events.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n- name: OAuth2Auth\n  source: openapi/linkedin-learning-activity-reports.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n- name: OAuth2Auth\n  source: openapi/linkedin-marketing-audience-insights.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n- name: OAuth2Auth\n  source: openapi/linkedin-marketing-audience.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n- name: OAuth2Auth\n  source: openapi/linkedin-marketing-campaigns.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n- name: OAuth2Auth\n  source: openapi/linkedin-talent-job-posting.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n  description: OAuth 2.0 authentication\n- name: OAuth2Auth\n  source: openapi/linkedin-talent-learning-parent-application.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://www.linkedin.com/oauth/v2/accessToken\n  description: OAuth 2.0 authentication for partner applications\n- name: OAuth2Auth\n  source: openapi/linkedin-talent-recruiter-system-connect.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n  description: OAuth 2.0 authentication with 3-legged flow\nscopes:\n- scope: r_ads\n  description: Read advertising data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linkedin-marketing-audience-insights.yml\n  - openapi/linkedin-marketing-campaigns.yml\n- scope: r_compliance\n  description: Read compliance data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linkedin-compliance-events.yml\n- scope: r_liteprofile\n  description: Read basic profile data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/linkedin-talent-learning-parent-application.yml\n  - openapi/linkedin-talent-recruiter-system-connect.yml\n\
  - scope: r_lms_learning\n  description: Read learning management data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linkedin-learning-activity-reports.yml\n- scope: rw_ads\n  description: Read and write advertising data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linkedin-marketing-audience.yml\n  - openapi/linkedin-marketing-campaigns.yml\n- scope: w_member_social\n  description: Post, comment and like posts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/linkedin-talent-learning-parent-application.yml\n- scope: w_organization_social\n  description: Write organization social content\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/linkedin-talent-job-posting.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/scopes/linkedin-scopes.yml
summary_line: 7 scopes · authorizationCode/clientCredentials
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
- Fortune 1000
token_urls:
- https://www.linkedin.com/oauth/v2/accessToken
---
