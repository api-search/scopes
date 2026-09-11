---
api_specs:
- filename: aeris-auth-3.0-openapi.yaml
  format: yaml
  label: Aeris IoT Accelerator REST API
  slug: aeris-iot-accelerator-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/openapi/aeris-auth-3.0-openapi.yaml
- filename: aeris-sms-messaging-api-openapi.yaml
  format: yaml
  label: Aeris IoT Accelerator SMS Messaging API
  slug: aeris-iot-accelerator-sms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/openapi/aeris-sms-messaging-api-openapi.yaml
- filename: aeris-watchtower-api-openapi-openapi.yaml
  format: yaml
  label: Aeris IoT Watchtower API
  slug: aeris-iot-watchtower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/openapi/aeris-watchtower-api-openapi-openapi.yaml
authorization_urls: []
description: ''
docs:
- https://iotdeveloper.aeris.net/hc/en-us/articles/25348523998748-API-Quick-start-guide
- https://iotdeveloper.aeris.net/hc/en-us/articles/25348574275868-JWT-Authentication-Best-Practices
- https://iotdeveloper.aeris.net/hc/en-us/articles/25348572926236-Auth-API-1-0-1
flows:
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Aeris Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aeris publishes 71 OAuth 2.0 scopes via the password and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aeris API on a user''s behalf.


  Tokens are issued from /iot/api/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aeris
provider_slug: aeris
schemes:
- flows:
  - flow: password
    tokenUrl: /iot/api/auth/token
  name: Oauth2_auth
  source: openapi/aeris-business-analytics-report-api-openapi.yaml
- flows:
  - flow: password
    tokenUrl: /iot/api/auth/token
  name: Oauth2_auth
  source: openapi/aeris-business-automation-api-openapi.yaml
- flows:
  - flow: password
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: Oauth2_auth
  source: openapi/aeris-consumer-connectivity-openapi.yaml
- description: The resources in the API are protected using the OAuth 2.0 protocol
  flows:
  - flow: clientCredentials
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: OAuth2
  source: openapi/aeris-eco-operations-api-openapi.yaml
- description: The resources in the API are protected using the OAuth 2.0 protocol
  flows:
  - flow: clientCredentials
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: OAuth2
  source: openapi/aeris-eim-info-api-openapi.yaml
- description: The Enterprise API uses OAuth2 and OIDC for authentication and authorization.
  flows:
  - flow: password
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: oauth2
  source: openapi/aeris-enterprise-management-api-openapi.yaml
- description: The resources in the API are protected using the OAuth 2.0 protocol
  flows:
  - flow: clientCredentials
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: OAuth2
  source: openapi/aeris-euicc-setup-api-openapi.yaml
- description: The External Incidents API uses OAuth2 and OIDC for authentication and authorization.
  flows:
  - flow: password
    tokenUrl: /iot/api/auth/token
  name: oauth2
  source: openapi/aeris-incidents-external-api-openapi.yaml
- description: The API uses OAuth2 and OIDC for authentication and authorization.
  flows:
  - flow: password
    tokenUrl: https://<baseURL>/iot/api/auth/token
  name: oauth2
  source: openapi/aeris-operator-order-management-api-openapi.yaml
- description: The API uses OAuth2 and OIDC for authentication and authorization.
  flows:
  - flow: password
    tokenUrl: /iot/api/auth/token
  name: OAuth2
  source: openapi/aeris-organization-signaling-aggregations-api-openapi.yaml
- description: The API uses OAuth2 and OIDC for authentication and authorization.
  flows:
  - flow: password
    tokenUrl: https://<baseURL>/iot/api/auth/token
  name: oauth2
  source: openapi/aeris-resource-inventory-api-openapi.yaml
- description: The resources in the API are protected using the OAuth 2.0 protocol with the password grant flow.
  flows:
  - flow: password
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: OAuth2
  source: openapi/aeris-shared-bundle-api-openapi.yaml
- flows:
  - flow: password
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: Oauth2_auth
  source: openapi/aeris-sim-specification-management-api-openapi.yaml
- flows:
  - flow: password
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: Oauth2_auth
  source: openapi/aeris-subscription-change-history-openapi.yaml
- flows:
  - flow: password
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: Oauth2_auth
  source: openapi/aeris-subscription-custom-fields-api-openapi.yaml
- description: The resources in the API are protected using the OAuth 2.0 protocol with the password grant flow.
  flows:
  - flow: password
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: OAuth2
  source: openapi/aeris-subscription-device-api-openapi.yaml
- flows:
  - flow: password
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: Oauth2_auth
  source: openapi/aeris-subscription-device-reconnect-api-openapi.yaml
- flows:
  - flow: password
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: Oauth2_auth
  source: openapi/aeris-subscription-inventory-common-api-openapi.yaml
- flows:
  - flow: password
    tokenUrl: '/iot/api/auth/token

      '
  name: Oauth2_auth
  source: openapi/aeris-subscription-location-api-openapi.yaml
- description: The resources in the API are protected using the OAuth 2.0 protocol with the password grant flow.
  flows:
  - flow: password
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: OAuth2
  source: openapi/aeris-subscription-number-management-api-openapi.yaml
- flows:
  - flow: password
    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token
  name: Oauth2Auth
  source: openapi/aeris-subscription-search-api-openapi.yaml
- description: The resources in the API are protected using the OAuth 2.0 protocol with the password grant flow.
  flows:
  - flow: password
    tokenUrl: /iot/api/auth/token
  name: OAuth2
  source: openapi/aeris-subscription-signalling-events-api-openapi.yaml
- description: The resources in the API are protected using the OAuth 2.0 protocol with the password grant flow.
  flows:
  - flow: password
    tokenUrl: /iot/api/auth/token
  name: OAuth2
  source: openapi/aeris-subscription-signalling-usages-api-openapi.yaml
- description: This API uses OAuth 2 with the Client Credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /watchtower/v1/auth/token
  name: oAuth2ClientCredentials
  source: openapi/aeris-watchtower-api-openapi-openapi.yaml
scope_count: 71
scope_names:
- cc.read
- cc.write
- cnx_aggregated_traffic
- cnx_eim_eco_add
- cnx_eim_eco_delete
- cnx_eim_eco_update
- cnx_eim_eco_view
- cnx_eim_read
- cnx_euicc_inventory
- cnx_invoice_download
- cnx_invoice_download_2
- cnx_invoice_download_operator
- cnx_invoice_download_operator_2
- cnx_invoice_download_supplier
- cnx_log_incident_2
- cnx_manage_incidents
- cnx_report_download
- cnx_report_download_2
- cnx_report_download_no_invoice
- cnx_report_download_no_invoice_2
- cnx_report_download_opco
- cnx_report_download_opco_2
- cnx_report_download_operator
- cnx_report_download_operator_2
- cnx_search_traffic
- cnx_show_movesim_action
- cnx_ss_euicc_activationcode_man
- cnx_ss_euicc_activationcode_ro
- cnx_subscription_view
- cnx_subscription_view2
- cnx_subscriptions_view
- cnx_top_traffic_subscr_gprs
- cnx_top_traffic_subscr_sms
- cnx_traffic_analytics
- cnx_usage_data_download
- cnx_usage_data_download_2
- cnx_view_networks
- cnx_view_resources
- css_deprecate_subscription_package
- css_manage_enterprise_groups
- css_manage_enterprise_hierarchy
- css_manage_incidents_for_advanced_reseller_enterprise
- css_premium_csp_incident_for_operators
- css_view_enterprise_groups
- css_view_resources
- custom-field.read
- custom-field.write
- euicc-mgt.agreement.read
- euicc-mgt.agreement.write
- om_manage_order
- om_resource_approval
- om_service_approval
- om_view_order
- org-mgt.shared-bundle-consumption.read
- rulesets.read
- rulesets.write
- ssm.euicc-spec.read
- ssm.euicc-spec.write
- ssm.sim-spec.read
- ssm.sim-spec.write
- subscription-history.read
- subscription-service.read
- subscription-service.write
- subscription-signalling-events.read
- subscription-signalling-usages.read
- subscription.write
- sulo.cell-global-identities.read
- triggered-actions.read
- triggered-actions.write
- xdr-raw-api.read
- xdr-report-api.read
scopes:
- description: Access right needed to read from Consumer Connectivity service.
  flows:
  - password
  scope: cc.read
- description: Access right needed to write to Consumer Connectivity service.
  flows:
  - password
  scope: cc.write
- description: Access right to perform query operation.
  flows:
  - password
  scope: cnx_aggregated_traffic
- description: Grant client access to create add eCO operations
  flows:
  - clientCredentials
  scope: cnx_eim_eco_add
- description: Grant client access to create delete eCO operations
  flows:
  - clientCredentials
  scope: cnx_eim_eco_delete
- description: Grant client access to create update eCO operations
  flows:
  - clientCredentials
  scope: cnx_eim_eco_update
- description: Grant client access to create/list eCO operations and read eCO job status
  flows:
  - clientCredentials
  scope: cnx_eim_eco_view
- description: Grant client read access to eIM info resources
  flows:
  - clientCredentials
  scope: cnx_eim_read
- description: Grant user read access to device inventory resource
  flows:
  - password
  scope: cnx_euicc_inventory
- description: Download invoices - for enterprises (old)
  flows:
  - password
  scope: cnx_invoice_download
- description: Download invoices
  flows:
  - password
  scope: cnx_invoice_download_2
- description: Download invoices + invoice deletion - for operators (old)
  flows:
  - password
  scope: cnx_invoice_download_operator
- description: Download invoices + invoice deletion
  flows:
  - password
  scope: cnx_invoice_download_operator_2
- description: Download invoices + invoice deletion - for supplier
  flows:
  - password
  scope: cnx_invoice_download_supplier
- description: Grants access to view and create incidents information by operator users.
  flows:
  - password
  scope: cnx_log_incident_2
- description: Grants access to manage incidents information by operator users.
  flows:
  - password
  scope: cnx_manage_incidents
- description: Download monthly reports - for TCXN (old)
  flows:
  - password
  scope: cnx_report_download
- description: Download monthly reports - for enterprises
  flows:
  - password
  scope: cnx_report_download_2
- description: Download monthly reports (no billing-related reports) - for enterprises (old)
  flows:
  - password
  scope: cnx_report_download_no_invoice
- description: Download monthly reports (no billing-related reports) - for enterprises
  flows:
  - password
  scope: cnx_report_download_no_invoice_2
- description: Download monthly reports - for operators (old)
  flows:
  - password
  scope: cnx_report_download_opco
- description: Download monthly reports - for operators
  flows:
  - password
  scope: cnx_report_download_opco_2
- description: Download monthly reports - for TCXN (old)
  flows:
  - password
  scope: cnx_report_download_operator
- description: Download monthly reports - for TCXN
  flows:
  - password
  scope: cnx_report_download_operator_2
- description: Grant user access to subscription traffic search resource
  flows:
  - password
  scope: cnx_search_traffic
- description: Grant user access to change subscription owner
  flows:
  - password
  scope: cnx_show_movesim_action
- description: ''
  flows: []
  scope: cnx_ss_euicc_activationcode_man
- description: ''
  flows: []
  scope: cnx_ss_euicc_activationcode_ro
- description: Grant user read access to Number management inventory resource
  flows:
  - password
  scope: cnx_subscription_view
- description: Grant user access to subscription inventory resource
  flows:
  - password
  scope: cnx_subscription_view2
- description: Grant user access to subscriptions inventory resource
  flows:
  - password
  scope: cnx_subscriptions_view
- description: 'API: Subscriptions with most data traffic'
  flows:
  - password
  scope: cnx_top_traffic_subscr_gprs
- description: 'API: Subscriptions with most SMS traffic'
  flows:
  - password
  scope: cnx_top_traffic_subscr_sms
- description: Grant user read access to traffic analytics view
  flows:
  - password
  scope: cnx_traffic_analytics
- description: Download usage data (old)
  flows:
  - password
  scope: cnx_usage_data_download
- description: Download usage data
  flows:
  - password
  scope: cnx_usage_data_download_2
- description: ''
  flows: []
  scope: cnx_view_networks
- description: Access right to read APN
  flows:
  - password
  scope: cnx_view_resources
- description: ''
  flows: []
  scope: css_deprecate_subscription_package
- description: ''
  flows: []
  scope: css_manage_enterprise_groups
- description: Grants access to read, create and update enterprise and subscription package information.
  flows:
  - password
  scope: css_manage_enterprise_hierarchy
- description: Grants access to view, create and update incidents information by reseller users.
  flows:
  - password
  scope: css_manage_incidents_for_advanced_reseller_enterprise
- description: Enables premium CSPs to create VIP Incidents compared to the standard incident severity matrix
  flows:
  - password
  scope: css_premium_csp_incident_for_operators
- description: ''
  flows: []
  scope: css_view_enterprise_groups
- description: Grants access to read resource information.
  flows:
  - password
  scope: css_view_resources
- description: read custom fields
  flows:
  - password
  scope: custom-field.read
- description: create or update custom fields
  flows:
  - password
  scope: custom-field.write
- description: Grant client read access to eUICC agreement resources
  flows:
  - clientCredentials
  scope: euicc-mgt.agreement.read
- description: Grant client write access to eUICC agreement resources
  flows:
  - clientCredentials
  scope: euicc-mgt.agreement.write
- description: Manage order
  flows:
  - password
  scope: om_manage_order
- description: Approve or reject resource order
  flows:
  - password
  scope: om_resource_approval
- description: Approve or reject service order
  flows:
  - password
  scope: om_service_approval
- description: View order
  flows:
  - password
  scope: om_view_order
- description: Grant read access to shared bundle traffic consumption information.
  flows:
  - password
  scope: org-mgt.shared-bundle-consumption.read
- description: Access right to read a rulesets.
  flows:
  - password
  scope: rulesets.read
- description: Access right to write a rulesets..
  flows:
  - password
  scope: rulesets.write
- description: Read access to eUICC spec resources in SSM
  flows:
  - password
  scope: ssm.euicc-spec.read
- description: Write access to eUICC spec resources in SSM
  flows:
  - password
  scope: ssm.euicc-spec.write
- description: Read access to sim spec resources in SSM
  flows:
  - password
  scope: ssm.sim-spec.read
- description: Write access to sim spec resources in SSM
  flows:
  - password
  scope: ssm.sim-spec.write
- description: access subscription history
  flows:
  - password
  scope: subscription-history.read
- description: Access right needed to read from the Subscription service.
  flows:
  - password
  scope: subscription-service.read
- description: Access right needed to write to the Subscription service.
  flows:
  - password
  scope: subscription-service.write
- description: Grant read access to listing subscription signalling events.
  flows:
  - password
  scope: subscription-signalling-events.read
- description: Grant read access to subscription signalling usages API.
  flows:
  - password
  scope: subscription-signalling-usages.read
- description: update subscription
  flows:
  - password
  scope: subscription.write
- description: Access cell global identity
  flows:
  - password
  scope: sulo.cell-global-identities.read
- description: Access right to read a triggered action.
  flows:
  - password
  scope: triggered-actions.read
- description: Access right to write a triggered action.
  flows:
  - password
  scope: triggered-actions.write
- description: Grant read access to listing signalling events.
  flows:
  - password
  scope: xdr-raw-api.read
- description: Grant read access to usage reports.
  flows:
  - password
  scope: xdr-report-api.read
slug: aeris-scopes
source_filename: aeris-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: openapi/aeris-business-analytics-report-api-openapi.yaml, openapi/aeris-business-automation-api-openapi.yaml,\n  openapi/aeris-consumer-connectivity-openapi.yaml, openapi/aeris-eco-operations-api-openapi.yaml, openapi/aeris-eim-info-api-openapi.yaml,\n  openapi/aeris-enterprise-management-api-openapi.yaml, openapi/aeris-euicc-setup-api-openapi.yaml, openapi/aeris-incidents-external-api-openapi.yaml,\n  openapi/aeris-operator-order-management-api-openapi.yaml, openapi/aeris-organization-signaling-aggregations-api-openapi.yaml,\n  openapi/aeris-resource-inventory-api-openapi.yaml, openapi/aeris-shared-bundle-api-openapi.yaml, openapi/aeris-sim-specification-management-api-openapi.yaml,\n  openapi/aeris-subscription-change-history-openapi.yaml, openapi/aeris-subscription-custom-fields-api-openapi.yaml,\n  openapi/aeris-subscription-device-api-openapi.yaml, openapi/aeris-subscription-device-reconnect-api-openapi.yaml,\n  openapi/aeris-subscription-inventory-common-api-openapi.yaml,\
  \ openapi/aeris-subscription-location-api-openapi.yaml,\n  openapi/aeris-subscription-number-management-api-openapi.yaml, openapi/aeris-subscription-search-api-openapi.yaml,\n  openapi/aeris-subscription-signalling-events-api-openapi.yaml, openapi/aeris-subscription-signalling-usages-api-openapi.yaml,\n  openapi/aeris-watchtower-api-openapi-openapi.yaml — upgraded from the Aeris IoT Developer Portal API Quick start\n  guide, which publishes the authentication mechanism used by each API group.\nschemes:\n- name: Oauth2_auth\n  source: openapi/aeris-business-analytics-report-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: /iot/api/auth/token\n- name: Oauth2_auth\n  source: openapi/aeris-business-automation-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: /iot/api/auth/token\n- name: Oauth2_auth\n  source: openapi/aeris-consumer-connectivity-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n- name: OAuth2\n \
  \ source: openapi/aeris-eco-operations-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n  description: The resources in the API are protected using the OAuth 2.0 protocol\n- name: OAuth2\n  source: openapi/aeris-eim-info-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n  description: The resources in the API are protected using the OAuth 2.0 protocol\n- name: oauth2\n  source: openapi/aeris-enterprise-management-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n  description: The Enterprise API uses OAuth2 and OIDC for authentication and authorization.\n- name: OAuth2\n  source: openapi/aeris-euicc-setup-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n  description: The resources in the API are protected using the OAuth 2.0 protocol\n\
  - name: oauth2\n  source: openapi/aeris-incidents-external-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: /iot/api/auth/token\n  description: The External Incidents API uses OAuth2 and OIDC for authentication and authorization.\n- name: oauth2\n  source: openapi/aeris-operator-order-management-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://<baseURL>/iot/api/auth/token\n  description: The API uses OAuth2 and OIDC for authentication and authorization.\n- name: OAuth2\n  source: openapi/aeris-organization-signaling-aggregations-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: /iot/api/auth/token\n  description: The API uses OAuth2 and OIDC for authentication and authorization.\n- name: oauth2\n  source: openapi/aeris-resource-inventory-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://<baseURL>/iot/api/auth/token\n  description: The API uses OAuth2 and OIDC for authentication and authorization.\n- name: OAuth2\n  source:\
  \ openapi/aeris-shared-bundle-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n  description: The resources in the API are protected using the OAuth 2.0 protocol with the password grant flow.\n- name: Oauth2_auth\n  source: openapi/aeris-sim-specification-management-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n- name: Oauth2_auth\n  source: openapi/aeris-subscription-change-history-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n- name: Oauth2_auth\n  source: openapi/aeris-subscription-custom-fields-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n- name: OAuth2\n  source: openapi/aeris-subscription-device-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n  description: The resources in the API are\
  \ protected using the OAuth 2.0 protocol with the password grant flow.\n- name: Oauth2_auth\n  source: openapi/aeris-subscription-device-reconnect-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n- name: Oauth2_auth\n  source: openapi/aeris-subscription-inventory-common-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n- name: Oauth2_auth\n  source: openapi/aeris-subscription-location-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: '/iot/api/auth/token\n\n      '\n- name: OAuth2\n  source: openapi/aeris-subscription-number-management-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n  description: The resources in the API are protected using the OAuth 2.0 protocol with the password grant flow.\n- name: Oauth2Auth\n  source: openapi/aeris-subscription-search-api-openapi.yaml\n  flows:\n  - flow: password\n\
  \    tokenUrl: https://iot-api.aeris.com/iot/api/auth/token\n- name: OAuth2\n  source: openapi/aeris-subscription-signalling-events-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: /iot/api/auth/token\n  description: The resources in the API are protected using the OAuth 2.0 protocol with the password grant flow.\n- name: OAuth2\n  source: openapi/aeris-subscription-signalling-usages-api-openapi.yaml\n  flows:\n  - flow: password\n    tokenUrl: /iot/api/auth/token\n  description: The resources in the API are protected using the OAuth 2.0 protocol with the password grant flow.\n- name: oAuth2ClientCredentials\n  source: openapi/aeris-watchtower-api-openapi-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /watchtower/v1/auth/token\n  description: This API uses OAuth 2 with the Client Credentials flow.\nscopes:\n- scope: cc.read\n  description: Access right needed to read from Consumer Connectivity service.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-consumer-connectivity-openapi.yaml\n\
  - scope: cc.write\n  description: Access right needed to write to Consumer Connectivity service.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-consumer-connectivity-openapi.yaml\n- scope: cnx_aggregated_traffic\n  description: Access right to perform query operation.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-organization-signaling-aggregations-api-openapi.yaml\n- scope: cnx_eim_eco_add\n  description: Grant client access to create add eCO operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aeris-eco-operations-api-openapi.yaml\n- scope: cnx_eim_eco_delete\n  description: Grant client access to create delete eCO operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aeris-eco-operations-api-openapi.yaml\n- scope: cnx_eim_eco_update\n  description: Grant client access to create update eCO operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aeris-eco-operations-api-openapi.yaml\n- scope: cnx_eim_eco_view\n  description:\
  \ Grant client access to create/list eCO operations and read eCO job status\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aeris-eco-operations-api-openapi.yaml\n- scope: cnx_eim_read\n  description: Grant client read access to eIM info resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aeris-eim-info-api-openapi.yaml\n- scope: cnx_euicc_inventory\n  description: Grant user read access to device inventory resource\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-device-api-openapi.yaml\n- scope: cnx_invoice_download\n  description: Download invoices - for enterprises (old)\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_invoice_download_2\n  description: Download invoices\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_invoice_download_operator\n  description: Download invoices + invoice deletion - for operators (old)\n\
  \  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_invoice_download_operator_2\n  description: Download invoices + invoice deletion\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_invoice_download_supplier\n  description: Download invoices + invoice deletion - for supplier\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_log_incident_2\n  description: Grants access to view and create incidents information by operator users.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-incidents-external-api-openapi.yaml\n- scope: cnx_manage_incidents\n  description: Grants access to manage incidents information by operator users.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-incidents-external-api-openapi.yaml\n- scope: cnx_report_download\n  description: Download monthly reports - for TCXN (old)\n\
  \  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_report_download_2\n  description: Download monthly reports - for enterprises\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_report_download_no_invoice\n  description: Download monthly reports (no billing-related reports) - for enterprises (old)\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_report_download_no_invoice_2\n  description: Download monthly reports (no billing-related reports) - for enterprises\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_report_download_opco\n  description: Download monthly reports - for operators (old)\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_report_download_opco_2\n  description: Download\
  \ monthly reports - for operators\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_report_download_operator\n  description: Download monthly reports - for TCXN (old)\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_report_download_operator_2\n  description: Download monthly reports - for TCXN\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_search_traffic\n  description: Grant user access to subscription traffic search resource\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-device-api-openapi.yaml\n- scope: cnx_show_movesim_action\n  description: Grant user access to change subscription owner\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-device-api-openapi.yaml\n- scope: cnx_ss_euicc_activationcode_man\n  sources:\n  - openapi/aeris-euicc-setup-api-openapi.yaml\n\
  - scope: cnx_ss_euicc_activationcode_ro\n  sources:\n  - openapi/aeris-euicc-setup-api-openapi.yaml\n- scope: cnx_subscription_view\n  description: Grant user read access to Number management inventory resource\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-number-management-api-openapi.yaml\n- scope: cnx_subscription_view2\n  description: Grant user access to subscription inventory resource\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-device-api-openapi.yaml\n- scope: cnx_subscriptions_view\n  description: Grant user access to subscriptions inventory resource\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-device-api-openapi.yaml\n- scope: cnx_top_traffic_subscr_gprs\n  description: 'API: Subscriptions with most data traffic'\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_top_traffic_subscr_sms\n  description: 'API: Subscriptions with most SMS traffic'\n  flows:\n\
  \  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_traffic_analytics\n  description: Grant user read access to traffic analytics view\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-device-api-openapi.yaml\n- scope: cnx_usage_data_download\n  description: Download usage data (old)\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_usage_data_download_2\n  description: Download usage data\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-analytics-report-api-openapi.yaml\n- scope: cnx_view_networks\n  sources:\n  - openapi/aeris-resource-inventory-api-openapi.yaml\n- scope: cnx_view_resources\n  description: Access right to read APN\n  flows:\n  - password\n  sources:\n  - openapi/aeris-resource-inventory-api-openapi.yaml\n- scope: css_deprecate_subscription_package\n  sources:\n  - openapi/aeris-enterprise-management-api-openapi.yaml\n- scope:\
  \ css_manage_enterprise_groups\n  sources:\n  - openapi/aeris-enterprise-management-api-openapi.yaml\n- scope: css_manage_enterprise_hierarchy\n  description: Grants access to read, create and update enterprise and subscription package information.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-enterprise-management-api-openapi.yaml\n- scope: css_manage_incidents_for_advanced_reseller_enterprise\n  description: Grants access to view, create and update incidents information by reseller users.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-incidents-external-api-openapi.yaml\n- scope: css_premium_csp_incident_for_operators\n  description: Enables premium CSPs to create VIP Incidents compared to the standard incident severity matrix\n  flows:\n  - password\n  sources:\n  - openapi/aeris-incidents-external-api-openapi.yaml\n- scope: css_view_enterprise_groups\n  sources:\n  - openapi/aeris-enterprise-management-api-openapi.yaml\n- scope: css_view_resources\n  description: Grants\
  \ access to read resource information.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-enterprise-management-api-openapi.yaml\n- scope: custom-field.read\n  description: read custom fields\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-custom-fields-api-openapi.yaml\n- scope: custom-field.write\n  description: create or update custom fields\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-custom-fields-api-openapi.yaml\n- scope: euicc-mgt.agreement.read\n  description: Grant client read access to eUICC agreement resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aeris-euicc-setup-api-openapi.yaml\n- scope: euicc-mgt.agreement.write\n  description: Grant client write access to eUICC agreement resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aeris-euicc-setup-api-openapi.yaml\n- scope: om_manage_order\n  description: Manage order\n  flows:\n  - password\n  sources:\n  - openapi/aeris-operator-order-management-api-openapi.yaml\n\
  - scope: om_resource_approval\n  description: Approve or reject resource order\n  flows:\n  - password\n  sources:\n  - openapi/aeris-operator-order-management-api-openapi.yaml\n- scope: om_service_approval\n  description: Approve or reject service order\n  flows:\n  - password\n  sources:\n  - openapi/aeris-operator-order-management-api-openapi.yaml\n- scope: om_view_order\n  description: View order\n  flows:\n  - password\n  sources:\n  - openapi/aeris-operator-order-management-api-openapi.yaml\n- scope: org-mgt.shared-bundle-consumption.read\n  description: Grant read access to shared bundle traffic consumption information.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-shared-bundle-api-openapi.yaml\n- scope: rulesets.read\n  description: Access right to read a rulesets.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-automation-api-openapi.yaml\n- scope: rulesets.write\n  description: Access right to write a rulesets..\n  flows:\n  - password\n  sources:\n\
  \  - openapi/aeris-business-automation-api-openapi.yaml\n- scope: ssm.euicc-spec.read\n  description: Read access to eUICC spec resources in SSM\n  flows:\n  - password\n  sources:\n  - openapi/aeris-sim-specification-management-api-openapi.yaml\n- scope: ssm.euicc-spec.write\n  description: Write access to eUICC spec resources in SSM\n  flows:\n  - password\n  sources:\n  - openapi/aeris-sim-specification-management-api-openapi.yaml\n- scope: ssm.sim-spec.read\n  description: Read access to sim spec resources in SSM\n  flows:\n  - password\n  sources:\n  - openapi/aeris-sim-specification-management-api-openapi.yaml\n- scope: ssm.sim-spec.write\n  description: Write access to sim spec resources in SSM\n  flows:\n  - password\n  sources:\n  - openapi/aeris-sim-specification-management-api-openapi.yaml\n- scope: subscription-history.read\n  description: access subscription history\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-change-history-openapi.yaml\n- scope: subscription-service.read\n\
  \  description: Access right needed to read from the Subscription service.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-device-reconnect-api-openapi.yaml\n  - openapi/aeris-subscription-inventory-common-api-openapi.yaml\n  - openapi/aeris-subscription-search-api-openapi.yaml\n- scope: subscription-service.write\n  description: Access right needed to write to the Subscription service.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-device-reconnect-api-openapi.yaml\n  - openapi/aeris-subscription-inventory-common-api-openapi.yaml\n  - openapi/aeris-subscription-search-api-openapi.yaml\n- scope: subscription-signalling-events.read\n  description: Grant read access to listing subscription signalling events.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-signalling-events-api-openapi.yaml\n- scope: subscription-signalling-usages.read\n  description: Grant read access to subscription signalling usages API.\n  flows:\n  - password\n\
  \  sources:\n  - openapi/aeris-subscription-signalling-usages-api-openapi.yaml\n- scope: subscription.write\n  description: update subscription\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-custom-fields-api-openapi.yaml\n- scope: sulo.cell-global-identities.read\n  description: Access cell global identity\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-location-api-openapi.yaml\n- scope: triggered-actions.read\n  description: Access right to read a triggered action.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-automation-api-openapi.yaml\n- scope: triggered-actions.write\n  description: Access right to write a triggered action.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-business-automation-api-openapi.yaml\n- scope: xdr-raw-api.read\n  description: Grant read access to listing signalling events.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-signalling-events-api-openapi.yaml\n- scope: xdr-report-api.read\n\
  \  description: Grant read access to usage reports.\n  flows:\n  - password\n  sources:\n  - openapi/aeris-subscription-signalling-usages-api-openapi.yaml\ndocs:\n- https://iotdeveloper.aeris.net/hc/en-us/articles/25348523998748-API-Quick-start-guide\n- https://iotdeveloper.aeris.net/hc/en-us/articles/25348574275868-JWT-Authentication-Best-Practices\n- https://iotdeveloper.aeris.net/hc/en-us/articles/25348572926236-Auth-API-1-0-1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeris/refs/heads/main/scopes/aeris-scopes.yml
summary_line: 71 scopes · password/clientCredentials
tags:
- IoT
- Cellular Connectivity
- M2M
- eSIM
- SIM Management
- Telecom
- Device Management
- IoT Security
- Connectivity Management Platform
- SMS Messaging
- eUICC
- Fleet Telematics
token_urls:
- /iot/api/auth/token
- https://iot-api.aeris.com/iot/api/auth/token
- https://<baseURL>/iot/api/auth/token
- '/iot/api/auth/token

  '
- /watchtower/v1/auth/token
---
