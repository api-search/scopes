---
api_specs:
- filename: linkedin-ads-adaccounts-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdAccounts API
  slug: linkedin-ads-adaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adaccounts-api-openapi.yml
- filename: linkedin-ads-adbudgetpricing-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdBudgetPricing API
  slug: linkedin-ads-adbudgetpricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adbudgetpricing-api-openapi.yml
- filename: linkedin-ads-adtargetingentities-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdTargetingEntities API
  slug: linkedin-ads-adtargetingentities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adtargetingentities-api-openapi.yml
- filename: linkedin-ads-adtargetingfacets-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdTargetingFacets API
  slug: linkedin-ads-adtargetingfacets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adtargetingfacets-api-openapi.yml
- filename: linkedin-ads-audiencecounts-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AudienceCounts API
  slug: linkedin-ads-audiencecounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-audiencecounts-api-openapi.yml
authorization_urls:
- https://www.linkedin.com/oauth/v2/authorization
description: ''
docs: https://learn.microsoft.com/en-us/linkedin/marketing/getting-started
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Linkedin Ads Scopes
name_suffix: OAuth Scopes
note: LinkedIn publishes no single canonical scope reference page. Scopes are granted per product and are shown on the Auth tab of your own app in the Developer Portal, so the authoritative list is per-application. The scopes below are only those evidenced either by the repository OpenAPI or by a named LinkedIn documentation page; there are more scopes across Lead Sync, Conversions, Community Management, Events and Company Intelligence that LinkedIn discloses only to approved partners. A member must consent to the whole requested set — individual scopes cannot be selected — and changing an app's scopes forces re-authentication.
overview: 'LinkedIn Marketing API publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the LinkedIn Marketing API API on a user''s behalf.


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
- description: Sign In with LinkedIn using OpenID Connect.
  name: OpenIDConnect
  source: well-known/linkedin-ads-openid-configuration.json
scope_count: 13
scope_names:
- r_ads
- rw_ads
- r_ads_reporting
- r_basicprofile
- rw_organization_admin
- w_organization_social
- w_member_social
- rw_events
- r_events
- r_marketing_leadgen_automation
- openid
- profile
- email
scopes:
- description: Read ad accounts, campaign groups, campaigns and creatives.
  flows:
  - authorizationCode
  scope: r_ads
- description: Read and write ad accounts, campaign groups, campaigns and creatives.
  flows:
  - authorizationCode
  scope: rw_ads
- description: Read ad campaign reporting and analytics data.
  flows:
  - authorizationCode
  scope: r_ads_reporting
- description: Read the authenticated member's basic profile.
  flows:
  - authorizationCode
  scope: r_basicprofile
- description: Manage the organization (Page) an application administers.
  flows:
  - authorizationCode
  scope: rw_organization_admin
- description: Post, comment and react on behalf of an organization Page.
  flows:
  - authorizationCode
  scope: w_organization_social
- description: Post, comment and react on behalf of the authenticated member.
  flows:
  - authorizationCode
  scope: w_member_social
- description: Create and manage LinkedIn Events for the Event Management API.
  flows:
  - authorizationCode
  scope: rw_events
- description: Read LinkedIn Events.
  flows:
  - authorizationCode
  scope: r_events
- description: Read Lead Gen Form responses and manage lead notification subscriptions.
  flows:
  - authorizationCode
  scope: r_marketing_leadgen_automation
- description: OpenID Connect sign-in; returns an RS256 id_token.
  flows:
  - authorizationCode
  scope: openid
- description: OpenID Connect profile claims (name, given_name, family_name, picture, locale).
  flows:
  - authorizationCode
  scope: profile
- description: OpenID Connect email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
slug: linkedin-ads-scopes
source_filename: linkedin-ads-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/linkedin-ads-openapi.yml\ndocs: https://learn.microsoft.com/en-us/linkedin/marketing/getting-started\nnote: >-\n  LinkedIn publishes no single canonical scope reference page. Scopes are granted\n  per product and are shown on the Auth tab of your own app in the Developer\n  Portal, so the authoritative list is per-application. The scopes below are only\n  those evidenced either by the repository OpenAPI or by a named LinkedIn\n  documentation page; there are more scopes across Lead Sync, Conversions,\n  Community Management, Events and Company Intelligence that LinkedIn discloses\n  only to approved partners. A member must consent to the whole requested set —\n  individual scopes cannot be selected — and changing an app's scopes forces\n  re-authentication.\nschemes:\n  - name: OAuth2\n    source: openapi/linkedin-ads-openapi.yml\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n\
  \        tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n    description: OAuth 2.0 three-legged (authorization code) flow.\n  - name: OpenIDConnect\n    source: well-known/linkedin-ads-openid-configuration.json\n    description: Sign In with LinkedIn using OpenID Connect.\nscopes:\n  - scope: r_ads\n    description: Read ad accounts, campaign groups, campaigns and creatives.\n    flows: [authorizationCode]\n    sources: [openapi/linkedin-ads-openapi.yml]\n  - scope: rw_ads\n    description: Read and write ad accounts, campaign groups, campaigns and creatives.\n    flows: [authorizationCode]\n    sources:\n      - openapi/linkedin-ads-openapi.yml\n      - https://learn.microsoft.com/en-us/linkedin/marketing/authentication/lms-generate-an-access-token\n  - scope: r_ads_reporting\n    description: Read ad campaign reporting and analytics data.\n    flows: [authorizationCode]\n    sources: [openapi/linkedin-ads-openapi.yml]\n  - scope: r_basicprofile\n    description: Read the authenticated\
  \ member's basic profile.\n    flows: [authorizationCode]\n    sources:\n      - openapi/linkedin-ads-openapi.yml\n      - https://learn.microsoft.com/en-us/linkedin/marketing/authentication/lms-generate-an-access-token\n  - scope: rw_organization_admin\n    description: Manage the organization (Page) an application administers.\n    flows: [authorizationCode]\n    sources: [https://learn.microsoft.com/en-us/linkedin/marketing/authentication/lms-generate-an-access-token]\n  - scope: w_organization_social\n    description: Post, comment and react on behalf of an organization Page.\n    flows: [authorizationCode]\n    sources: [https://learn.microsoft.com/en-us/linkedin/marketing/authentication/lms-generate-an-access-token]\n  - scope: w_member_social\n    description: Post, comment and react on behalf of the authenticated member.\n    flows: [authorizationCode]\n    sources: [https://learn.microsoft.com/en-us/linkedin/marketing/authentication/lms-generate-an-access-token]\n  - scope: rw_events\n\
  \    description: Create and manage LinkedIn Events for the Event Management API.\n    flows: [authorizationCode]\n    sources: [https://learn.microsoft.com/en-us/linkedin/marketing/integrations/recent-changes]\n  - scope: r_events\n    description: Read LinkedIn Events.\n    flows: [authorizationCode]\n    sources: [https://learn.microsoft.com/en-us/linkedin/marketing/integrations/recent-changes]\n  - scope: r_marketing_leadgen_automation\n    description: Read Lead Gen Form responses and manage lead notification subscriptions.\n    flows: [authorizationCode]\n    sources: [https://learn.microsoft.com/en-us/linkedin/marketing/lead-sync/leadsync]\n  - scope: openid\n    description: OpenID Connect sign-in; returns an RS256 id_token.\n    flows: [authorizationCode]\n    sources: [well-known/linkedin-ads-openid-configuration.json]\n  - scope: profile\n    description: OpenID Connect profile claims (name, given_name, family_name, picture, locale).\n    flows: [authorizationCode]\n    sources:\
  \ [well-known/linkedin-ads-openid-configuration.json]\n  - scope: email\n    description: OpenID Connect email and email_verified claims.\n    flows: [authorizationCode]\n    sources: [well-known/linkedin-ads-openid-configuration.json]\nconsent:\n  granularity: all-or-nothing per authorization request\n  re_auth_on_scope_change: true\n  guidance: Request the least number of scopes your integration needs.\n  docs: https://learn.microsoft.com/en-us/linkedin/shared/authentication/authorization-code-flow\nx-evidence:\n  fetched: '2026-08-13'\n  checks:\n    - url: https://learn.microsoft.com/en-us/linkedin/marketing/authentication/lms-generate-an-access-token\n      http_status: 200\n    - url: https://www.linkedin.com/oauth/.well-known/openid-configuration\n      http_status: 200\n    - url: https://learn.microsoft.com/en-us/linkedin/shared/authentication/permissions\n      http_status: 404\n      note: No canonical permissions/scopes reference page is published at the expected path.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/scopes/linkedin-ads-scopes.yml
summary_line: 13 scopes · authorizationCode
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
