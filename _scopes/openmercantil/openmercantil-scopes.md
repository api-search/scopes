---
api_specs:
- filename: openmercantil-api-credentials-api-openapi.yml
  format: yaml
  label: OpenMercantil API Credentials API
  slug: openmercantil-api-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-api-credentials-api-openapi.yml
- filename: openmercantil-billing-api-openapi.yml
  format: yaml
  label: OpenMercantil Billing API
  slug: openmercantil-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-billing-api-openapi.yml
- filename: openmercantil-borme-api-openapi.yml
  format: yaml
  label: OpenMercantil BORME API
  slug: openmercantil-borme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-borme-api-openapi.yml
- filename: openmercantil-companies-api-openapi.yml
  format: yaml
  label: OpenMercantil Companies API
  slug: openmercantil-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-companies-api-openapi.yml
- filename: openmercantil-datasets-api-openapi.yml
  format: yaml
  label: OpenMercantil Datasets API
  slug: openmercantil-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-datasets-api-openapi.yml
- filename: openmercantil-graph-api-openapi.yml
  format: yaml
  label: OpenMercantil Graph API
  slug: openmercantil-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-graph-api-openapi.yml
- filename: openmercantil-integrations-api-openapi.yml
  format: yaml
  label: OpenMercantil Integrations API
  slug: openmercantil-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-integrations-api-openapi.yml
- filename: openmercantil-legal-api-openapi.yml
  format: yaml
  label: OpenMercantil Legal API
  slug: openmercantil-legal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-legal-api-openapi.yml
- filename: openmercantil-persons-api-openapi.yml
  format: yaml
  label: OpenMercantil Persons API
  slug: openmercantil-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-persons-api-openapi.yml
- filename: openmercantil-public-procurement-api-openapi.yml
  format: yaml
  label: OpenMercantil Public Procurement API
  slug: openmercantil-public-procurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-public-procurement-api-openapi.yml
- filename: openmercantil-risk-signals-api-openapi.yml
  format: yaml
  label: OpenMercantil Risk Signals API
  slug: openmercantil-risk-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-risk-signals-api-openapi.yml
- filename: openmercantil-search-api-openapi.yml
  format: yaml
  label: OpenMercantil Search API
  slug: openmercantil-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-search-api-openapi.yml
- filename: openmercantil-sectors-api-openapi.yml
  format: yaml
  label: OpenMercantil Sectors API
  slug: openmercantil-sectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-sectors-api-openapi.yml
- filename: openmercantil-sources-api-openapi.yml
  format: yaml
  label: OpenMercantil Sources API
  slug: openmercantil-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-sources-api-openapi.yml
- filename: openmercantil-support-api-openapi.yml
  format: yaml
  label: OpenMercantil Support API
  slug: openmercantil-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-support-api-openapi.yml
- filename: openmercantil-system-api-openapi.yml
  format: yaml
  label: OpenMercantil System API
  slug: openmercantil-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-system-api-openapi.yml
- filename: openmercantil-user-api-openapi.yml
  format: yaml
  label: OpenMercantil User API
  slug: openmercantil-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-user-api-openapi.yml
- filename: openmercantil-webhooks-api-openapi.yml
  format: yaml
  label: OpenMercantil Webhooks API
  slug: openmercantil-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/openapi/openmercantil-webhooks-api-openapi.yml
authorization_urls: []
description: 'OpenMercantil publishes a real, named authorization scope registry — but it is NOT OAuth 2.0. Scopes attach to opaque `omk_*` API credentials issued from the account panel and presented as `X-API-Key` (or `Authorization: Bearer`). The registry is declared machine-readably in the OpenAPI document under `components.x-api-credential-scopes`, and 43 of the 139 operations carry an `x-api-credential-scope` naming the scope that selects the caller''s account quota for that route. There is no authorization server, no consent screen and no token exchange — a scope selects quota and read plane, it does not grant access a caller lacked, because the public read plane is anonymous by default.'
docs: https://openmercantil.es/api/documentacion
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Openmercantil Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OpenMercantil uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OpenMercantil
provider_slug: openmercantil
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: openmercantil-scopes
source_filename: openmercantil-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  openapi/_original/openmercantil-openapi-1.9.3.json\n  (components.x-api-credential-scopes and per-operation\n  x-api-credential-scope) and https://openmercantil.es/api/documentacion\ndocs: https://openmercantil.es/api/documentacion\nprovider: OpenMercantil\nproviderId: openmercantil\nmodel: api-credential-scopes\noauth2: false\ndescription: >-\n  OpenMercantil publishes a real, named authorization scope registry — but it\n  is NOT OAuth 2.0. Scopes attach to opaque `omk_*` API credentials issued from\n  the account panel and presented as `X-API-Key` (or `Authorization: Bearer`).\n  The registry is declared machine-readably in the OpenAPI document under\n  `components.x-api-credential-scopes`, and 43 of the 139 operations carry an\n  `x-api-credential-scope` naming the scope that selects the caller's account\n  quota for that route. There is no authorization server, no consent screen and\n  no token exchange — a scope\
  \ selects quota and read plane, it does not grant\n  access a caller lacked, because the public read plane is anonymous by\n  default.\nimportant_semantics: >-\n  A scope on this API is a QUOTA and PLANE selector, not an access grant.\n  Anonymous access to the public read plane remains valid without any\n  credential; presenting a credential whose scope matches the operation (or the\n  umbrella `public:read`) moves the request from the per-IP anonymous quota to\n  the credential's account quota. Account-plane operations are NOT reachable\n  with an API credential at all — they require the `ob_sess` session cookie\n  plus an `X-CSRF-Token` header.\nscope_count: 6\nscopes:\n  - name: public:read\n    description: Umbrella scope accepted by every public read route except bulk exports.\n    umbrella: true\n    operation_count: null\n    note: >-\n      Accepted in place of any specific read scope. Bulk export routes are\n      deliberately outside it.\n  - name: companies:read\n    description:\
  \ Companies, BORME, CNAE sectors and public aggregates.\n    operation_count: 28\n    operations:\n      - compareCompanies\n      - getCcaaStatsJson\n      - getCnaeByCode\n      - getCnaeTree\n      - getCompanyBySlug\n      - getCompanyBySlugActivity\n      - getCompanyBySlugBde\n      - getCompanyBySlugCnmv\n      - getCompanyBySlugContracts\n      - getCompanyBySlugEvents\n      - getCompanyBySlugGrants\n      - getCompanyBySlugOfficers\n      - getCompanyBySlugRelationships\n      - getCompanyBySlugSimilar\n      - getCompanyBySlugSources\n      - getCompanyBySlugTed\n      - getCompanyBySlugTimeline\n      - getCompanyBySlugWikidata\n      - getDailyByDate\n      - getEmpresaBySlugFacts\n      - getGrafoBySlug\n      - getHealth\n      - getSearch\n      - getSectorByCnaeCompanies\n      - getSectorByCnaeRatios\n      - getSectoresStatsJson\n      - getStats\n      - listPublicCompanyDownloads\n  - name: people:read\n    description: Documentary mentions of natural persons.\n  \
  \  operation_count: 3\n    operations:\n      - getGrafoPersonaBySlug\n      - getPersonSearch\n      - getPersonaBySlug\n    note: >-\n      The narrowest and most sensitive plane. Responses are doubly redacted —\n      no DNI/NIE, no personal contact data — and natural persons appear only as\n      documentary mentions of published BORME acts, never as profiles.\n  - name: tenders:read\n    description: Sanitized public procurement projections.\n    operation_count: 4\n    operations:\n      - getTender\n      - getTenderStats\n      - listTenderSuppliers\n      - searchTenders\n  - name: legal:read\n    description: BOE mercantile-law corpus.\n    operation_count: 5\n    operations:\n      - getLegalActMap\n      - getLegalActMapByActo\n      - getLegalArticleByNormByN\n      - getLegalNormBySlug\n      - getLegalNorms\n  - name: integrations:read\n    description: Public integration capability catalog.\n    operation_count: 3\n    operations:\n      - getIntegration\n      - getSourcesFreshness\n\
  \      - listIntegrations\ncredential_lifecycle:\n  issuer: account panel (/mi-cuenta)\n  prefix: omk_\n  opaque: true\n  jwt: false\n  management_operations:\n    - listUserApiCredentials\n    - createUserApiCredential\n    - rotateUserApiCredential\n    - revokeUserApiCredential\n  secret_visibility: >-\n    The credential secret is returned once, in the original mutation response,\n    and is replayable only through an identical `Idempotency-Key` request\n    inside a 24-hour window. It is never returned by list or get.\n  rotation_supported: true\n  revocation_supported: true\n  transport_rules:\n    - 'Header only: X-API-Key, or Authorization: Bearer.'\n    - Never permitted in a query string (stated explicitly in the scheme description).\nunscoped_operations:\n  count: 96\n  note: >-\n    The remaining operations carry no x-api-credential-scope because they are\n    either account-plane (session cookie + CSRF, 65 User operations plus\n    billing, support and webhooks) or provider-callback\
  \ routes. Absence of a\n    scope on those is correct, not a gap.\nsee_also:\n  authentication: authentication/openmercantil-authentication.yml\n  conventions: conventions/openmercantil-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmercantil/refs/heads/main/scopes/openmercantil-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- BDNS
- BORME
- Business Registry
- CIF
- CNAE
- CNMV
- CSV
- Company Data
- Company Search
- Corporate Registry
- DCAT-AP
- Daily Summary
- Geocoding
- JSON
- Legal Data
- Mercantile Law
- OEPM
- Open Data
- Open Government Data
- OpenAPI
- OpenSanctions
- PLACSP
- Public Procurement
- Public Records
- Public-Interest Data
- REST API
- Registry Timeline
- Risk Signals
- Sanctions
- Spain
- Spanish Companies
- Spanish Open Data
- Tenders
- Trust Score
- Webhook
token_urls: []
---
