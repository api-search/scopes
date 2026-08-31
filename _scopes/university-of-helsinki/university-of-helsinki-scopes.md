---
api_specs:
- filename: university-of-helsinki-hy-organisation-api-openapi.yml
  format: yaml
  label: HY Organisation API
  slug: hy-organisation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-hy-organisation-api-openapi.yml
- filename: university-of-helsinki-contact-search-api-openapi.yml
  format: yaml
  label: Contact Search API
  slug: contact-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-contact-search-api-openapi.yml
- filename: university-of-helsinki-course-pages-cms-openapi.yml
  format: yaml
  label: Course pages CMS
  slug: course-pages-cms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-course-pages-cms-openapi.yml
- filename: university-of-helsinki-helsinki-fi-content-openapi.yml
  format: yaml
  label: Helsinki.fi content
  slug: helsinki-fi-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-helsinki-fi-content-openapi.yml
- filename: university-of-helsinki-hy-building-api-openapi.yml
  format: yaml
  label: HY Building API
  slug: hy-building
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-hy-building-api-openapi.yml
- filename: university-of-helsinki-serviceapi-openapi.yml
  format: yaml
  label: ServiceAPI
  slug: serviceapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-serviceapi-openapi.yml
- filename: university-of-helsinki-employeeinformationapi-openapi.yml
  format: yaml
  label: EmployeeInformationAPI
  slug: employeeinformation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-employeeinformationapi-openapi.yml
- filename: university-of-helsinki-persongroup-openapi.yml
  format: yaml
  label: PersonGroup
  slug: persongroup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-persongroup-openapi.yml
- filename: university-of-helsinki-general-efecte-api-openapi.yml
  format: yaml
  label: General Efecte API
  slug: general-efecte
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-general-efecte-api-openapi.yml
- filename: university-of-helsinki-network-registry-api-openapi.yml
  format: yaml
  label: Network registry API
  slug: network-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-network-registry-api-openapi.yml
- filename: university-of-helsinki-sovellussalkku-api-openapi.yml
  format: yaml
  label: Sovellussalkku API
  slug: sovellussalkku
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-sovellussalkku-api-openapi.yml
- filename: university-of-helsinki-dawa-sync-api-openapi.yml
  format: yaml
  label: Dawa Sync API
  slug: dawa-sync
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-dawa-sync-api-openapi.yml
- filename: university-of-helsinki-finbif-laji-openapi.yml
  format: yaml
  label: FinBIF Laji API (Finnish Biodiversity Information Facility)
  slug: finbif-laji
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-finbif-laji-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Helsinki Scopes
name_suffix: OAuth Scopes
note: NO SCOPE STRINGS ARE PUBLISHED. This artifact records a measured absence, not an inventory. All thirteen institution-operated OpenAPI documents harvested from the University of Helsinki API portal and from api.laji.fi were parsed for `components.securitySchemes.*.flows.*.scopes` and the result was empty across every one of them. The single `oauth2` securityScheme in the estate (Course pages CMS) declares no flows at all, so there is nothing for a scope to hang from. Nothing here is inferred; no scope has been invented to fill the slot.
overview: 'University of Helsinki uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Helsinki
provider_slug: university-of-helsinki
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-helsinki-scopes
source_filename: university-of-helsinki-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://api.helsinki.fi/portal/environments/DEFAULT/configuration\nx-operator: institution\nnote: >-\n  NO SCOPE STRINGS ARE PUBLISHED. This artifact records a measured absence, not an inventory.\n  All thirteen institution-operated OpenAPI documents harvested from the University of Helsinki\n  API portal and from api.laji.fi were parsed for `components.securitySchemes.*.flows.*.scopes`\n  and the result was empty across every one of them. The single `oauth2` securityScheme in the\n  estate (Course pages CMS) declares no flows at all, so there is nothing for a scope to hang\n  from. Nothing here is inferred; no scope has been invented to fill the slot.\nauthorization_model:\n  kind: plan-subscription\n  described_by: Gravitee API Management\n  detail: >-\n    Authorization at the University of Helsinki gateway is not expressed as OAuth scopes. It is\n    expressed as a SUBSCRIPTION: an application is registered in the portal,\
  \ subscribed to one\n    named API, and granted one named plan on that API. The plan is the grant. Two APIs make this\n    visible in their own specs — Helsinki.fi content declares two separate `X-Api-Key` schemes,\n    `NewsApiKey` and `StudySearchApiKey`, described as \"issued by the news plan\" and \"issued by\n    the study search plan\", which is plan-as-scope stated in the provider's own words.\n  plan_security_enabled:\n  - apikey\n  - oauth2\n  - jwt\n  plan_security_disabled:\n  - sharedApiKey\n  - keyless\n  evidence:\n  - url: https://api.helsinki.fi/portal/environments/DEFAULT/configuration\n    status: 200\n    note: plan.security.{apikey,oauth2,jwt}.enabled true; sharedApiKey and keyless false.\n  - url: https://api.helsinki.fi/portal/environments/DEFAULT/apis?size=200\n    status: 200\n    note: >-\n      Fifteen public APIs listed. Per-API `plans` links exist on every entry but return 401\n      without a portal session, so the plan names themselves are not publicly readable.\n\
  plan_endpoints_probed:\n- url: https://api.helsinki.fi/portal/environments/DEFAULT/portal-information\n  status: 401\n  note: Authenticated-only; not readable anonymously.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/scopes/university-of-helsinki-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Finland
- Nordic
- Research
- Open Data
- Research Data
- Institutional Repository
- OAI-PMH
- Identity Federation
- API Gateway
- Course Catalog
- Library
- Biodiversity
token_urls: []
---
