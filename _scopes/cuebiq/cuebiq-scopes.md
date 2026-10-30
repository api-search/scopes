---
api_specs:
- filename: cuebiq-conversion-feed-v1-api-openapi.yml
  format: yaml
  label: Cuebiq Conversion Feed V1 API
  slug: cuebiq-conversion-feed-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-conversion-feed-v1-api-openapi.yml
- filename: cuebiq-geoset-api-openapi.yml
  format: yaml
  label: Cuebiq Geoset API
  slug: cuebiq-geoset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-geoset-api-openapi.yml
- filename: cuebiq-kpis-v2-campaign-reports-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Campaign Reports API
  slug: cuebiq-kpis-v2-campaign-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-campaign-reports-api-openapi.yml
- filename: cuebiq-kpis-v2-campaigns-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Campaigns API
  slug: cuebiq-kpis-v2-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-campaigns-api-openapi.yml
- filename: cuebiq-kpis-v2-customer-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Customer API
  slug: cuebiq-kpis-v2-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-customer-api-openapi.yml
- filename: cuebiq-kpis-v2-shared-campaign-reports-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Shared Campaign Reports API
  slug: cuebiq-kpis-v2-shared-campaign-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-shared-campaign-reports-api-openapi.yml
- filename: cuebiq-kpis-v2-shared-campaigns-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Shared Campaigns API
  slug: cuebiq-kpis-v2-shared-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-shared-campaigns-api-openapi.yml
- filename: cuebiq-kpis-v2-shared-reports-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Shared Reports API
  slug: cuebiq-kpis-v2-shared-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-shared-reports-api-openapi.yml
- filename: cuebiq-measurement-v2-api-openapi.yml
  format: yaml
  label: Cuebiq Measurement V2 API
  slug: cuebiq-measurement-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-measurement-v2-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Cuebiq Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cuebiq uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.cuebiq.com/auth/realms/Customers/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cuebiq
provider_slug: cuebiq
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.cuebiq.com/auth/realms/Customers/protocol/openid-connect/token
  name: cuebiq_auth
  source: openapi/cuebiq-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: cuebiq-scopes
source_filename: cuebiq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: derived\nsource: openapi/cuebiq-openapi.json\nschemes:\n- name: cuebiq_auth\n  source: openapi/cuebiq-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.cuebiq.com/auth/realms/Customers/protocol/openid-connect/token\nscopes:\n  - openid\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/scopes/cuebiq-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Location Intelligence
- Marketing
- Data Analytics
- Footfall-Measurement
token_bound: false
token_urls:
- https://auth.cuebiq.com/auth/realms/Customers/protocol/openid-connect/token
---
