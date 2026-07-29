---
api_specs:
- filename: edf-energy-kraken-openapi.yml
  format: yaml
  label: EDF Kraken REST API
  slug: edf-kraken-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-kraken-openapi.yml
- filename: edf-energy-kraken-data-import-openapi.yml
  format: yaml
  label: EDF Kraken Customer Migration (Data Import) API
  slug: edf-kraken-customer-migration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-kraken-data-import-openapi.yml
authorization_urls:
- https://auth.edfgb-kraken.energy/authorize/
description: 'The OAuth 2.0 / OpenID Connect scope surface of the EDF GB Kraken authorisation server. Harvested verbatim from the anonymously served OpenID Provider Metadata document (HTTP 200, 2026-07-27) at auth.edfgb-kraken.energy, which advertises 111 scopes_supported. Scope grammar is verb:resource (query:, view:, create:, update:, manage:, cancel:, request:, change:, set:, add:, join:, edit:, verify:, configure:, accept:, register:, delete:, revoke:), plus the two coarse scopes openid and full-customer-access. There is no separate published scope-reference page: the discovery document is the reference. Scopes are granted to an OAuth application by EDF/Kraken on request — the auth server''s own getting-started text states an application must be requested by contacting them with the client type, grant type, redirect URIs and the resources it needs.'
docs: https://auth.edfgb-kraken.energy/
flows:
- authorizationCode
- clientCredentials
- deviceCode
- tokenExchange
kind: oauth-scopes
layout: scope
method: searched
name: Edf Energy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EDF Energy publishes 111 OAuth 2.0 scopes via the authorizationCode, clientCredentials, deviceCode, and tokenExchange flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the EDF Energy API on a user''s behalf.


  Tokens are issued from https://auth.edfgb-kraken.energy/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EDF Energy
provider_slug: edf-energy
schemes:
- flows:
  - authorizationUrl: https://auth.edfgb-kraken.energy/authorize/
    flow: authorizationCode
    pkce: true
    tokenUrl: https://auth.edfgb-kraken.energy/token/
  - flow: clientCredentials
    tokenUrl: https://auth.edfgb-kraken.energy/token/
  - deviceAuthorizationUrl: https://auth.edfgb-kraken.energy/device-authorization/
    flow: deviceCode
    tokenUrl: https://auth.edfgb-kraken.energy/token/
  - flow: tokenExchange
    rfc: RFC 8693
    tokenUrl: https://auth.edfgb-kraken.energy/token/
  name: KrakenOAuth2
  source: https://auth.edfgb-kraken.energy/.well-known/openid-configuration
scope_count: 111
scope_names:
- openid
- full-customer-access
- update:reading-consent-granularity
- create:payment-method-action-intents
- query:property-meters
- create:payment-action-intents
- query:property
- cancel:siteworks-appointments
- update:smart-meter-data-preferences
- join:campaigns
- change:centrepay-deductions
- update:sensitive-customer-information
- query:loyalty-points-balance
- query:user-details
- update:dd-amount
- query:account-campaigns
- query:auto-topup-config
- query:account-payments
- view:smartflex-data
- query:customer-flexibility-campaigns
- query:complaints
- create:quoting-offer-group
- manage:payment-schedules
- add:credit-to-smart-meter
- query:authorized-applications
- query:agreements
- create:goods-quotes
- query:portfolios
- query:fit-schedules
- query:fit-installations
- query:account-applications
- query:payment-instructions
- update:dd-day
- create:complaints
- configure:auto-topup-config
- cancel:enrollment
- create:payment-instructions
- cancel:centrepay-deductions
- query:lifecycle-processes
- manage:contribution-agreements
- query:businesses
- update:user-details
- manage:ink-live-chat
- query:loyalty-enrollment-eligibility
- edit:customer-marketing-preference
- set:loyalty-points-user
- view:account-type
- query:customer-assets
- create:property
- query:loyalty-points-ledger-entry
- query:contribution-agreements
- query:devices
- view:customer-marketing-preference
- accept:fit-terms-and-conditions
- verify:customer-details
- manage:customer-assets
- query:mfa-device
- register:smartflex-devices
- manage:account-renewals
- update:ssd
- add:campaign-to-account
- submit:fit-meter-readings
- update:smart-meter-interest
- query:electricity-meter-point-details
- join:campaign-events
- view:detailed-usage
- view:api-key
- amend:payments
- access:customer-queries
- send:loss-objection-for-change-of-supplier
- query:goods-products
- transfer:loyalty-points
- update:account-details
- query:personally-identifiable-information
- create:customer-feedback
- manage:ev
- view:customer-communications
- view:account-user-permissions
- view:ev-data
- checkout:quote
- query:goods-quotes
- redeem:loyalty-points
- process:move-outs
- initiate:standalone-payments
- occupy:accounts
- view:sensitive-customer-information
- view:account-number
- query:billing-information
- delete:mfa-device
- accept:fit-schedules
- book:smart-meter-appointments
- accept:terms-and-conditions
- review:quote
- query:establishments
- manage:goods-purchases
- provide:missing-meter-point-details
- report:move-out
- manage:product-enrolment
- validate:mfa-device
- create:centrepay-deductions
- query:workflows
- view:campaign-dashboards
- create:mfa-device
- query:payment-preferences
- submit:customer-feedback
- submit:meter-readings
- request:consumption-data
- query:account-reminders
- query:contracts
- create:repayment-request
- escalate:ink-conversation
scopes:
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: full-customer-access
- description: ''
  flows: []
  scope: update:reading-consent-granularity
- description: ''
  flows: []
  scope: create:payment-method-action-intents
- description: ''
  flows: []
  scope: query:property-meters
- description: ''
  flows: []
  scope: create:payment-action-intents
- description: ''
  flows: []
  scope: query:property
- description: ''
  flows: []
  scope: cancel:siteworks-appointments
- description: ''
  flows: []
  scope: update:smart-meter-data-preferences
- description: ''
  flows: []
  scope: join:campaigns
- description: ''
  flows: []
  scope: change:centrepay-deductions
- description: ''
  flows: []
  scope: update:sensitive-customer-information
- description: ''
  flows: []
  scope: query:loyalty-points-balance
- description: ''
  flows: []
  scope: query:user-details
- description: ''
  flows: []
  scope: update:dd-amount
- description: ''
  flows: []
  scope: query:account-campaigns
- description: ''
  flows: []
  scope: query:auto-topup-config
- description: ''
  flows: []
  scope: query:account-payments
- description: ''
  flows: []
  scope: view:smartflex-data
- description: ''
  flows: []
  scope: query:customer-flexibility-campaigns
- description: ''
  flows: []
  scope: query:complaints
- description: ''
  flows: []
  scope: create:quoting-offer-group
- description: ''
  flows: []
  scope: manage:payment-schedules
- description: ''
  flows: []
  scope: add:credit-to-smart-meter
- description: ''
  flows: []
  scope: query:authorized-applications
- description: ''
  flows: []
  scope: query:agreements
- description: ''
  flows: []
  scope: create:goods-quotes
- description: ''
  flows: []
  scope: query:portfolios
- description: ''
  flows: []
  scope: query:fit-schedules
- description: ''
  flows: []
  scope: query:fit-installations
- description: ''
  flows: []
  scope: query:account-applications
- description: ''
  flows: []
  scope: query:payment-instructions
- description: ''
  flows: []
  scope: update:dd-day
- description: ''
  flows: []
  scope: create:complaints
- description: ''
  flows: []
  scope: configure:auto-topup-config
- description: ''
  flows: []
  scope: cancel:enrollment
- description: ''
  flows: []
  scope: create:payment-instructions
- description: ''
  flows: []
  scope: cancel:centrepay-deductions
- description: ''
  flows: []
  scope: query:lifecycle-processes
- description: ''
  flows: []
  scope: manage:contribution-agreements
- description: ''
  flows: []
  scope: query:businesses
- description: ''
  flows: []
  scope: update:user-details
- description: ''
  flows: []
  scope: manage:ink-live-chat
- description: ''
  flows: []
  scope: query:loyalty-enrollment-eligibility
- description: ''
  flows: []
  scope: edit:customer-marketing-preference
- description: ''
  flows: []
  scope: set:loyalty-points-user
- description: ''
  flows: []
  scope: view:account-type
- description: ''
  flows: []
  scope: query:customer-assets
- description: ''
  flows: []
  scope: create:property
- description: ''
  flows: []
  scope: query:loyalty-points-ledger-entry
- description: ''
  flows: []
  scope: query:contribution-agreements
- description: ''
  flows: []
  scope: query:devices
- description: ''
  flows: []
  scope: view:customer-marketing-preference
- description: ''
  flows: []
  scope: accept:fit-terms-and-conditions
- description: ''
  flows: []
  scope: verify:customer-details
- description: ''
  flows: []
  scope: manage:customer-assets
- description: ''
  flows: []
  scope: query:mfa-device
- description: ''
  flows: []
  scope: register:smartflex-devices
- description: ''
  flows: []
  scope: manage:account-renewals
- description: ''
  flows: []
  scope: update:ssd
- description: ''
  flows: []
  scope: add:campaign-to-account
- description: ''
  flows: []
  scope: submit:fit-meter-readings
- description: ''
  flows: []
  scope: update:smart-meter-interest
- description: ''
  flows: []
  scope: query:electricity-meter-point-details
- description: ''
  flows: []
  scope: join:campaign-events
- description: ''
  flows: []
  scope: view:detailed-usage
- description: ''
  flows: []
  scope: view:api-key
- description: ''
  flows: []
  scope: amend:payments
- description: ''
  flows: []
  scope: access:customer-queries
- description: ''
  flows: []
  scope: send:loss-objection-for-change-of-supplier
- description: ''
  flows: []
  scope: query:goods-products
- description: ''
  flows: []
  scope: transfer:loyalty-points
- description: ''
  flows: []
  scope: update:account-details
- description: ''
  flows: []
  scope: query:personally-identifiable-information
- description: ''
  flows: []
  scope: create:customer-feedback
- description: ''
  flows: []
  scope: manage:ev
- description: ''
  flows: []
  scope: view:customer-communications
- description: ''
  flows: []
  scope: view:account-user-permissions
- description: ''
  flows: []
  scope: view:ev-data
- description: ''
  flows: []
  scope: checkout:quote
- description: ''
  flows: []
  scope: query:goods-quotes
- description: ''
  flows: []
  scope: redeem:loyalty-points
- description: ''
  flows: []
  scope: process:move-outs
- description: ''
  flows: []
  scope: initiate:standalone-payments
- description: ''
  flows: []
  scope: occupy:accounts
- description: ''
  flows: []
  scope: view:sensitive-customer-information
- description: ''
  flows: []
  scope: view:account-number
- description: ''
  flows: []
  scope: query:billing-information
- description: ''
  flows: []
  scope: delete:mfa-device
- description: ''
  flows: []
  scope: accept:fit-schedules
- description: ''
  flows: []
  scope: book:smart-meter-appointments
- description: ''
  flows: []
  scope: accept:terms-and-conditions
- description: ''
  flows: []
  scope: review:quote
- description: ''
  flows: []
  scope: query:establishments
- description: ''
  flows: []
  scope: manage:goods-purchases
- description: ''
  flows: []
  scope: provide:missing-meter-point-details
- description: ''
  flows: []
  scope: report:move-out
- description: ''
  flows: []
  scope: manage:product-enrolment
- description: ''
  flows: []
  scope: validate:mfa-device
- description: ''
  flows: []
  scope: create:centrepay-deductions
- description: ''
  flows: []
  scope: query:workflows
- description: ''
  flows: []
  scope: view:campaign-dashboards
- description: ''
  flows: []
  scope: create:mfa-device
- description: ''
  flows: []
  scope: query:payment-preferences
- description: ''
  flows: []
  scope: submit:customer-feedback
- description: ''
  flows: []
  scope: submit:meter-readings
- description: ''
  flows: []
  scope: request:consumption-data
- description: ''
  flows: []
  scope: query:account-reminders
- description: ''
  flows: []
  scope: query:contracts
- description: ''
  flows: []
  scope: create:repayment-request
- description: ''
  flows: []
  scope: escalate:ink-conversation
slug: edf-energy-scopes
source_filename: edf-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://auth.edfgb-kraken.energy/.well-known/openid-configuration\ndocs: https://auth.edfgb-kraken.energy/\ndescription: >-\n  The OAuth 2.0 / OpenID Connect scope surface of the EDF GB Kraken authorisation\n  server. Harvested verbatim from the anonymously served OpenID Provider Metadata\n  document (HTTP 200, 2026-07-27) at auth.edfgb-kraken.energy, which advertises 111\n  scopes_supported. Scope grammar is verb:resource (query:, view:, create:, update:,\n  manage:, cancel:, request:, change:, set:, add:, join:, edit:, verify:, configure:,\n  accept:, register:, delete:, revoke:), plus the two coarse scopes openid and\n  full-customer-access. There is no separate published scope-reference page: the\n  discovery document is the reference. Scopes are granted to an OAuth application by\n  EDF/Kraken on request — the auth server's own getting-started text states an\n  application must be requested by contacting them with the\
  \ client type, grant type,\n  redirect URIs and the resources it needs.\nissuer: https://auth.edfgb-kraken.energy/token/\nschemes:\n- name: KrakenOAuth2\n  source: https://auth.edfgb-kraken.energy/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    pkce: true\n    authorizationUrl: https://auth.edfgb-kraken.energy/authorize/\n    tokenUrl: https://auth.edfgb-kraken.energy/token/\n  - flow: clientCredentials\n    tokenUrl: https://auth.edfgb-kraken.energy/token/\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.edfgb-kraken.energy/device-authorization/\n    tokenUrl: https://auth.edfgb-kraken.energy/token/\n  - flow: tokenExchange\n    tokenUrl: https://auth.edfgb-kraken.energy/token/\n    rfc: RFC 8693\nscope_count: 111\nscopes:\n- scope: \"openid\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"full-customer-access\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope:\
  \ \"update:reading-consent-granularity\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"create:payment-method-action-intents\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:property-meters\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"create:payment-action-intents\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:property\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"cancel:siteworks-appointments\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"update:smart-meter-data-preferences\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"join:campaigns\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"change:centrepay-deductions\"\
  \n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"update:sensitive-customer-information\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:loyalty-points-balance\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:user-details\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"update:dd-amount\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:account-campaigns\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:auto-topup-config\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:account-payments\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"view:smartflex-data\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n\
  - scope: \"query:customer-flexibility-campaigns\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:complaints\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"create:quoting-offer-group\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"manage:payment-schedules\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"add:credit-to-smart-meter\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:authorized-applications\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:agreements\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"create:goods-quotes\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:portfolios\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n\
  - scope: \"query:fit-schedules\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:fit-installations\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:account-applications\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:payment-instructions\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"update:dd-day\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"create:complaints\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"configure:auto-topup-config\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"cancel:enrollment\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"create:payment-instructions\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n\
  - scope: \"cancel:centrepay-deductions\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:lifecycle-processes\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"manage:contribution-agreements\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:businesses\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"update:user-details\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"manage:ink-live-chat\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:loyalty-enrollment-eligibility\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"edit:customer-marketing-preference\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"set:loyalty-points-user\"\
  \n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"view:account-type\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:customer-assets\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"create:property\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:loyalty-points-ledger-entry\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:contribution-agreements\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:devices\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"view:customer-marketing-preference\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"accept:fit-terms-and-conditions\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n\
  - scope: \"verify:customer-details\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"manage:customer-assets\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:mfa-device\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"register:smartflex-devices\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"manage:account-renewals\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"update:ssd\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"add:campaign-to-account\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"submit:fit-meter-readings\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"update:smart-meter-interest\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n\
  - scope: \"query:electricity-meter-point-details\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"join:campaign-events\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"view:detailed-usage\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"view:api-key\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"amend:payments\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"access:customer-queries\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"send:loss-objection-for-change-of-supplier\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:goods-products\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"transfer:loyalty-points\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n\
  - scope: \"update:account-details\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:personally-identifiable-information\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"create:customer-feedback\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"manage:ev\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"view:customer-communications\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"view:account-user-permissions\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"view:ev-data\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"checkout:quote\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:goods-quotes\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n\
  - scope: \"redeem:loyalty-points\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"process:move-outs\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"initiate:standalone-payments\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"occupy:accounts\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"view:sensitive-customer-information\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"view:account-number\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:billing-information\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"delete:mfa-device\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"accept:fit-schedules\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n\
  - scope: \"book:smart-meter-appointments\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"accept:terms-and-conditions\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"review:quote\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:establishments\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"manage:goods-purchases\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"provide:missing-meter-point-details\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"report:move-out\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"manage:product-enrolment\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"validate:mfa-device\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n\
  - scope: \"create:centrepay-deductions\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:workflows\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"view:campaign-dashboards\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"create:mfa-device\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:payment-preferences\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"submit:customer-feedback\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"submit:meter-readings\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"request:consumption-data\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"query:account-reminders\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n\
  - scope: \"query:contracts\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"create:repayment-request\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n- scope: \"escalate:ink-conversation\"\n  sources: [https://auth.edfgb-kraken.energy/.well-known/openid-configuration]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/scopes/edf-energy-scopes.yml
summary_line: 111 scopes · authorizationCode/clientCredentials/deviceCode/tokenExchange
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Energy Retailer
- Energy Supplier
- Smart Metering
- Nuclear
- Renewables
- EV Charging
- Demand Response
- Tariffs
- Energy Markets
token_urls:
- https://auth.edfgb-kraken.energy/token/
---
