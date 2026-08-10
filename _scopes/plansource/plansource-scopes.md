---
api_specs:
- filename: plansource-aca-api-openapi.yml
  format: yaml
  label: PlanSource ACA API
  slug: plansource-aca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-aca-api-openapi.yml
- filename: plansource-administrators-api-openapi.yml
  format: yaml
  label: PlanSource Administrators API
  slug: plansource-administrators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-administrators-api-openapi.yml
- filename: plansource-all-api-openapi.yml
  format: yaml
  label: PlanSource All API
  slug: plansource-all-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-all-api-openapi.yml
- filename: plansource-collections-api-openapi.yml
  format: yaml
  label: PlanSource Collections API
  slug: plansource-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-collections-api-openapi.yml
- filename: plansource-composites-api-openapi.yml
  format: yaml
  label: PlanSource Composites API
  slug: plansource-composites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-composites-api-openapi.yml
- filename: plansource-coverage-api-openapi.yml
  format: yaml
  label: PlanSource Coverage API
  slug: plansource-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-coverage-api-openapi.yml
- filename: plansource-demographic-api-openapi.yml
  format: yaml
  label: PlanSource Demographic API
  slug: plansource-demographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-demographic-api-openapi.yml
- filename: plansource-eoi-api-openapi.yml
  format: yaml
  label: PlanSource EOI API
  slug: plansource-eoi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-eoi-api-openapi.yml
- filename: plansource-page-content-api-openapi.yml
  format: yaml
  label: PlanSource Page Content API
  slug: plansource-page-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-page-content-api-openapi.yml
- filename: plansource-payroll-api-openapi.yml
  format: yaml
  label: PlanSource Payroll API
  slug: plansource-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-payroll-api-openapi.yml
- filename: plansource-processing-api-openapi.yml
  format: yaml
  label: PlanSource Processing API
  slug: plansource-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-processing-api-openapi.yml
- filename: plansource-resources-api-openapi.yml
  format: yaml
  label: PlanSource Resources API
  slug: plansource-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-resources-api-openapi.yml
- filename: plansource-security-api-openapi.yml
  format: yaml
  label: PlanSource Security API
  slug: plansource-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/openapi/plansource-security-api-openapi.yml
authorization_urls:
- https://api.plansource.com/sso/oauth2/authorize
description: ''
docs: https://developer.plansource.com/v2.0/reference
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Plansource Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PlanSource publishes 8 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the PlanSource API on a user''s behalf.


  Tokens are issued from https://api.plansource.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PlanSource
provider_slug: plansource
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.plansource.com/oauth/v2/token
  name: clientSecretJwt
  source: openapi/plansource-admin-api-openapi-original.json
  surface: Admin API
- flows:
  - authorizationUrl: https://api.plansource.com/sso/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.plansource.com/sso/oauth2/token
  name: plansource-sso-oidc
  source: well-known/plansource-openid-configuration.json
  surface: end-user SSO
scope_count: 8
scope_names:
- admin_api_v2
- openid
- profile
- email
- address
- phone
- admin_access
- subscriber_access
scopes:
- description: Access to all endpoints
  flows:
  - clientCredentials
  scope: admin_api_v2
- description: OpenID Connect authentication
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC profile claims
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC email claim
  flows:
  - authorizationCode
  scope: email
- description: Standard OIDC address claim
  flows:
  - authorizationCode
  scope: address
- description: Standard OIDC phone claim
  flows:
  - authorizationCode
  scope: phone
- description: 'PlanSource-specific: administrator-level portal access'
  flows:
  - authorizationCode
  scope: admin_access
- description: 'PlanSource-specific: employee (subscriber) portal access'
  flows:
  - authorizationCode
  scope: subscriber_access
slug: plansource-scopes
source_filename: plansource-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource:\n- openapi/plansource-admin-api-openapi-original.json\n- https://api.plansource.com/.well-known/openid-configuration\ndocs: https://developer.plansource.com/v2.0/reference\nschemes:\n- name: clientSecretJwt\n  surface: Admin API\n  source: openapi/plansource-admin-api-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.plansource.com/oauth/v2/token\n- name: plansource-sso-oidc\n  surface: end-user SSO\n  source: well-known/plansource-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.plansource.com/sso/oauth2/authorize\n    tokenUrl: https://api.plansource.com/sso/oauth2/token\nscopes:\n- scope: admin_api_v2\n  description: Access to all endpoints\n  flows:\n  - clientCredentials\n  surface: Admin API\n  sources:\n  - openapi/plansource-admin-api-openapi-original.json\n- scope: openid\n  description: OpenID Connect authentication\n  flows:\n\
  \  - authorizationCode\n  surface: SSO\n  sources:\n  - well-known/plansource-openid-configuration.json\n- scope: profile\n  description: Standard OIDC profile claims\n  flows:\n  - authorizationCode\n  surface: SSO\n  sources:\n  - well-known/plansource-openid-configuration.json\n- scope: email\n  description: Standard OIDC email claim\n  flows:\n  - authorizationCode\n  surface: SSO\n  sources:\n  - well-known/plansource-openid-configuration.json\n- scope: address\n  description: Standard OIDC address claim\n  flows:\n  - authorizationCode\n  surface: SSO\n  sources:\n  - well-known/plansource-openid-configuration.json\n- scope: phone\n  description: Standard OIDC phone claim\n  flows:\n  - authorizationCode\n  surface: SSO\n  sources:\n  - well-known/plansource-openid-configuration.json\n- scope: admin_access\n  description: 'PlanSource-specific: administrator-level portal access'\n  flows:\n  - authorizationCode\n  surface: SSO\n  sources:\n  - well-known/plansource-openid-configuration.json\n\
  - scope: subscriber_access\n  description: 'PlanSource-specific: employee (subscriber) portal access'\n  flows:\n  - authorizationCode\n  surface: SSO\n  sources:\n  - well-known/plansource-openid-configuration.json\nanalysis:\n  granularity: none on the Admin API\n  note: The Admin API has exactly ONE scope, `admin_api_v2`, whose own description is \"Access to all endpoints\".\n    A token issued for a partner that only needs to read payroll deductions carries the same authority\n    as one that can terminate every coverage for every employee (PUT /coverage/subscriber/{subscriber_id}/terminate)\n    and disable administrators. There is no read-only scope, no per-domain scope (demographic / payroll\n    / coverage / EOI / administrator) and no way to least-privilege an integration. For an API carrying\n    HIPAA-regulated PHI across 80 operations, this is the single largest authorization gap in the profile.\n  contrast: The SSO surface does distinguish admin_access from subscriber_access,\
  \ so the concept exists\n    in the platform - it just has not been carried into the Admin API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plansource/refs/heads/main/scopes/plansource-scopes.yml
summary_line: 8 scopes · clientCredentials/authorizationCode
tags:
- Employee Benefits
- Benefits Administration
- Insurance
- Human Resources
- Payroll
- Health Insurance
- Enrollment
- HR Technology
- Evidence of Insurability
- ACA Reporting
- Eligibility
- Single Sign-On
token_urls:
- https://api.plansource.com/oauth/v2/token
- https://api.plansource.com/sso/oauth2/token
---
