---
api_specs:
- filename: ki-insurance-administration-api-openapi.yml
  format: yaml
  label: Ki Insurance Administration API
  slug: ki-insurance-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-administration-api-openapi.yml
- filename: ki-insurance-broking-houses-api-openapi.yml
  format: yaml
  label: Ki Insurance Broking Houses API
  slug: ki-insurance-broking-houses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-broking-houses-api-openapi.yml
- filename: ki-insurance-classes-of-business-api-openapi.yml
  format: yaml
  label: Ki Insurance Classes of Business API
  slug: ki-insurance-classes-of-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-classes-of-business-api-openapi.yml
- filename: ki-insurance-configuration-api-openapi.yml
  format: yaml
  label: Ki Insurance Configuration API
  slug: ki-insurance-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-configuration-api-openapi.yml
- filename: ki-insurance-dashboard-api-openapi.yml
  format: yaml
  label: Ki Insurance Dashboard API
  slug: ki-insurance-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-dashboard-api-openapi.yml
- filename: ki-insurance-facilities-api-openapi.yml
  format: yaml
  label: Ki Insurance Facilities API
  slug: ki-insurance-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-facilities-api-openapi.yml
- filename: ki-insurance-indications-api-openapi.yml
  format: yaml
  label: Ki Insurance Indications API
  slug: ki-insurance-indications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-indications-api-openapi.yml
- filename: ki-insurance-leads-api-openapi.yml
  format: yaml
  label: Ki Insurance Leads API
  slug: ki-insurance-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-leads-api-openapi.yml
- filename: ki-insurance-market-leaders-api-openapi.yml
  format: yaml
  label: Ki Insurance Market Leaders API
  slug: ki-insurance-market-leaders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-market-leaders-api-openapi.yml
- filename: ki-insurance-master-data-api-openapi.yml
  format: yaml
  label: Ki Insurance Master Data API
  slug: ki-insurance-master-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-master-data-api-openapi.yml
- filename: ki-insurance-pipeline-api-openapi.yml
  format: yaml
  label: Ki Insurance Pipeline API
  slug: ki-insurance-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-pipeline-api-openapi.yml
- filename: ki-insurance-quotes-api-openapi.yml
  format: yaml
  label: Ki Insurance Quotes API
  slug: ki-insurance-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-quotes-api-openapi.yml
- filename: ki-insurance-risk-codes-api-openapi.yml
  format: yaml
  label: Ki Insurance Risk Codes API
  slug: ki-insurance-risk-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-risk-codes-api-openapi.yml
- filename: ki-insurance-schedule-of-values-api-openapi.yml
  format: yaml
  label: Ki Insurance Schedule of Values API
  slug: ki-insurance-schedule-of-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-schedule-of-values-api-openapi.yml
- filename: ki-insurance-slip-extraction-api-openapi.yml
  format: yaml
  label: Ki Insurance Slip Extraction API
  slug: ki-insurance-slip-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-slip-extraction-api-openapi.yml
- filename: ki-insurance-support-api-openapi.yml
  format: yaml
  label: Ki Insurance Support API
  slug: ki-insurance-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-support-api-openapi.yml
- filename: ki-insurance-telemetry-api-openapi.yml
  format: yaml
  label: Ki Insurance Telemetry API
  slug: ki-insurance-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-telemetry-api-openapi.yml
- filename: ki-insurance-users-api-openapi.yml
  format: yaml
  label: Ki Insurance Users API
  slug: ki-insurance-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/openapi/ki-insurance-users-api-openapi.yml
authorization_urls:
- https://login.ki-insurance.com/authorize
description: ''
docs: https://login.ki-insurance.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Ki Insurance Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ki Insurance publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ki Insurance API on a user''s behalf.


  Tokens are issued from https://login.ki-insurance.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ki Insurance
provider_slug: ki-insurance
schemes:
- audience: https://api.ki.com
  flows:
  - authorizationUrl: https://login.ki-insurance.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.ki-insurance.com/oauth/token
  name: auth0OAuth2
  source: https://login.ki-insurance.com/.well-known/openid-configuration
scope_count: 14
scope_names:
- openid
- profile
- email
- offline_access
- address
- phone
- name
- given_name
- family_name
- nickname
- picture
- email_verified
- created_at
- identities
scopes:
- description: Standard OIDC scope — request an ID token for the authenticated broker user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC scope — name, nickname and picture claims.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC scope — email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Standard OAuth scope — issue a refresh token for the broker session.
  flows:
  - authorizationCode
  scope: offline_access
- description: Standard OIDC scope — address claim.
  flows:
  - authorizationCode
  scope: address
- description: Standard OIDC scope — phone_number claim.
  flows:
  - authorizationCode
  scope: phone
- description: Auth0 profile sub-scope — name claim.
  flows:
  - authorizationCode
  scope: name
- description: Auth0 profile sub-scope — given_name claim.
  flows:
  - authorizationCode
  scope: given_name
- description: Auth0 profile sub-scope — family_name claim.
  flows:
  - authorizationCode
  scope: family_name
- description: Auth0 profile sub-scope — nickname claim.
  flows:
  - authorizationCode
  scope: nickname
- description: Auth0 profile sub-scope — picture claim.
  flows:
  - authorizationCode
  scope: picture
- description: Auth0 profile sub-scope — email_verified claim.
  flows:
  - authorizationCode
  scope: email_verified
- description: Auth0 profile sub-scope — created_at claim.
  flows:
  - authorizationCode
  scope: created_at
- description: Auth0 profile sub-scope — linked identities claim.
  flows:
  - authorizationCode
  scope: identities
slug: ki-insurance-scopes
source_filename: ki-insurance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://login.ki-insurance.com/.well-known/openid-configuration\ndocs: https://login.ki-insurance.com/.well-known/openid-configuration\nsummary: >-\n  Ki's authorization server publishes only the standard OpenID Connect scopes.\n  No Ki business scope (quote:read, quote:write, pipeline:read or similar) is\n  advertised anywhere on the public surface, and none appears in the platform\n  client bundle — the broker app requests a token for audience\n  https://api.ki.com and authorises every /api call with that single bearer\n  token. Any partner-specific scope model, if one exists, is private.\nschemes:\n- name: auth0OAuth2\n  source: https://login.ki-insurance.com/.well-known/openid-configuration\n  audience: https://api.ki.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.ki-insurance.com/authorize\n    tokenUrl: https://login.ki-insurance.com/oauth/token\nscopes:\n- scope: openid\n  description:\
  \ Standard OIDC scope — request an ID token for the authenticated broker user.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: profile\n  description: Standard OIDC scope — name, nickname and picture claims.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: email\n  description: Standard OIDC scope — email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: offline_access\n  description: Standard OAuth scope — issue a refresh token for the broker session.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: address\n  description: Standard OIDC scope — address claim.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: phone\n  description:\
  \ Standard OIDC scope — phone_number claim.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: name\n  description: Auth0 profile sub-scope — name claim.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: given_name\n  description: Auth0 profile sub-scope — given_name claim.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: family_name\n  description: Auth0 profile sub-scope — family_name claim.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: nickname\n  description: Auth0 profile sub-scope — nickname claim.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: picture\n  description: Auth0 profile sub-scope — picture claim.\n  flows: [authorizationCode]\n\
  \  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: email_verified\n  description: Auth0 profile sub-scope — email_verified claim.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: created_at\n  description: Auth0 profile sub-scope — created_at claim.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\n- scope: identities\n  description: Auth0 profile sub-scope — linked identities claim.\n  flows: [authorizationCode]\n  sources: [https://login.ki-insurance.com/.well-known/openid-configuration]\nauthorization_model:\n  note: >-\n    Authorisation inside the Ki platform is role- and entitlement-based rather\n    than scope-based. The client bundle carries an admin surface\n    (/api/system/admin/*, /api/maxlinesizes, bulk user management) and a\n    per-user class-of-business entitlement (/api/user/{userId}/selected-cobs),\n    which\
  \ implies server-side role checks — the 403 handling in the client\n    confirms it. None of that is published as OAuth scopes.\ngaps:\n- No Ki-specific API scopes are published.\n- No scope-to-operation mapping exists; do not infer one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ki-insurance/refs/heads/main/scopes/ki-insurance-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Insurance
- United Kingdom
- Lloyd's of London
- Specialty Insurance
- Property and Casualty
- Underwriting
- Insurtech
- Brokers
- Algorithmic Underwriting
- Reinsurance
token_urls:
- https://login.ki-insurance.com/oauth/token
---
