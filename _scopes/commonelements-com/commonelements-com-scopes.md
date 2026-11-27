---
api_specs:
- filename: commonelements-com-aggregates-and-compliance-api-openapi.yml
  format: yaml
  label: Common Elements Aggregates and compliance API
  slug: commonelements-com-aggregates-and-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-aggregates-and-compliance-api-openapi.yml
- filename: commonelements-com-association-resources-api-openapi.yml
  format: yaml
  label: Common Elements Association resources API
  slug: commonelements-com-association-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-association-resources-api-openapi.yml
- filename: commonelements-com-associations-api-openapi.yml
  format: yaml
  label: Common Elements Associations API
  slug: commonelements-com-associations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-associations-api-openapi.yml
- filename: commonelements-com-bulk-delivery-api-openapi.yml
  format: yaml
  label: Common Elements Bulk delivery API
  slug: commonelements-com-bulk-delivery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-bulk-delivery-api-openapi.yml
- filename: commonelements-com-bulk-export-api-openapi.yml
  format: yaml
  label: Common Elements Bulk export API
  slug: commonelements-com-bulk-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-bulk-export-api-openapi.yml
- filename: commonelements-com-change-feed-api-openapi.yml
  format: yaml
  label: Common Elements Change feed API
  slug: commonelements-com-change-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-change-feed-api-openapi.yml
- filename: commonelements-com-cross-association-collections-api-openapi.yml
  format: yaml
  label: Common Elements Cross-association collections API
  slug: commonelements-com-cross-association-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-cross-association-collections-api-openapi.yml
- filename: commonelements-com-dataset-catalog-api-openapi.yml
  format: yaml
  label: Common Elements Dataset catalog API
  slug: commonelements-com-dataset-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-dataset-catalog-api-openapi.yml
- filename: commonelements-com-meta-api-openapi.yml
  format: yaml
  label: Common Elements Meta API
  slug: commonelements-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-meta-api-openapi.yml
- filename: commonelements-com-professionals-and-licenses-api-openapi.yml
  format: yaml
  label: Common Elements Professionals and licenses API
  slug: commonelements-com-professionals-and-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-professionals-and-licenses-api-openapi.yml
- filename: commonelements-com-statutes-api-openapi.yml
  format: yaml
  label: Common Elements Statutes API
  slug: commonelements-com-statutes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-statutes-api-openapi.yml
- filename: commonelements-com-vendors-api-openapi.yml
  format: yaml
  label: Common Elements Vendors API
  slug: commonelements-com-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonelements-com/openapi/commonelements-com-vendors-api-openapi.yml
authorization_urls: []
description: REST API keys carry per-resource scopes (enforced as 403 scope_not_allowed); these are API-key scopes, not OAuth scopes. The MCP server separately uses OAuth with read/write grants split per domain ("Read and write are separate grants; granting read never implies write. Read-only is the default." -- https://commonelements.com/developers/mcp); its OAuth scope names are not listed on that page.
docs: https://commonelements.com/developers/docs
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Common Elements Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Common Elements publishes 19 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Common Elements API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Common Elements
provider_slug: commonelements-com
schemes: []
scope_count: 19
scope_names:
- associations
- changes
- statutes
- risk
- vendors.read
- vendors
- licenses
- professionals
- compliance
- property
- permits
- enforcement
- documents
- financials
- governance
- hazard
- insurance
- legal
- valuations
scopes:
- description: Association records
  flows: []
  scope: associations
- description: Change feed (/api/v1/changes, /changes/summary); "changes or associations".
  flows: []
  scope: changes
- description: Statute endpoints; "statutes or associations".
  flows: []
  scope: statutes
- description: Risk/flood and building-safety endpoints.
  flows: []
  scope: risk
- description: Vendor directory search and vendor detail.
  flows: []
  scope: vendors.read
- description: Vendor reviews.
  flows: []
  scope: vendors
- description: License verification.
  flows: []
  scope: licenses
- description: Licensed professional search
  flows: []
  scope: professionals
- description: Compliance scan of governing documents.
  flows: []
  scope: compliance
- description: Parcels and structures resources.
  flows: []
  scope: property
- description: Building permits resource.
  flows: []
  scope: permits
- description: Code enforcement / violations resource.
  flows: []
  scope: enforcement
- description: Recorded documents resource.
  flows: []
  scope: documents
- description: Financials resource.
  flows: []
  scope: financials
- description: Governance resource.
  flows: []
  scope: governance
- description: Hazards resource.
  flows: []
  scope: hazard
- description: Insurance resources.
  flows: []
  scope: insurance
- description: Legal resources.
  flows: []
  scope: legal
- description: Building structural facts / valuations resource.
  flows: []
  scope: valuations
slug: commonelements-com-scopes
source_filename: commonelements-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: 'generated: ''2026-11-04''

  method: searched

  source: https://commonelements.com/developers/docs

  docs: https://commonelements.com/developers/docs

  description: ''REST API keys carry per-resource scopes (enforced as 403 scope_not_allowed); these are API-key scopes, not OAuth scopes. The MCP server separately uses OAuth with read/write grants split per domain ("Read and write are separate grants; granting read never implies write. Read-only is the default." -- https://commonelements.com/developers/mcp); its OAuth scope names are not listed on that page.''

  scopes:

  - {scope: associations, description: Association records, lookup/match/by-address/nearby, datasets, statutes and change feed (alternative)., schemes: [bearerAuth]}

  - {scope: changes, description: ''Change feed (/api/v1/changes, /changes/summary); "changes or associations".'', schemes: [bearerAuth]}

  - {scope: statutes, description: ''Statute endpoints; "statutes or associations".'', schemes: [bearerAuth]}

  - {scope: risk, description: Risk/flood and building-safety endpoints., schemes: [bearerAuth]}

  - {scope: vendors.read, description: Vendor directory search and vendor detail., schemes: [bearerAuth]}

  - {scope: vendors, description: Vendor reviews., schemes: [bearerAuth]}

  - {scope: licenses, description: License verification., schemes: [bearerAuth]}

  - {scope: professionals, description: Licensed professional search, detail and associations., schemes: [bearerAuth]}

  - {scope: compliance, description: Compliance scan of governing documents., schemes: [bearerAuth]}

  - {scope: property, description: Parcels and structures resources., schemes: [bearerAuth]}

  - {scope: permits, description: Building permits resource., schemes: [bearerAuth]}

  - {scope: enforcement, description: Code enforcement / violations resource., schemes: [bearerAuth]}

  - {scope: documents, description: Recorded documents resource., schemes: [bearerAuth]}

  - {scope: financials, description: Financials resource., schemes: [bearerAuth]}

  - {scope: governance, description: Governance resource., schemes: [bearerAuth]}

  - {scope: hazard, description: Hazards resource., schemes: [bearerAuth]}

  - {scope: insurance, description: Insurance resources., schemes: [bearerAuth]}

  - {scope: legal, description: Legal resources., schemes: [bearerAuth]}

  - {scope: valuations, description: Building structural facts / valuations resource., schemes: [bearerAuth]}

  '
source_yaml_url: https://artifacts.apis.io/commonelements-com/scopes/commonelements-com-scopes.yml
summary_line: 19 scopes
tags:
- Company
- HOA
- Community Associations
- Real Estate
- PropTech
- Property Data
- Compliance
- Flood Risk
token_bound: false
token_urls: []
---
