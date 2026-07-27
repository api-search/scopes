---
api_specs:
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Address Suggestions API
  slug: domain-address-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Agents & Listings API
  slug: domain-agents-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Campaign API
  slug: domain-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Campaign API - Preview
  slug: domain-campaign-api-preview
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Listings Management API
  slug: domain-listings-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Price Estimation API
  slug: domain-price-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Properties & Locations API
  slug: domain-properties-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Property Enrichment API
  slug: domain-property-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Property Package API
  slug: domain-property-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain PropertyRadar API
  slug: domain-propertyradar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Rental AVM API
  slug: domain-rental-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Schools Data API
  slug: domain-schools-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Webhooks API
  slug: domain-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
authorization_urls:
- https://auth.domain.com.au/v1/connect/authorize
description: ''
docs: https://developer.domain.com.au/docs/latest/apis
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Domain Group Scopes
name_suffix: OAuth Scopes
note: Domain publishes no single scopes-reference page; each API package's documentation names the scope(s) it requires. The 25 scopes below come from the oauth2 flows in the three OpenAPI documents and from the per-operation security requirements; descriptions, api_package mapping and tag/operation usage were reconciled against the package documentation at https://developer.domain.com.au/docs/latest/apis. The scopes_supported array in the OIDC discovery document is the Domain identity platform's internal scope set (roles, address, offline_access, Domain product scopes) and is NOT the public API scope set.
overview: 'Domain Group publishes 25 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Domain Group API on a user''s behalf.


  Tokens are issued from https://auth.domain.com.au/v1/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Domain Group
provider_slug: domain-group
schemes:
- description: OAuth 2
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.domain.com.au/v1/connect/token
  - authorizationUrl: https://auth.domain.com.au/v1/connect/authorize
    flow: authorizationCode
    tokenUrl: https://auth.domain.com.au/v1/connect/token
  name: oauth2
  source: openapi/domain-group-openapi-latest.json
- description: OAuth 2
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.domain.com.au/v1/connect/token
  - authorizationUrl: https://auth.domain.com.au/v1/connect/authorize
    flow: authorizationCode
    tokenUrl: https://auth.domain.com.au/v1/connect/token
  name: oauth2
  source: openapi/domain-group-openapi-v1.json
- description: OAuth 2
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.domain.com.au/v1/connect/token
  - authorizationUrl: https://auth.domain.com.au/v1/connect/authorize
    flow: authorizationCode
    tokenUrl: https://auth.domain.com.au/v1/connect/token
  name: oauth2
  source: openapi/domain-group-openapi-v2.json
scope_count: 25
scope_names:
- api_addresslocators_read
- api_agencies_read
- api_agencies_write
- api_authorities_write
- api_avm_read
- api_campaignperformance_read
- api_dataset_read
- api_demographics_read
- api_enquiries_read
- api_enquiries_write
- api_listingperformance_read
- api_listings_read
- api_listings_write
- api_locations_read
- api_projectperformance_read
- api_properties_read
- api_propertyportfolio_read
- api_propertyportfolio_write
- api_propertyreports_read
- api_salesresults_read
- api_statistics_write
- api_suburbhistorical_read
- api_suburbperformance_read
- api_suburbsummary_read
- api_webhooks_write
scopes:
- description: Read access to the Domain addresslocators surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_addresslocators_read
- description: Read access to the Domain agencies surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_agencies_read
- description: Write access to the Domain agencies surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_agencies_write
- description: Write access to the Domain authorities surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_authorities_write
- description: Read access to the Domain avm surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_avm_read
- description: Read access to the Domain campaignperformance surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_campaignperformance_read
- description: Read access to the Domain dataset surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_dataset_read
- description: Read access to the Domain demographics surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_demographics_read
- description: Read access to the Domain enquiries surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_enquiries_read
- description: Write access to the Domain enquiries surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_enquiries_write
- description: Read access to the Domain listingperformance surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_listingperformance_read
- description: Read access to the Domain listings surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_listings_read
- description: Write access to the Domain listings surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_listings_write
- description: Read access to the Domain locations surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_locations_read
- description: Read access to the Domain projectperformance surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_projectperformance_read
- description: Read access to the Domain properties surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_properties_read
- description: Read access to the Domain propertyportfolio surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_propertyportfolio_read
- description: Write access to the Domain propertyportfolio surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_propertyportfolio_write
- description: Read access to the Domain propertyreports surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_propertyreports_read
- description: Read access to the Domain salesresults surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_salesresults_read
- description: Write access to the Domain statistics surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_statistics_write
- description: Read access to the Domain suburbhistorical surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_suburbhistorical_read
- description: Read access to the Domain suburbperformance surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_suburbperformance_read
- description: Read access to the Domain suburbsummary surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_suburbsummary_read
- description: Write access to the Domain webhooks surface.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api_webhooks_write
slug: domain-group-scopes
source_filename: domain-group-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/domain-group-openapi-latest.json, openapi/domain-group-openapi-v1.json, openapi/domain-group-openapi-v2.json,\n  https://developer.domain.com.au/docs/latest/apis\nschemes:\n- name: oauth2\n  source: openapi/domain-group-openapi-latest.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.domain.com.au/v1/connect/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.domain.com.au/v1/connect/authorize\n    tokenUrl: https://auth.domain.com.au/v1/connect/token\n  description: OAuth 2\n- name: oauth2\n  source: openapi/domain-group-openapi-v1.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.domain.com.au/v1/connect/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.domain.com.au/v1/connect/authorize\n    tokenUrl: https://auth.domain.com.au/v1/connect/token\n  description: OAuth 2\n- name: oauth2\n  source: openapi/domain-group-openapi-v2.json\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.domain.com.au/v1/connect/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.domain.com.au/v1/connect/authorize\n    tokenUrl: https://auth.domain.com.au/v1/connect/token\n  description: OAuth 2\nscopes:\n- scope: api_addresslocators_read\n  description: Read access to the Domain addresslocators surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - AddressLocators\n  operation_count: 1\n  example_operations:\n  - AddressLocators_Get\n  access: read\n  api_package: Address Suggestions\n- scope: api_agencies_read\n  description: Read access to the Domain agencies surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - Agencies\n  - Agents\n  - Leadscope\n  - Me\n\
  \  - Products\n  operation_count: 15\n  example_operations:\n  - Agencies_Get\n  - Agencies_GetStatistics\n  - Agencies_Head\n  - Agencies_Search\n  - Agents_Get\n  access: read\n  api_package: Agents & Listings\n- scope: api_agencies_write\n  description: Write access to the Domain agencies surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - Agencies\n  - Products\n  operation_count: 4\n  example_operations:\n  - Agencies_CreateTestAgency\n  - LimitedInventory_ReserveByBatch\n  - LimitedInventory_Unreserve\n  - LimitedInventory_UnreserveByBatch\n  access: write\n  api_package: Listings Management\n- scope: api_authorities_write\n  description: Write access to the Domain authorities surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - Authorities\n\
  \  operation_count: 6\n  example_operations:\n  - Authorities_Create\n  - Authorities_DownloadAttachments\n  - Authorities_GetById\n  - Authorities_UpdateById\n  - Authorities_UploadAttachment\n  access: write\n  api_package: Listings Management\n- scope: api_avm_read\n  description: Read access to the Domain avm surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - PropertyAvm\n  operation_count: 2\n  example_operations:\n  - PropertyAvm_Get\n  - PropertyAvm_ReportGet\n  access: read\n  api_package: Rental AVM\n- scope: api_campaignperformance_read\n  description: Read access to the Domain campaignperformance surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - CampaignReporting\n  operation_count: 2\n  example_operations:\n  - Campaign_GetListingPerformance_Report\n\
  \  - Campaign_GetProjectPerformance_Report\n  access: read\n  api_package: Campaign API\n- scope: api_dataset_read\n  description: Read access to the Domain dataset surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v2.json\n  tags:\n  - Dataset\n  operation_count: 1\n  example_operations:\n  - dataset_get\n  access: read\n  api_package: Properties & Locations\n- scope: api_demographics_read\n  description: Read access to the Domain demographics surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v2.json\n  tags:\n  - Demographics\n  operation_count: 1\n  example_operations:\n  - Demographics_Get_ByNamedSuburb\n  access: read\n  api_package: Properties & Locations\n- scope: api_enquiries_read\n  description: Read access to the Domain enquiries surface.\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - Enquiries\n  - Listings\n  - Projects\n  operation_count: 4\n  example_operations:\n  - Enquiries_Get\n  - Enquiries_Search\n  - Listings_GetEnquiries\n  - Projects_GetEnquiries\n  access: read\n  api_package: Agents & Listings\n- scope: api_enquiries_write\n  description: Write access to the Domain enquiries surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - Enquiries\n  - Listings\n  - Projects\n  operation_count: 5\n  example_operations:\n  - Enquiries_Get\n  - Enquiries_Post\n  - Enquiries_Search\n  - Listings_GetEnquiries\n  - Projects_GetEnquiries\n  access: write\n  api_package: Agents & Listings\n- scope: api_listingperformance_read\n  description: Read access to the Domain listingperformance surface.\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - CampaignReporting\n  operation_count: 1\n  example_operations:\n  - Campaign_GetListingPerformance_Report\n  access: read\n  api_package: Listings Management\n- scope: api_listings_read\n  description: Read access to the Domain listings surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  - openapi/domain-group-openapi-v2.json\n  tags:\n  - Agencies\n  - Agents\n  - ListingSearch\n  - Listings\n  - PreMarket\n  - Projects\n  - Properties\n  operation_count: 20\n  example_operations:\n  - Agencies_GetListings\n  - Agents_GetListings\n  - ListingLocations_Search\n  - Listings_DetailedBusinessSearch\n  - Listings_DetailedCommercialSearch\n  access: read\n  api_package: Agents & Listings\n- scope: api_listings_write\n  description: Write access\
  \ to the Domain listings surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  - openapi/domain-group-openapi-v2.json\n  tags:\n  - Listings\n  - Me\n  - PreMarket\n  - Projects\n  operation_count: 17\n  example_operations:\n  - ListingLocations_Search\n  - Listings_DetailedBusinessSearch\n  - Listings_DetailedCommercialSearch\n  - Listings_DetailedResidentialSearch\n  - Listings_Get\n  access: write\n  api_package: Listings Management\n- scope: api_locations_read\n  description: Read access to the Domain locations surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  - openapi/domain-group-openapi-v2.json\n  tags:\n  - Locations\n  - Schools\n  operation_count: 3\n  example_operations:\n  - LocationProfiles_Get\n  - Schools_Get_ById\n  - Schools_Search_ByLocation\n\
  \  access: read\n  api_package: Agents & Listings\n- scope: api_projectperformance_read\n  description: Read access to the Domain projectperformance surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - CampaignReporting\n  operation_count: 1\n  example_operations:\n  - Campaign_GetProjectPerformance_Report\n  access: read\n  api_package: Campaign API\n- scope: api_properties_read\n  description: Read access to the Domain properties surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  - openapi/domain-group-openapi-v2.json\n  tags:\n  - Disclaimers\n  - Properties\n  - PropertyFeatures\n  - PropertyLike\n  - PropertySearch\n  - PropertyZoningPerils\n  operation_count: 14\n  example_operations:\n  - Disclaimers_Get\n  - Disclaimers_GetByProduct\n  - Properties_Get\n\
  \  - Properties_GetPriceEstimate\n  - Properties_GetRentalEstimate\n  access: read\n  api_package: Properties & Locations\n- scope: api_propertyportfolio_read\n  description: Read access to the Domain propertyportfolio surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - PropertyRadar\n  operation_count: 5\n  example_operations:\n  - PropertyRadar_ListPortfolios\n  - PropertyRadar_ViewPortfolio\n  - PropertyRadar_ViewPortfolioFull\n  - PropertyRadar_viewPortfolioFullSingle\n  - PropertyRadar_viewPortfolioFullSingleByGnafId\n  access: read\n  api_package: PropertyRadar\n- scope: api_propertyportfolio_write\n  description: Write access to the Domain propertyportfolio surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - PropertyRadar\n  operation_count:\
  \ 4\n  example_operations:\n  - PropertyRadar_AddToPortfolio\n  - PropertyRadar_CreatePortfolio\n  - PropertyRadar_DeletePortfolio\n  - PropertyRadar_RemoveFromPortfolio\n  access: write\n  api_package: PropertyRadar\n- scope: api_propertyreports_read\n  description: Read access to the Domain propertyreports surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - Properties\n  operation_count: 1\n  example_operations:\n  - PropertyReports_Get\n  access: read\n- scope: api_salesresults_read\n  description: Read access to the Domain salesresults surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  - openapi/domain-group-openapi-v2.json\n  tags:\n  - SalesResults\n  operation_count: 5\n  example_operations:\n  - SalesResults_Get\n  - SalesResults_Head\n \
  \ - SalesResults_Listings\n  - SalesResults_SaturdayReport\n  - SalesResults_WeeklyMediaReport\n  access: read\n  api_package: Properties & Locations\n- scope: api_statistics_write\n  description: Write access to the Domain statistics surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - Statistics\n  operation_count: 1\n  example_operations:\n  - Statistics_Post\n  access: write\n- scope: api_suburbhistorical_read\n  description: Read access to the Domain suburbhistorical surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - Statistics\n  operation_count: 1\n  example_operations:\n  - SuburbHistorical_Get\n  access: read\n- scope: api_suburbperformance_read\n  description: Read access to the Domain suburbperformance surface.\n  flows:\n  -\
  \ authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  - openapi/domain-group-openapi-v2.json\n  tags:\n  - Statistics\n  operation_count: 3\n  example_operations:\n  - SuburbPerformanceStatistics_Get\n  - SuburbPerformance_Get_ByNamedSuburb\n  - SuburbPerformance_Get_ByNamedSuburb_WithoutPostcode\n  access: read\n  api_package: Properties & Locations\n- scope: api_suburbsummary_read\n  description: Read access to the Domain suburbsummary surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  tags:\n  - Statistics\n  operation_count: 1\n  example_operations:\n  - SuburbSummary_Get\n  access: read\n- scope: api_webhooks_write\n  description: Write access to the Domain webhooks surface.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/domain-group-openapi-latest.json\n\
  \  - openapi/domain-group-openapi-v1.json\n  tags:\n  - Authorities\n  - Webhooks\n  operation_count: 6\n  example_operations:\n  - Authorities_Subscribe\n  - Authorities_Unsubscribe\n  - Webhooks_CreateSubscription\n  - Webhooks_DeleteSubscription\n  - Webhooks_GetSubscription\n  access: write\n  api_package: Webhooks\ndocs: https://developer.domain.com.au/docs/latest/apis\nnote: Domain publishes no single scopes-reference page; each API package's documentation names the scope(s)\n  it requires. The 25 scopes below come from the oauth2 flows in the three OpenAPI documents and from\n  the per-operation security requirements; descriptions, api_package mapping and tag/operation usage were\n  reconciled against the package documentation at https://developer.domain.com.au/docs/latest/apis. The\n  scopes_supported array in the OIDC discovery document is the Domain identity platform's internal scope\n  set (roles, address, offline_access, Domain product scopes) and is NOT the public API scope\
  \ set.\ntoken_url: https://auth.domain.com.au/v1/connect/token\nauthorization_url: https://auth.domain.com.au/v1/connect/authorize\nscope_count: 25\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/scopes/domain-group-scopes.yml
summary_line: 25 scopes · clientCredentials/authorizationCode
tags:
- Real Estate
- Australia
- Property Listings
- Property Data
- Valuation
- AVM
- Rentals
- Listing Management
- PropTech
- Portal Marketplace
token_urls:
- https://auth.domain.com.au/v1/connect/token
---
