---
api_specs:
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Clients API
  slug: provet-cloud-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Patients API
  slug: provet-cloud-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Appointments API
  slug: provet-cloud-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Consultations API
  slug: provet-cloud-consultations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Billing & Invoicing API
  slug: provet-cloud-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Items & Reference Data API
  slug: provet-cloud-items-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Webhooks API
  slug: provet-cloud-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
authorization_urls:
- https://provetcloud.com/0/oauth2/authorize/
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Provet Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Provet Cloud publishes 2 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Provet Cloud API on a user''s behalf.


  Tokens are issued from https://provetcloud.com/0/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Provet Cloud
provider_slug: provet-cloud
schemes:
- description: OAuth 2.0. Client Credentials for backend services; Authorization Code with PKCE for user-facing apps. Token endpoint is https://provetcloud.com/<provet_id>/oauth2/token/ with scope "restapi".
  flows:
  - flow: clientCredentials
    tokenUrl: https://provetcloud.com/0/oauth2/token/
  - authorizationUrl: https://provetcloud.com/0/oauth2/authorize/
    flow: authorizationCode
    tokenUrl: https://provetcloud.com/0/oauth2/token/
  name: oauth2
  source: openapi/provet-cloud-openapi.yml
scope_count: 2
scope_names:
- openid
- restapi
scopes:
- description: Obtain additional user details.
  flows:
  - authorizationCode
  scope: openid
- description: Access the Provet Cloud REST API.
  flows:
  - authorizationCode
  - clientCredentials
  scope: restapi
slug: provet-cloud-scopes
source_filename: provet-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/provet-cloud-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/provet-cloud-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://provetcloud.com/0/oauth2/token/\n  - flow: authorizationCode\n    authorizationUrl: https://provetcloud.com/0/oauth2/authorize/\n    tokenUrl: https://provetcloud.com/0/oauth2/token/\n  description: OAuth 2.0. Client Credentials for backend services; Authorization Code with PKCE\n    for user-facing apps. Token endpoint is https://provetcloud.com/<provet_id>/oauth2/token/\n    with scope \"restapi\".\nscopes:\n- scope: openid\n  description: Obtain additional user details.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/provet-cloud-openapi.yml\n- scope: restapi\n  description: Access the Provet Cloud REST API.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/provet-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/scopes/provet-cloud-scopes.yml
summary_line: 2 scopes · clientCredentials/authorizationCode
tags:
- Veterinary
- Practice Management
- PIMS
- Healthcare
- Nordhealth
- Animal Health
- Appointments
- Billing
token_urls:
- https://provetcloud.com/0/oauth2/token/
---
