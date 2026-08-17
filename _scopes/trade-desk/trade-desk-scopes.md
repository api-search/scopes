---
api_specs:
- filename: trade-desk-advertiser-api-openapi.yml
  format: yaml
  label: The Trade Desk Advertiser API
  slug: trade-desk-advertiser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-advertiser-api-openapi.yml
- filename: trade-desk-deletionoptout-api-openapi.yml
  format: yaml
  label: The Trade Desk DeletionOptOut API
  slug: trade-desk-deletionoptout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-deletionoptout-api-openapi.yml
- filename: trade-desk-offlineconversion-api-openapi.yml
  format: yaml
  label: The Trade Desk OfflineConversion API
  slug: trade-desk-offlineconversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-offlineconversion-api-openapi.yml
- filename: trade-desk-thirdparty-api-openapi.yml
  format: yaml
  label: The Trade Desk ThirdParty API
  slug: trade-desk-thirdparty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-thirdparty-api-openapi.yml
- filename: trade-desk-ipaddress-api-openapi.yml
  format: yaml
  label: The Trade Desk IPAddress Data API
  slug: trade-desk-ipaddress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/openapi/trade-desk-ipaddress-api-openapi.yml
authorization_urls:
- https://auth.thetradedesk.com/connect/authorize
description: ''
docs: https://open.thetradedesk.com/advertiser/docsApp/Foundations/resources/doc/PlatformAuthentication
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Trade Desk Scopes
name_suffix: OAuth Scopes
note: Scopes are read from The Trade Desk's live OpenID Connect discovery document, not from an OpenAPI — none of the published Data API specs declare an oauth2 securityScheme. The provider does not publish a scopes/permissions reference page, so descriptions are supplied only where the scope name is unambiguous; the rest are recorded verbatim with no invented description.
overview: 'The Trade Desk publishes 91 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the The Trade Desk API on a user''s behalf.


  Tokens are issued from https://auth.thetradedesk.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Trade Desk
provider_slug: trade-desk
schemes:
- flows:
  - authorizationUrl: https://auth.thetradedesk.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://auth.thetradedesk.com/connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.thetradedesk.com/connect/token
  - deviceAuthorizationUrl: https://auth.thetradedesk.com/connect/deviceauthorization
    flow: deviceCode
    tokenUrl: https://auth.thetradedesk.com/connect/token
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  - delegated
  - urn:ietf:params:oauth:grant-type:azure-token-exchange
  - urn:ttd:params:oauth:grant-type:service-account
  issuer: https://auth.thetradedesk.com
  name: OpenIDConnect
  pkce:
  - plain
  - S256
  source: https://auth.thetradedesk.com/.well-known/openid-configuration
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
scope_count: 91
scope_names:
- openid
- profile
- email
- offline_access
- ttdapi
- activity.read_write
- ad_format.read
- ad_technology.read
- adgroup.activity.read
- adgroup.basic_read
- adgroup.basic_update
- adgroup.basic_write
- adgroup.delta.read
- adgroup.read_write
- advertiser.delta.read
- advertiser.overview.read
- advertiser.read
- advertiser.read_write
- advertiser_targeting.read
- audience.basic_read
- audience_workflows.write
- bidlist.basic_write
- bidlist.read_write
- billing_and_fees.write
- campaign.activity.read
- campaign.basic_read
- campaign.basic_write
- campaign.delta.read
- campaign.read_write
- campaign.write
- campaign_flight.create
- campaign_flight.read
- category.read
- category_taxonomy.read
- comscore.read
- content.read
- contract.delta.read
- contract.partner.read
- contract.read_write
- contract_group.read_write
- creative.delta.read
- creative.read
- creative.read_write
- creative.write
- currency.read
- data_group.read
- delivery_profile.read
- delivery_profile.read_write
- delta.read
- device_make_model.read
- direct_url_targeting_category.read
- fees.basic_write
- fees.read
- fees.read_write
- first_party.read
- frequency_counter.update
- geo_segment.read
- label.read_write
- language.read
- metadata_and_queries.write
- mobile_application.read
- mobile_carrier.read
- my_reports.read_write
- nielsen.reporting_countries.read
- partner.overview.read
- partner.read
- retail.write
- right_media_offer_type.read
- seller.read
- supply_vendor.read
- supply_vendor_publisher.read
- targeting.write
- tracking_tag.read
- universal_forecasting.generate
- weather_condition.read
- ttdui_refresh
- openpath
- openpath_ui
- openpass
- ttdops
- ttd_info
- ttdapi_elevated
- manage_api_tokens
- ttd-dev-portal.access
- bidlist.read
- frequency_config.read
- datarate.read_write
- claudeai
- applications
- segment.update
- offline_access
scopes:
- description: OpenID Connect authentication.
  flows: []
  scope: openid
- description: Profile claims.
  flows: []
  scope: profile
- description: Email claim.
  flows: []
  scope: email
- description: Issue a refresh token.
  flows: []
  scope: offline_access
- description: Access to The Trade Desk Platform API.
  flows: []
  scope: ttdapi
- description: ''
  flows: []
  scope: activity.read_write
- description: ''
  flows: []
  scope: ad_format.read
- description: ''
  flows: []
  scope: ad_technology.read
- description: ''
  flows: []
  scope: adgroup.activity.read
- description: ''
  flows: []
  scope: adgroup.basic_read
- description: ''
  flows: []
  scope: adgroup.basic_update
- description: ''
  flows: []
  scope: adgroup.basic_write
- description: ''
  flows: []
  scope: adgroup.delta.read
- description: ''
  flows: []
  scope: adgroup.read_write
- description: ''
  flows: []
  scope: advertiser.delta.read
- description: ''
  flows: []
  scope: advertiser.overview.read
- description: ''
  flows: []
  scope: advertiser.read
- description: ''
  flows: []
  scope: advertiser.read_write
- description: ''
  flows: []
  scope: advertiser_targeting.read
- description: ''
  flows: []
  scope: audience.basic_read
- description: ''
  flows: []
  scope: audience_workflows.write
- description: ''
  flows: []
  scope: bidlist.basic_write
- description: ''
  flows: []
  scope: bidlist.read_write
- description: ''
  flows: []
  scope: billing_and_fees.write
- description: ''
  flows: []
  scope: campaign.activity.read
- description: ''
  flows: []
  scope: campaign.basic_read
- description: ''
  flows: []
  scope: campaign.basic_write
- description: ''
  flows: []
  scope: campaign.delta.read
- description: ''
  flows: []
  scope: campaign.read_write
- description: ''
  flows: []
  scope: campaign.write
- description: ''
  flows: []
  scope: campaign_flight.create
- description: ''
  flows: []
  scope: campaign_flight.read
- description: ''
  flows: []
  scope: category.read
- description: ''
  flows: []
  scope: category_taxonomy.read
- description: ''
  flows: []
  scope: comscore.read
- description: ''
  flows: []
  scope: content.read
- description: ''
  flows: []
  scope: contract.delta.read
- description: ''
  flows: []
  scope: contract.partner.read
- description: ''
  flows: []
  scope: contract.read_write
- description: ''
  flows: []
  scope: contract_group.read_write
- description: ''
  flows: []
  scope: creative.delta.read
- description: ''
  flows: []
  scope: creative.read
- description: ''
  flows: []
  scope: creative.read_write
- description: ''
  flows: []
  scope: creative.write
- description: ''
  flows: []
  scope: currency.read
- description: ''
  flows: []
  scope: data_group.read
- description: ''
  flows: []
  scope: delivery_profile.read
- description: ''
  flows: []
  scope: delivery_profile.read_write
- description: ''
  flows: []
  scope: delta.read
- description: ''
  flows: []
  scope: device_make_model.read
- description: ''
  flows: []
  scope: direct_url_targeting_category.read
- description: ''
  flows: []
  scope: fees.basic_write
- description: ''
  flows: []
  scope: fees.read
- description: ''
  flows: []
  scope: fees.read_write
- description: ''
  flows: []
  scope: first_party.read
- description: ''
  flows: []
  scope: frequency_counter.update
- description: ''
  flows: []
  scope: geo_segment.read
- description: ''
  flows: []
  scope: label.read_write
- description: ''
  flows: []
  scope: language.read
- description: ''
  flows: []
  scope: metadata_and_queries.write
- description: ''
  flows: []
  scope: mobile_application.read
- description: ''
  flows: []
  scope: mobile_carrier.read
- description: ''
  flows: []
  scope: my_reports.read_write
- description: ''
  flows: []
  scope: nielsen.reporting_countries.read
- description: ''
  flows: []
  scope: partner.overview.read
- description: ''
  flows: []
  scope: partner.read
- description: ''
  flows: []
  scope: retail.write
- description: ''
  flows: []
  scope: right_media_offer_type.read
- description: ''
  flows: []
  scope: seller.read
- description: ''
  flows: []
  scope: supply_vendor.read
- description: ''
  flows: []
  scope: supply_vendor_publisher.read
- description: ''
  flows: []
  scope: targeting.write
- description: ''
  flows: []
  scope: tracking_tag.read
- description: ''
  flows: []
  scope: universal_forecasting.generate
- description: ''
  flows: []
  scope: weather_condition.read
- description: Refresh the platform UI session.
  flows: []
  scope: ttdui_refresh
- description: OpenPath access.
  flows: []
  scope: openpath
- description: ''
  flows: []
  scope: openpath_ui
- description: OpenPass access.
  flows: []
  scope: openpass
- description: ''
  flows: []
  scope: ttdops
- description: ''
  flows: []
  scope: ttd_info
- description: Elevated Platform API access.
  flows: []
  scope: ttdapi_elevated
- description: Create and revoke API tokens.
  flows: []
  scope: manage_api_tokens
- description: Access to the developer portal.
  flows: []
  scope: ttd-dev-portal.access
- description: ''
  flows: []
  scope: bidlist.read
- description: ''
  flows: []
  scope: frequency_config.read
- description: ''
  flows: []
  scope: datarate.read_write
- description: ''
  flows: []
  scope: claudeai
- description: ''
  flows: []
  scope: applications
- description: ''
  flows: []
  scope: segment.update
- description: Issue a refresh token.
  flows: []
  scope: offline_access
slug: trade-desk-scopes
source_filename: trade-desk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.thetradedesk.com/.well-known/openid-configuration\ndocs: https://open.thetradedesk.com/advertiser/docsApp/Foundations/resources/doc/PlatformAuthentication\nnote: Scopes are read from The Trade Desk's live OpenID Connect discovery document, not from an OpenAPI\n  — none of the published Data API specs declare an oauth2 securityScheme. The provider does not publish\n  a scopes/permissions reference page, so descriptions are supplied only where the scope name is unambiguous;\n  the rest are recorded verbatim with no invented description.\nschemes:\n- name: OpenIDConnect\n  source: https://auth.thetradedesk.com/.well-known/openid-configuration\n  issuer: https://auth.thetradedesk.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.thetradedesk.com/connect/authorize\n    tokenUrl: https://auth.thetradedesk.com/connect/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.thetradedesk.com/connect/token\n\
  \  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.thetradedesk.com/connect/deviceauthorization\n    tokenUrl: https://auth.thetradedesk.com/connect/token\n  pkce:\n  - plain\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  - delegated\n  - urn:ietf:params:oauth:grant-type:azure-token-exchange\n  - urn:ttd:params:oauth:grant-type:service-account\nmcp_resource_scopes:\n  resource: https://api.thetradedesk.com/mcp/platform-management\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  - ttdapi\n  source: https://api.thetradedesk.com/.well-known/oauth-protected-resource/mcp/platform-management\nscope_count: 91\nscopes:\n- scope: openid\n  description: OpenID Connect authentication.\n- scope: profile\n\
  \  description: Profile claims.\n- scope: email\n  description: Email claim.\n- scope: offline_access\n  description: Issue a refresh token.\n- scope: ttdapi\n  description: Access to The Trade Desk Platform API.\n- scope: activity.read_write\n- scope: ad_format.read\n- scope: ad_technology.read\n- scope: adgroup.activity.read\n- scope: adgroup.basic_read\n- scope: adgroup.basic_update\n- scope: adgroup.basic_write\n- scope: adgroup.delta.read\n- scope: adgroup.read_write\n- scope: advertiser.delta.read\n- scope: advertiser.overview.read\n- scope: advertiser.read\n- scope: advertiser.read_write\n- scope: advertiser_targeting.read\n- scope: audience.basic_read\n- scope: audience_workflows.write\n- scope: bidlist.basic_write\n- scope: bidlist.read_write\n- scope: billing_and_fees.write\n- scope: campaign.activity.read\n- scope: campaign.basic_read\n- scope: campaign.basic_write\n- scope: campaign.delta.read\n- scope: campaign.read_write\n- scope: campaign.write\n- scope: campaign_flight.create\n\
  - scope: campaign_flight.read\n- scope: category.read\n- scope: category_taxonomy.read\n- scope: comscore.read\n- scope: content.read\n- scope: contract.delta.read\n- scope: contract.partner.read\n- scope: contract.read_write\n- scope: contract_group.read_write\n- scope: creative.delta.read\n- scope: creative.read\n- scope: creative.read_write\n- scope: creative.write\n- scope: currency.read\n- scope: data_group.read\n- scope: delivery_profile.read\n- scope: delivery_profile.read_write\n- scope: delta.read\n- scope: device_make_model.read\n- scope: direct_url_targeting_category.read\n- scope: fees.basic_write\n- scope: fees.read\n- scope: fees.read_write\n- scope: first_party.read\n- scope: frequency_counter.update\n- scope: geo_segment.read\n- scope: label.read_write\n- scope: language.read\n- scope: metadata_and_queries.write\n- scope: mobile_application.read\n- scope: mobile_carrier.read\n- scope: my_reports.read_write\n- scope: nielsen.reporting_countries.read\n- scope: partner.overview.read\n\
  - scope: partner.read\n- scope: retail.write\n- scope: right_media_offer_type.read\n- scope: seller.read\n- scope: supply_vendor.read\n- scope: supply_vendor_publisher.read\n- scope: targeting.write\n- scope: tracking_tag.read\n- scope: universal_forecasting.generate\n- scope: weather_condition.read\n- scope: ttdui_refresh\n  description: Refresh the platform UI session.\n- scope: openpath\n  description: OpenPath access.\n- scope: openpath_ui\n- scope: openpass\n  description: OpenPass access.\n- scope: ttdops\n- scope: ttd_info\n- scope: ttdapi_elevated\n  description: Elevated Platform API access.\n- scope: manage_api_tokens\n  description: Create and revoke API tokens.\n- scope: ttd-dev-portal.access\n  description: Access to the developer portal.\n- scope: bidlist.read\n- scope: frequency_config.read\n- scope: datarate.read_write\n- scope: claudeai\n- scope: applications\n- scope: segment.update\n- scope: offline_access\n  description: Issue a refresh token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trade-desk/refs/heads/main/scopes/trade-desk-scopes.yml
summary_line: 91 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Advertising
- Programmatic Advertising
- Demand-Side Platform
- DSP
- AdTech
- Connected TV
- CTV
- Identity
- Unified ID 2.0
- UID2
- OpenPath
- Kokai
- Koa AI
- Galileo
- Sincera
- Open Internet
- Real-Time Bidding
- Open Measurement
token_urls:
- https://auth.thetradedesk.com/connect/token
---
