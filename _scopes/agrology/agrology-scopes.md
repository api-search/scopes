---
api_specs:
- filename: agrology-alerts-api-openapi.yml
  format: yaml
  label: Agrology Alerts API
  slug: agrology-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-alerts-api-openapi.yml
- filename: agrology-charts-api-openapi.yml
  format: yaml
  label: Agrology Charts API
  slug: agrology-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-charts-api-openapi.yml
- filename: agrology-dashboards-api-openapi.yml
  format: yaml
  label: Agrology Dashboards API
  slug: agrology-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-dashboards-api-openapi.yml
- filename: agrology-experiments-api-openapi.yml
  format: yaml
  label: Agrology Experiments API
  slug: agrology-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-experiments-api-openapi.yml
- filename: agrology-feedback-api-openapi.yml
  format: yaml
  label: Agrology Feedback API
  slug: agrology-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-feedback-api-openapi.yml
- filename: agrology-files-api-openapi.yml
  format: yaml
  label: Agrology Files API
  slug: agrology-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-files-api-openapi.yml
- filename: agrology-ground-truth-api-openapi.yml
  format: yaml
  label: Agrology Ground Truth API
  slug: agrology-ground-truth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-ground-truth-api-openapi.yml
- filename: agrology-metrics-api-openapi.yml
  format: yaml
  label: Agrology Metrics API
  slug: agrology-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-metrics-api-openapi.yml
- filename: agrology-microclimate-api-openapi.yml
  format: yaml
  label: Agrology Microclimate API
  slug: agrology-microclimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-microclimate-api-openapi.yml
- filename: agrology-reports-api-openapi.yml
  format: yaml
  label: Agrology Reports API
  slug: agrology-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-reports-api-openapi.yml
- filename: agrology-summary-data-api-openapi.yml
  format: yaml
  label: Agrology Summary Data API
  slug: agrology-summary-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-summary-data-api-openapi.yml
- filename: agrology-synthetics-api-openapi.yml
  format: yaml
  label: Agrology Synthetics API
  slug: agrology-synthetics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-synthetics-api-openapi.yml
- filename: agrology-topology-api-openapi.yml
  format: yaml
  label: Agrology Topology API
  slug: agrology-topology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-topology-api-openapi.yml
- filename: agrology-user-api-openapi.yml
  format: yaml
  label: Agrology User API
  slug: agrology-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-user-api-openapi.yml
- filename: agrology-weather-api-openapi.yml
  format: yaml
  label: Agrology Weather API
  slug: agrology-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-weather-api-openapi.yml
authorization_urls: []
description: ''
docs: https://github.com/agrology/public-api-docs/blob/main/README.md#authentication-security
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Agrology Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Agrology uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agrology
provider_slug: agrology
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: agrology-scopes
source_filename: agrology-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_qBmvSfyNK/.well-known/openid-configuration\ndocs: https://github.com/agrology/public-api-docs/blob/main/README.md#authentication-security\nhttp_status: 200\napplies_to: >-\n  IDENTITY-PROVIDER SCOPES ONLY. These are the OIDC scopes the Amazon Cognito user\n  pool behind the Agrology Grower's Portal advertises for issuing an identity. They\n  are NOT API authorization scopes: the Agrology Public API v2 declares a single\n  http/bearer securityScheme with no oauth2 flows and no scope list, and gates access\n  by an entity ACL (GET /access) rather than by scope. Recorded here because they are\n  real, published and anonymously verifiable, and because a client integrating the\n  login flow needs them.\nscope_source: oidc-discovery\nscope_count: 4\nscopes:\n- name: openid\n  description: Required to request an ID token from the Cognito user pool; establishes\n    the OIDC flow.\n\
  \  standard: OpenID Connect Core 1.0\n- name: email\n  description: Releases the email and email_verified claims for the signed-in grower.\n  standard: OpenID Connect Core 1.0\n- name: phone\n  description: Releases the phone_number and phone_number_verified claims.\n  standard: OpenID Connect Core 1.0\n- name: profile\n  description: Releases the default profile claims for the signed-in user.\n  standard: OpenID Connect Core 1.0\nauthorization_endpoint: https://auth.agrology.ag/oauth2/authorize\ntoken_endpoint: https://auth.agrology.ag/oauth2/token\napi_scope_coverage:\n  documented: false\n  note: >-\n    No per-operation scope, permission or role vocabulary is published for the 90\n    Public API operations. Authorization is resolved from the caller's access list.\n    The access-grant endpoint POST /access/manage/{customerID}/{accessUser}/{accessLevel}\n    implies an accessLevel vocabulary; only the value \"admin\" appears in the published\n    example. An agent cannot determine,\
  \ before calling, which operations its credential\n    may invoke — it must call GET /access and read the returned roles.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/scopes/agrology-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Agriculture
- AgTech
- Climate
- Sensors
- IoT
- Weather
- Soil
- Carbon
- Predictive Analytics
- Geospatial
- Time Series
- Machine-Learning
- Viticulture
- Sustainability
- Environmental Monitoring
token_urls: []
---
