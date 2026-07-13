---
api_specs:
- filename: at-t-developer-hub-network-insights-api.yaml
  format: yaml
  label: AT&T Network Insights API
  slug: att-network-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-network-insights-api.yaml
- filename: at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml
  format: yaml
  label: AT&T Mobility Threat and Anomaly Detection API
  slug: att-mobility-threat-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml
- filename: at-t-developer-hub-sim-swap-api.yaml
  format: yaml
  label: AT&T SIM Swap API
  slug: att-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-sim-swap-api.yaml
- filename: at-t-developer-hub-device-status-api.yaml
  format: yaml
  label: AT&T Device Status API
  slug: att-device-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-device-status-api.yaml
- filename: at-t-developer-hub-quality-on-demand-api.yaml
  format: yaml
  label: AT&T Quality on Demand API
  slug: att-quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-quality-on-demand-api.yaml
- filename: at-t-developer-hub-number-verification-api.yaml
  format: yaml
  label: AT&T Number Verification API
  slug: att-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/openapi/at-t-developer-hub-number-verification-api.yaml
authorization_urls: []
description: ''
docs: https://developer.att.com/oauth-2/docs
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: At T Developer Hub Scopes
name_suffix: OAuth Scopes
note: AT&T publishes no OAuth scopes for the Developer Hub's invite-only CAMARA network APIs, which use a client_credentials flow (https://devex-web.att.com/developer-hub/docs/network-api-accelerator-program); the OAuth 2.0 scope documentation at https://developer.att.com/oauth-2/docs covers only legacy APIs (SMS, MMS, ADS, Speech).
overview: 'AT&T Developer Hub uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.att.com/oauth/v4/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schemes:
- description: AT&T OAuth 2.0 for CAMARA network APIs
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  source: openapi/at-t-developer-hub-device-status-api.yaml
- description: AT&T OAuth 2.0 for network security APIs
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  source: openapi/at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml
- description: AT&T OAuth 2.0 for network APIs
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  source: openapi/at-t-developer-hub-network-insights-api.yaml
- description: AT&T OAuth 2.0 for CAMARA network APIs
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  source: openapi/at-t-developer-hub-number-verification-api.yaml
- description: AT&T OAuth 2.0 for CAMARA network APIs
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  source: openapi/at-t-developer-hub-quality-on-demand-api.yaml
- description: AT&T OAuth 2.0 for CAMARA network APIs
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  source: openapi/at-t-developer-hub-sim-swap-api.yaml
scope_count: 0
scope_names: []
scopes: []
slug: at-t-developer-hub-scopes
source_filename: at-t-developer-hub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\ndocs: https://developer.att.com/oauth-2/docs\nnote: AT&T publishes no OAuth scopes for the Developer Hub's invite-only CAMARA network\n  APIs, which use a client_credentials flow (https://devex-web.att.com/developer-hub/docs/network-api-accelerator-program);\n  the OAuth 2.0 scope documentation at https://developer.att.com/oauth-2/docs covers\n  only legacy APIs (SMS, MMS, ADS, Speech).\nsource: openapi/at-t-developer-hub-device-status-api.yaml, openapi/at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml,\n  openapi/at-t-developer-hub-network-insights-api.yaml, openapi/at-t-developer-hub-number-verification-api.yaml,\n  openapi/at-t-developer-hub-quality-on-demand-api.yaml, openapi/at-t-developer-hub-sim-swap-api.yaml\nschemes:\n- name: oauth2\n  source: openapi/at-t-developer-hub-device-status-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.att.com/oauth/v4/token\n  description: AT&T OAuth 2.0 for\
  \ CAMARA network APIs\n- name: oauth2\n  source: openapi/at-t-developer-hub-mobility-threat-anomaly-detection-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.att.com/oauth/v4/token\n  description: AT&T OAuth 2.0 for network security APIs\n- name: oauth2\n  source: openapi/at-t-developer-hub-network-insights-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.att.com/oauth/v4/token\n  description: AT&T OAuth 2.0 for network APIs\n- name: oauth2\n  source: openapi/at-t-developer-hub-number-verification-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.att.com/oauth/v4/token\n  description: AT&T OAuth 2.0 for CAMARA network APIs\n- name: oauth2\n  source: openapi/at-t-developer-hub-quality-on-demand-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.att.com/oauth/v4/token\n  description: AT&T OAuth 2.0 for CAMARA network APIs\n- name: oauth2\n  source: openapi/at-t-developer-hub-sim-swap-api.yaml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.att.com/oauth/v4/token\n  description: AT&T OAuth 2.0 for CAMARA network APIs\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-t-developer-hub/refs/heads/main/scopes/at-t-developer-hub-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fortune 100
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
token_urls:
- https://api.att.com/oauth/v4/token
---
