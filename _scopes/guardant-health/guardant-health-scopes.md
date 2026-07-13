---
api_specs:
- filename: guardant-health-openapi.yml
  format: yaml
  label: Guardant Health EMR Ordering Integration
  slug: guardant-health-emr-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/openapi/guardant-health-openapi.yml
- filename: guardant-health-openapi.yml
  format: yaml
  label: Guardant Health Results Delivery Integration
  slug: guardant-health-results-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/openapi/guardant-health-openapi.yml
authorization_urls: []
description: ''
docs: https://guardanthealth.com/precision-oncology/for-institutional-partners/emr-integration-services/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Guardant Health Scopes
name_suffix: OAuth Scopes
note: Guardant Health does not publish OAuth scopes; access is partner-provisioned during EMR onboarding (Epic Aura, Flatiron OncoEMR) with no public developer authentication documentation (https://guardanthealth.com/precision-oncology/for-institutional-partners/emr-integration-services/).
overview: 'Guardant Health uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://example.invalid/guardant-health/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Guardant Health
provider_slug: guardant-health
schemes:
- description: Placeholder. Partner-provisioned authentication is negotiated during EMR onboarding; no public auth flow is documented.
  flows:
  - flow: clientCredentials
    tokenUrl: https://example.invalid/guardant-health/oauth/token
  name: partnerOAuth2
  source: openapi/guardant-health-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: guardant-health-scopes
source_filename: guardant-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/guardant-health-openapi.yml\ndocs: https://guardanthealth.com/precision-oncology/for-institutional-partners/emr-integration-services/\nnote: Guardant Health does not publish OAuth scopes; access is partner-provisioned\n  during EMR onboarding (Epic Aura, Flatiron OncoEMR) with no public developer\n  authentication documentation (https://guardanthealth.com/precision-oncology/for-institutional-partners/emr-integration-services/).\nschemes:\n- name: partnerOAuth2\n  source: openapi/guardant-health-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.invalid/guardant-health/oauth/token\n  description: Placeholder. Partner-provisioned authentication is negotiated during EMR onboarding;\n    no public auth flow is documented.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/scopes/guardant-health-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Healthcare
- Precision Oncology
- Liquid Biopsy
- Genomics
- EMR Integration
token_urls:
- https://example.invalid/guardant-health/oauth/token
---
