---
api_specs:
- filename: constructorio-search-openapi.yml
  format: yaml
  label: Constructor Search API
  slug: constructor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-search-openapi.yml
- filename: constructorio-autocomplete-openapi.yml
  format: yaml
  label: Constructor Autocomplete API
  slug: constructor-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-autocomplete-openapi.yml
- filename: constructorio-browse-openapi.yml
  format: yaml
  label: Constructor Browse API
  slug: constructor-browse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-browse-openapi.yml
- filename: constructorio-recommendations-openapi.yml
  format: yaml
  label: Constructor Recommendations API
  slug: constructor-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-recommendations-openapi.yml
- filename: constructorio-image-search-openapi.yml
  format: yaml
  label: Constructor Image Search API
  slug: constructor-image-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-image-search-openapi.yml
- filename: constructorio-ai-shopping-agent-openapi.yml
  format: yaml
  label: Constructor AI Shopping Agent API
  slug: constructor-ai-shopping-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-ai-shopping-agent-openapi.yml
- filename: constructorio-catalog-management-openapi.yml
  format: yaml
  label: Constructor Catalog Management API
  slug: constructor-catalog-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-catalog-management-openapi.yml
- filename: constructorio-catalog-batching-openapi.yml
  format: yaml
  label: Constructor Catalog Batching API
  slug: constructor-catalog-batching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-catalog-batching-openapi.yml
- filename: constructorio-configuration-openapi.yml
  format: yaml
  label: Constructor Configuration API
  slug: constructor-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-configuration-openapi.yml
- filename: constructorio-searchandising-openapi.yml
  format: yaml
  label: Constructor Searchandising API
  slug: constructor-searchandising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-searchandising-openapi.yml
- filename: constructorio-quizzes-openapi.yml
  format: yaml
  label: Constructor Quizzes API
  slug: constructor-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-quizzes-openapi.yml
- filename: constructorio-offsite-discovery-recommendations-openapi.yml
  format: yaml
  label: Constructor Offsite Discovery Recommendations API
  slug: constructor-offsite-discovery-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-offsite-discovery-recommendations-openapi.yml
- filename: constructorio-retail-media-openapi.yml
  format: yaml
  label: Constructor Retail Media API
  slug: constructor-retail-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-retail-media-openapi.yml
- filename: constructorio-retail-media-display-ads-openapi.yml
  format: yaml
  label: Constructor Retail Media Display Ads API
  slug: constructor-retail-media-display-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-retail-media-display-ads-openapi.yml
- filename: constructorio-product-details-openapi.yml
  format: yaml
  label: Constructor Product Details API
  slug: constructor-product-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-product-details-openapi.yml
- filename: constructorio-behavioral-actions-openapi.yml
  format: yaml
  label: Constructor Behavioral Actions API
  slug: constructor-behavioral-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-behavioral-actions-openapi.yml
- filename: constructorio-user-profile-openapi.yml
  format: yaml
  label: Constructor User Profile API
  slug: constructor-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-user-profile-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.constructor.com/reference/main-authentication#permissions-and-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Constructorio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Constructor.io publishes 37 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Constructor.io API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Constructor.io
provider_slug: constructorio
schemes:
- name: http_bearer_auth
  scheme: bearer
  sources:
  - openapi/constructorio-autocomplete-openapi.yml
  - openapi/constructorio-browse-openapi.yml
  - openapi/constructorio-catalog-batching-openapi.yml
  - openapi/constructorio-catalog-management-openapi.yml
  - openapi/constructorio-configuration-openapi.yml
  - openapi/constructorio-image-search-openapi.yml
  - openapi/constructorio-product-details-openapi.yml
  - openapi/constructorio-recommendations-openapi.yml
  - openapi/constructorio-search-openapi.yml
  - openapi/constructorio-searchandising-openapi.yml
  - openapi/constructorio-user-profile-openapi.yml
  type: http
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/constructorio-retail-media-display-ads-openapi.yml
  - openapi/constructorio-retail-media-openapi.yml
  type: http
scope_count: 37
scope_names:
- catalog(r)
- catalog(w)
- collections(r)
- collections(w)
- facets(r)
- facets(w)
- facets.refined_filters(r)
- facets.refined_filters(w)
- facets.refined_queries(r)
- facets.refined_queries(w)
- metadata_overrides(r)
- metadata_overrides(w)
- quizzes(r)
- quizzes(w)
- redirects(r)
- redirects(w)
- retail_media.ad_spend_tracking(r)
- retail_media.engagements(w)
- search_suggestions(w)
- searchabilities(r)
- searchabilities(w)
- searchandising.campaigns(r)
- searchandising.campaigns(w)
- searchandising.recommendations(r)
- searchandising.recommendations(w)
- searchandising.refined_collections(r)
- searchandising.refined_collections(w)
- searchandising.refined_filters(r)
- searchandising.refined_filters(w)
- searchandising.refined_queries(r)
- searchandising.refined_queries(w)
- searchandising.refined_tags(r)
- searchandising.refined_tags(w)
- sort_options(r)
- sort_options(w)
- synonyms(r)
- synonyms(w)
scopes:
- description: ''
  flows: []
  scope: catalog(r)
- description: ''
  flows: []
  scope: catalog(w)
- description: ''
  flows: []
  scope: collections(r)
- description: ''
  flows: []
  scope: collections(w)
- description: ''
  flows: []
  scope: facets(r)
- description: ''
  flows: []
  scope: facets(w)
- description: ''
  flows: []
  scope: facets.refined_filters(r)
- description: ''
  flows: []
  scope: facets.refined_filters(w)
- description: ''
  flows: []
  scope: facets.refined_queries(r)
- description: ''
  flows: []
  scope: facets.refined_queries(w)
- description: ''
  flows: []
  scope: metadata_overrides(r)
- description: ''
  flows: []
  scope: metadata_overrides(w)
- description: ''
  flows: []
  scope: quizzes(r)
- description: ''
  flows: []
  scope: quizzes(w)
- description: ''
  flows: []
  scope: redirects(r)
- description: ''
  flows: []
  scope: redirects(w)
- description: ''
  flows: []
  scope: retail_media.ad_spend_tracking(r)
- description: ''
  flows: []
  scope: retail_media.engagements(w)
- description: ''
  flows: []
  scope: search_suggestions(w)
- description: ''
  flows: []
  scope: searchabilities(r)
- description: ''
  flows: []
  scope: searchabilities(w)
- description: ''
  flows: []
  scope: searchandising.campaigns(r)
- description: ''
  flows: []
  scope: searchandising.campaigns(w)
- description: ''
  flows: []
  scope: searchandising.recommendations(r)
- description: ''
  flows: []
  scope: searchandising.recommendations(w)
- description: ''
  flows: []
  scope: searchandising.refined_collections(r)
- description: ''
  flows: []
  scope: searchandising.refined_collections(w)
- description: ''
  flows: []
  scope: searchandising.refined_filters(r)
- description: ''
  flows: []
  scope: searchandising.refined_filters(w)
- description: ''
  flows: []
  scope: searchandising.refined_queries(r)
- description: ''
  flows: []
  scope: searchandising.refined_queries(w)
- description: ''
  flows: []
  scope: searchandising.refined_tags(r)
- description: ''
  flows: []
  scope: searchandising.refined_tags(w)
- description: ''
  flows: []
  scope: sort_options(r)
- description: ''
  flows: []
  scope: sort_options(w)
- description: ''
  flows: []
  scope: synonyms(r)
- description: ''
  flows: []
  scope: synonyms(w)
slug: constructorio-scopes
source_filename: constructorio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/*.yml operation security[] requirements\ndocs: https://docs.constructor.com/reference/main-authentication#permissions-and-scopes\noauth2: false\nscheme_type: http-bearer token permissions (NOT OAuth 2.0)\nmodel: 'Constructor Bearer API tokens carry explicit permissions. A permission is {\"scope\": \"<scope>\",\n  \"operation\": \"r|w|rw\", \"resources\": [\"<API key>\", ...]}. Scopes appear in the API reference in the form\n  scope(r) / scope(w). A token lacking the required permission is rejected with 403 Forbidden; a missing\n  or malformed token is rejected with 401 Unauthorized. `resources` currently accepts API keys, scoping\n  a token to specific indexes.'\nschemes:\n- name: http_bearer_auth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/constructorio-autocomplete-openapi.yml\n  - openapi/constructorio-browse-openapi.yml\n  - openapi/constructorio-catalog-batching-openapi.yml\n  - openapi/constructorio-catalog-management-openapi.yml\n\
  \  - openapi/constructorio-configuration-openapi.yml\n  - openapi/constructorio-image-search-openapi.yml\n  - openapi/constructorio-product-details-openapi.yml\n  - openapi/constructorio-recommendations-openapi.yml\n  - openapi/constructorio-search-openapi.yml\n  - openapi/constructorio-searchandising-openapi.yml\n  - openapi/constructorio-user-profile-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/constructorio-retail-media-display-ads-openapi.yml\n  - openapi/constructorio-retail-media-openapi.yml\nscope_count: 37\nscopes:\n- scope: catalog(r)\n  resource: catalog\n  operation: read\n  operation_count: 12\n  operations:\n  - v1-item-groups-retrieve-item-group\n  - v1-item-groups-retrieve-item-groups\n  - v1-items-fields-stats-retrieve-item-field-stats\n  - v1-items-fields-stats-retrieve-items-fields-stats\n  - v1-tasks-retrieve-task\n  - v1-tasks-retrieve-tasks\n  - v2-item-groups-retrieve-item-group\n  - v2-item-groups-retrieve-item-groups\n\
  - scope: catalog(w)\n  resource: catalog\n  operation: write\n  operation_count: 23\n  operations:\n  - v1-catalog-create-or-replace-catalog\n  - v1-catalog-update-catalog\n  - v1-item-groups-create-item-groups\n  - v1-item-groups-create-or-replace-item-groups\n  - v1-item-groups-create-or-update-item-group\n  - v1-item-groups-create-or-update-item-groups\n  - v1-item-groups-delete-item-groups\n  - v1-tasks-create-task\n- scope: collections(r)\n  resource: collections\n  operation: read\n  operation_count: 3\n  operations:\n  - v1-collections-retrieve-collection\n  - v1-collections-retrieve-collection-items\n  - v1-collections-retrieve-collections\n- scope: collections(w)\n  resource: collections\n  operation: write\n  operation_count: 7\n  operations:\n  - v1-collections-create-collection\n  - v1-collections-create-or-ignore-collection-items\n  - v1-collections-delete-collection\n  - v1-collections-delete-collection-item\n  - v1-collections-delete-collection-items\n  - v1-collections-replace-collection\n\
  \  - v1-collections-update-collection\n- scope: facets(r)\n  resource: facets\n  operation: read\n  operation_count: 6\n  operations:\n  - v1-facet-options-retrieve-facet-option\n  - v1-facet-options-retrieve-facet-options\n  - v1-facets-retrieve-facet\n  - v1-facets-retrieve-facets\n  - v2-facets-retrieve-facet\n  - v2-facets-retrieve-facets\n- scope: facets(w)\n  resource: facets\n  operation: write\n  operation_count: 17\n  operations:\n  - v1-facet-options-create-facet-option\n  - v1-facet-options-create-or-update-facet-options\n  - v1-facet-options-delete-facet-option\n  - v1-facet-options-replace-facet-option\n  - v1-facet-options-update-facet-option\n  - v1-facets-create-facet\n  - v1-facets-create-or-replace-facets\n  - v1-facets-delete-facet\n- scope: facets.refined_filters(r)\n  resource: facets.refined_filters\n  operation: read\n  operation_count: 4\n  operations:\n  - v1-searchandising-get-facet-rule-campaign\n  - v1-searchandising-retrieve-facet-rule-campaigns\n  - v1-searchandising-retrieve-refined-filter\n\
  \  - v1-searchandising-retrieve-refined-filters\n- scope: facets.refined_filters(w)\n  resource: facets.refined_filters\n  operation: write\n  operation_count: 5\n  operations:\n  - v1-searchandising-create-facet-rule-campaign\n  - v1-searchandising-create-or-replace-refined-filter\n  - v1-searchandising-delete-facet-rule-campaign\n  - v1-searchandising-delete-refined-filter-rules\n  - v1-searchandising-update-facet-rule-campaign\n- scope: facets.refined_queries(r)\n  resource: facets.refined_queries\n  operation: read\n  operation_count: 4\n  operations:\n  - v1-searchandising-get-facet-rule-campaign\n  - v1-searchandising-retrieve-facet-rule-campaigns\n  - v1-searchandising-retrieve-refined-queries\n  - v1-searchandising-retrieve-refined-query\n- scope: facets.refined_queries(w)\n  resource: facets.refined_queries\n  operation: write\n  operation_count: 5\n  operations:\n  - v1-searchandising-create-facet-rule-campaign\n  - v1-searchandising-create-refined-query\n  - v1-searchandising-delete-facet-rule-campaign\n\
  \  - v1-searchandising-replace-refined-query\n  - v1-searchandising-update-facet-rule-campaign\n- scope: metadata_overrides(r)\n  resource: metadata_overrides\n  operation: read\n  operation_count: 1\n  operations:\n  - metadata-overrides-get-metadata-overrides\n- scope: metadata_overrides(w)\n  resource: metadata_overrides\n  operation: write\n  operation_count: 3\n  operations:\n  - metadata-overrides-delete-metadata-override\n  - metadata-overrides-patch-metadata-override\n  - metadata-overrides-post-metadata-override\n- scope: quizzes(r)\n  resource: quizzes\n  operation: read\n  operation_count: 1\n  operations:\n  - v1-quizzes-retrieve-quiz\n- scope: quizzes(w)\n  resource: quizzes\n  operation: write\n  operation_count: 3\n  operations:\n  - v1-quizzes-create-or-replace-quiz\n  - v1-quizzes-delete-quiz\n  - v1-quizzes-update-quiz\n- scope: redirects(r)\n  resource: redirects\n  operation: read\n  operation_count: 2\n  operations:\n  - v1-redirects-retrieve-redirect-rule\n  - v1-redirects-retrieve-redirect-rules\n\
  - scope: redirects(w)\n  resource: redirects\n  operation: write\n  operation_count: 4\n  operations:\n  - v1-redirects-create-redirect-rule\n  - v1-redirects-delete-redirect-rule\n  - v1-redirects-replace-redirect-rule\n  - v1-redirects-update-redirect-rule\n- scope: retail_media.ad_spend_tracking(r)\n  resource: retail_media.ad_spend_tracking\n  operation: read\n  operation_count: 1\n  operations:\n  - v1-advertiser-spend-retrieve-advertiser-spend\n- scope: retail_media.engagements(w)\n  resource: retail_media.engagements\n  operation: write\n  operation_count: 1\n  operations:\n  - v1-engagements-update\n- scope: search_suggestions(w)\n  resource: search_suggestions\n  operation: write\n  operation_count: 8\n  operations:\n  - v1-catalog-create-or-replace-catalog\n  - v1-catalog-update-catalog\n  - v2-items-create-or-replace-items\n  - v2-items-delete-items\n  - v2-items-update-items\n  - v2-variations-create-or-replace-variations\n  - v2-variations-delete-variations\n  - v2-variations-update-variations\n\
  - scope: searchabilities(r)\n  resource: searchabilities\n  operation: read\n  operation_count: 4\n  operations:\n  - v1-searchabilities-retrieve-searchabilities\n  - v1-searchabilities-retrieve-searchability\n  - v2-searchabilities-retrieve-searchabilities\n  - v2-searchabilities-retrieve-searchability\n- scope: searchabilities(w)\n  resource: searchabilities\n  operation: write\n  operation_count: 8\n  operations:\n  - v1-searchabilities-create-or-update-searchabilities\n  - v1-searchabilities-create-or-update-searchability\n  - v1-searchabilities-delete-searchabilities\n  - v1-searchabilities-delete-searchability\n  - v2-searchabilities-create-or-update-searchabilities\n  - v2-searchabilities-create-or-update-searchability\n  - v2-searchabilities-delete-searchabilities\n  - v2-searchabilities-delete-searchability\n- scope: searchandising.campaigns(r)\n  resource: searchandising.campaigns\n  operation: read\n  operation_count: 2\n  operations:\n  - v1-searchandising-retrieve-campaign\n\
  \  - v1-searchandising-retrieve-campaigns\n- scope: searchandising.campaigns(w)\n  resource: searchandising.campaigns\n  operation: write\n  operation_count: 3\n  operations:\n  - v1-searchandising-create-campaign\n  - v1-searchandising-delete-campaign\n  - v1-searchandising-update-campaign\n- scope: searchandising.recommendations(r)\n  resource: searchandising.recommendations\n  operation: read\n  operation_count: 2\n  operations:\n  - v1-searchandising-retrieve-campaign\n  - v1-searchandising-retrieve-campaigns\n- scope: searchandising.recommendations(w)\n  resource: searchandising.recommendations\n  operation: write\n  operation_count: 3\n  operations:\n  - v1-searchandising-create-campaign\n  - v1-searchandising-delete-campaign\n  - v1-searchandising-update-campaign\n- scope: searchandising.refined_collections(r)\n  resource: searchandising.refined_collections\n  operation: read\n  operation_count: 2\n  operations:\n  - v1-searchandising-retrieve-refined-collection\n  - v1-searchandising-retrieve-refined-collections\n\
  - scope: searchandising.refined_collections(w)\n  resource: searchandising.refined_collections\n  operation: write\n  operation_count: 3\n  operations:\n  - v1-searchandising-create-or-replace-refined-collection\n  - v1-searchandising-delete-refined-collection\n  - v1-searchandising-update-refined-collection\n- scope: searchandising.refined_filters(r)\n  resource: searchandising.refined_filters\n  operation: read\n  operation_count: 3\n  operations:\n  - v1-searchandising-retrieve-refined-filter\n  - v1-searchandising-retrieve-refined-filter-rules\n  - v1-searchandising-retrieve-refined-filters\n- scope: searchandising.refined_filters(w)\n  resource: searchandising.refined_filters\n  operation: write\n  operation_count: 4\n  operations:\n  - v1-searchandising-create-or-replace-refined-filter\n  - v1-searchandising-delete-refined-filter\n  - v1-searchandising-delete-refined-filter-rules\n  - v1-searchandising-update-refined-filter\n- scope: searchandising.refined_queries(r)\n  resource:\
  \ searchandising.refined_queries\n  operation: read\n  operation_count: 2\n  operations:\n  - v1-searchandising-retrieve-refined-queries\n  - v1-searchandising-retrieve-refined-query\n- scope: searchandising.refined_queries(w)\n  resource: searchandising.refined_queries\n  operation: write\n  operation_count: 4\n  operations:\n  - v1-searchandising-create-refined-query\n  - v1-searchandising-delete-refined-query\n  - v1-searchandising-replace-refined-query\n  - v1-searchandising-update-refined-query\n- scope: searchandising.refined_tags(r)\n  resource: searchandising.refined_tags\n  operation: read\n  operation_count: 2\n  operations:\n  - v1-searchandising-retreive-refined-tags\n  - v1-searchandising-retrieve-refined-tag\n- scope: searchandising.refined_tags(w)\n  resource: searchandising.refined_tags\n  operation: write\n  operation_count: 3\n  operations:\n  - v1-searchandising-create-or-replace-refined-tag\n  - v1-searchandising-delete-refined-tag\n  - v1-searchandising-update-refined-tag\n\
  - scope: sort_options(r)\n  resource: sort_options\n  operation: read\n  operation_count: 1\n  operations:\n  - v1-sort-options-retrieve-sort-options\n- scope: sort_options(w)\n  resource: sort_options\n  operation: write\n  operation_count: 5\n  operations:\n  - v1-sort-options-create-or-replace-sort-option\n  - v1-sort-options-create-or-replace-sort-options\n  - v1-sort-options-create-sort-option\n  - v1-sort-options-delete-sort-options\n  - v1-sort-options-update-sort-option\n- scope: synonyms(r)\n  resource: synonyms\n  operation: read\n  operation_count: 4\n  operations:\n  - v1-synonyms-list-synonyms\n  - v1-synonyms-retrieve-synonym\n  - v2-one-way-synonyms-retrieve-one-way-synonym\n  - v2-one-way-synonyms-retrieve-one-way-synonyms\n- scope: synonyms(w)\n  resource: synonyms\n  operation: write\n  operation_count: 8\n  operations:\n  - v1-synonyms-create-synonym\n  - v1-synonyms-delete-synonym\n  - v1-synonyms-delete-synonyms\n  - v1-synonyms-update-synonym\n  - v2-one-way-synonyms-create-one-way-synonym\n\
  \  - v2-one-way-synonyms-delete-one-way-synonym\n  - v2-one-way-synonyms-delete-one-way-synonyms\n  - v2-one-way-synonyms-replace-one-way-synonym\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/scopes/constructorio-scopes.yml
summary_line: 37 scopes
tags:
- Company
- Search
- Ecommerce
- Product Discovery
- Recommendations
- Personalization
- Retail
- Retail Media
- Artificial Intelligence
- Merchandising
- Catalog Management
- Agentic Commerce
token_urls: []
---
