---
api_specs:
- filename: consumer-data-standards-energy-api-openapi.json
  format: json
  label: Origin Energy CDR Energy API
  slug: origin-energy-cdr-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/consumer-data-standards-energy-api-openapi.json
- filename: consumer-data-standards-common-api-openapi.json
  format: json
  label: Origin Energy CDR Public Discovery API
  slug: origin-energy-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/consumer-data-standards-common-api-openapi.json
- filename: consumer-data-standards-energy-api-openapi.json
  format: json
  label: Origin Energy Plan Reference Data API (AER Energy Made Easy)
  slug: origin-energy-plan-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/consumer-data-standards-energy-api-openapi.json
- filename: origin-energy-kraken-default-openapi.yml
  format: yaml
  label: Origin Energy Kraken REST API
  slug: origin-energy-kraken-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/origin-energy-kraken-default-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.origin-kraken.energy/graphql/guides/basics/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Origin Energy Scopes
name_suffix: OAuth Scopes
note: Harvested verbatim from the Kraken authorisation server's OpenID Connect discovery document (HTTP 200, anonymous, 2026-07-27). The Kraken OpenAPI documents declare only apiKey/basic security schemes and no oauth2 flows, so these scopes cannot be derived from the specs — they exist only in the discovery document. Scopes are enforced on the GraphQL and REST surfaces behind the same bearer token. The Consumer Data Right surface uses the separate CDR consent scopes defined by the Data Standards Body, not these.
overview: 'Origin Energy publishes 113 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Origin Energy API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Origin Energy
provider_slug: origin-energy
schemes:
- authorizationUrl: https://auth.origin-kraken.energy/authorize/
  discovery: https://auth.origin-kraken.energy/.well-known/openid-configuration
  dynamic_client_registration: false
  endSessionUrl: https://auth.origin-kraken.energy/logout/
  issuer: https://auth.origin-kraken.energy/token/
  jwksUrl: https://auth.origin-kraken.energy/.well-known/jwks.json
  name: Kraken OpenID Connect
  pkce_methods_advertised: false
  response_types_supported:
  - code
  - token
  - id_token
  - id_token token
  - code token
  - code id_token
  - code id_token token
  revocationUrl: https://auth.origin-kraken.energy/revoke-token/
  tokenUrl: https://auth.origin-kraken.energy/token/
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
  userinfoUrl: https://auth.origin-kraken.energy/userinfo/
scope_count: 113
scope_names:
- openid
- full-customer-access
- create:payment-method-action-intents
- change:centrepay-deductions
- query:agreements
- view:smartflex-data
- amend:payments
- query:customer-flexibility-campaigns
- query:goods-products
- query:loyalty-enrollment-eligibility
- query:workflows
- query:fit-installations
- create:goods-quotes
- query:contribution-agreements
- configure:auto-topup-config
- query:payment-preferences
- manage:payment-schedules
- update:ssd
- query:businesses
- view:detailed-usage
- create:repayment-request
- query:fit-schedules
- join:campaign-events
- create:complaints
- update:sensitive-customer-information
- manage:product-enrolment
- query:property
- query:devices
- query:mfa-device
- query:account-campaigns
- cancel:centrepay-deductions
- query:electricity-meter-point-details
- stop:automated-payments
- occupy:accounts
- update:user-details
- accept:terms-and-conditions
- review:quote
- query:account-payments
- manage:account-renewals
- join:campaigns
- query:account-reminders
- update:account-details
- update:smart-meter-data-preferences
- report:move-out
- process:move-outs
- query:establishments
- query:payment-instructions
- create:quoting-offer-group
- query:portfolios
- view:api-key
- query:user-details
- access:customer-queries
- query:account-applications
- manage:goods-purchases
- edit:customer-marketing-preference
- provide:missing-meter-point-details
- accept:fit-schedules
- cancel:enrollment
- query:loyalty-points-ledger-entry
- create:mfa-device
- request:consumption-data
- create:payment-action-intents
- query:personally-identifiable-information
- create:customer-feedback
- create:centrepay-deductions
- view:sensitive-customer-information
- accept:fit-terms-and-conditions
- create:property
- submit:customer-feedback
- view:account-type
- add:credit-to-smart-meter
- escalate:ink-conversation
- query:contracts
- submit:fit-meter-readings
- add:campaign-to-account
- view:campaign-dashboards
- send:loss-objection-for-change-of-supplier
- query:customer-assets
- register:smartflex-devices
- query:property-meters
- query:billing-information
- manage:customer-assets
- verify:customer-details
- view:account-user-permissions
- view:account-number
- view:ev-data
- update:reading-consent-granularity
- book:smart-meter-appointments
- checkout:quote
- update:dd-day
- transfer:loyalty-points
- set:loyalty-points-user
- manage:ink-live-chat
- update:dd-amount
- query:complaints
- submit:meter-readings
- query:authorized-applications
- validate:mfa-device
- initiate:standalone-payments
- view:customer-communications
- view:customer-marketing-preference
- manage:contribution-agreements
- delete:mfa-device
- cancel:siteworks-appointments
- set:payment-preference
- query:goods-quotes
- query:auto-topup-config
- manage:ev
- create:payment-instructions
- redeem:loyalty-points
- query:loyalty-points-balance
- update:smart-meter-interest
- query:lifecycle-processes
scopes:
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: full-customer-access
- description: ''
  flows: []
  scope: create:payment-method-action-intents
- description: ''
  flows: []
  scope: change:centrepay-deductions
- description: ''
  flows: []
  scope: query:agreements
- description: ''
  flows: []
  scope: view:smartflex-data
- description: ''
  flows: []
  scope: amend:payments
- description: ''
  flows: []
  scope: query:customer-flexibility-campaigns
- description: ''
  flows: []
  scope: query:goods-products
- description: ''
  flows: []
  scope: query:loyalty-enrollment-eligibility
- description: ''
  flows: []
  scope: query:workflows
- description: ''
  flows: []
  scope: query:fit-installations
- description: ''
  flows: []
  scope: create:goods-quotes
- description: ''
  flows: []
  scope: query:contribution-agreements
- description: ''
  flows: []
  scope: configure:auto-topup-config
- description: ''
  flows: []
  scope: query:payment-preferences
- description: ''
  flows: []
  scope: manage:payment-schedules
- description: ''
  flows: []
  scope: update:ssd
- description: ''
  flows: []
  scope: query:businesses
- description: ''
  flows: []
  scope: view:detailed-usage
- description: ''
  flows: []
  scope: create:repayment-request
- description: ''
  flows: []
  scope: query:fit-schedules
- description: ''
  flows: []
  scope: join:campaign-events
- description: ''
  flows: []
  scope: create:complaints
- description: ''
  flows: []
  scope: update:sensitive-customer-information
- description: ''
  flows: []
  scope: manage:product-enrolment
- description: ''
  flows: []
  scope: query:property
- description: ''
  flows: []
  scope: query:devices
- description: ''
  flows: []
  scope: query:mfa-device
- description: ''
  flows: []
  scope: query:account-campaigns
- description: ''
  flows: []
  scope: cancel:centrepay-deductions
- description: ''
  flows: []
  scope: query:electricity-meter-point-details
- description: ''
  flows: []
  scope: stop:automated-payments
- description: ''
  flows: []
  scope: occupy:accounts
- description: ''
  flows: []
  scope: update:user-details
- description: ''
  flows: []
  scope: accept:terms-and-conditions
- description: ''
  flows: []
  scope: review:quote
- description: ''
  flows: []
  scope: query:account-payments
- description: ''
  flows: []
  scope: manage:account-renewals
- description: ''
  flows: []
  scope: join:campaigns
- description: ''
  flows: []
  scope: query:account-reminders
- description: ''
  flows: []
  scope: update:account-details
- description: ''
  flows: []
  scope: update:smart-meter-data-preferences
- description: ''
  flows: []
  scope: report:move-out
- description: ''
  flows: []
  scope: process:move-outs
- description: ''
  flows: []
  scope: query:establishments
- description: ''
  flows: []
  scope: query:payment-instructions
- description: ''
  flows: []
  scope: create:quoting-offer-group
- description: ''
  flows: []
  scope: query:portfolios
- description: ''
  flows: []
  scope: view:api-key
- description: ''
  flows: []
  scope: query:user-details
- description: ''
  flows: []
  scope: access:customer-queries
- description: ''
  flows: []
  scope: query:account-applications
- description: ''
  flows: []
  scope: manage:goods-purchases
- description: ''
  flows: []
  scope: edit:customer-marketing-preference
- description: ''
  flows: []
  scope: provide:missing-meter-point-details
- description: ''
  flows: []
  scope: accept:fit-schedules
- description: ''
  flows: []
  scope: cancel:enrollment
- description: ''
  flows: []
  scope: query:loyalty-points-ledger-entry
- description: ''
  flows: []
  scope: create:mfa-device
- description: ''
  flows: []
  scope: request:consumption-data
- description: ''
  flows: []
  scope: create:payment-action-intents
- description: ''
  flows: []
  scope: query:personally-identifiable-information
- description: ''
  flows: []
  scope: create:customer-feedback
- description: ''
  flows: []
  scope: create:centrepay-deductions
- description: ''
  flows: []
  scope: view:sensitive-customer-information
- description: ''
  flows: []
  scope: accept:fit-terms-and-conditions
- description: ''
  flows: []
  scope: create:property
- description: ''
  flows: []
  scope: submit:customer-feedback
- description: ''
  flows: []
  scope: view:account-type
- description: ''
  flows: []
  scope: add:credit-to-smart-meter
- description: ''
  flows: []
  scope: escalate:ink-conversation
- description: ''
  flows: []
  scope: query:contracts
- description: ''
  flows: []
  scope: submit:fit-meter-readings
- description: ''
  flows: []
  scope: add:campaign-to-account
- description: ''
  flows: []
  scope: view:campaign-dashboards
- description: ''
  flows: []
  scope: send:loss-objection-for-change-of-supplier
- description: ''
  flows: []
  scope: query:customer-assets
- description: ''
  flows: []
  scope: register:smartflex-devices
- description: ''
  flows: []
  scope: query:property-meters
- description: ''
  flows: []
  scope: query:billing-information
- description: ''
  flows: []
  scope: manage:customer-assets
- description: ''
  flows: []
  scope: verify:customer-details
- description: ''
  flows: []
  scope: view:account-user-permissions
- description: ''
  flows: []
  scope: view:account-number
- description: ''
  flows: []
  scope: view:ev-data
- description: ''
  flows: []
  scope: update:reading-consent-granularity
- description: ''
  flows: []
  scope: book:smart-meter-appointments
- description: ''
  flows: []
  scope: checkout:quote
- description: ''
  flows: []
  scope: update:dd-day
- description: ''
  flows: []
  scope: transfer:loyalty-points
- description: ''
  flows: []
  scope: set:loyalty-points-user
- description: ''
  flows: []
  scope: manage:ink-live-chat
- description: ''
  flows: []
  scope: update:dd-amount
- description: ''
  flows: []
  scope: query:complaints
- description: ''
  flows: []
  scope: submit:meter-readings
- description: ''
  flows: []
  scope: query:authorized-applications
- description: ''
  flows: []
  scope: validate:mfa-device
- description: ''
  flows: []
  scope: initiate:standalone-payments
- description: ''
  flows: []
  scope: view:customer-communications
- description: ''
  flows: []
  scope: view:customer-marketing-preference
- description: ''
  flows: []
  scope: manage:contribution-agreements
- description: ''
  flows: []
  scope: delete:mfa-device
- description: ''
  flows: []
  scope: cancel:siteworks-appointments
- description: ''
  flows: []
  scope: set:payment-preference
- description: ''
  flows: []
  scope: query:goods-quotes
- description: ''
  flows: []
  scope: query:auto-topup-config
- description: ''
  flows: []
  scope: manage:ev
- description: ''
  flows: []
  scope: create:payment-instructions
- description: ''
  flows: []
  scope: redeem:loyalty-points
- description: ''
  flows: []
  scope: query:loyalty-points-balance
- description: ''
  flows: []
  scope: update:smart-meter-interest
- description: ''
  flows: []
  scope: query:lifecycle-processes
slug: origin-energy-scopes
source_filename: origin-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: well-known/origin-energy-kraken-openid-configuration.json\ndocs: https://developer.origin-kraken.energy/graphql/guides/basics/\nnote: Harvested verbatim from the Kraken authorisation server's OpenID Connect discovery document (HTTP\n  200, anonymous, 2026-07-27). The Kraken OpenAPI documents declare only apiKey/basic security schemes\n  and no oauth2 flows, so these scopes cannot be derived from the specs — they exist only in the discovery\n  document. Scopes are enforced on the GraphQL and REST surfaces behind the same bearer token. The Consumer\n  Data Right surface uses the separate CDR consent scopes defined by the Data Standards Body, not these.\nschemes:\n- name: Kraken OpenID Connect\n  type: openIdConnect\n  issuer: https://auth.origin-kraken.energy/token/\n  discovery: https://auth.origin-kraken.energy/.well-known/openid-configuration\n  authorizationUrl: https://auth.origin-kraken.energy/authorize/\n  tokenUrl: https://auth.origin-kraken.energy/token/\n\
  \  revocationUrl: https://auth.origin-kraken.energy/revoke-token/\n  userinfoUrl: https://auth.origin-kraken.energy/userinfo/\n  jwksUrl: https://auth.origin-kraken.energy/.well-known/jwks.json\n  endSessionUrl: https://auth.origin-kraken.energy/logout/\n  response_types_supported:\n  - code\n  - token\n  - id_token\n  - id_token token\n  - code token\n  - code id_token\n  - code id_token token\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  dynamic_client_registration: false\n  pkce_methods_advertised: false\ncounts:\n  scopes: 113\n  groups: 36\nscopes:\n- scope: openid\n  group: openid-connect\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: full-customer-access\n  group: broad\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: create:payment-method-action-intents\n  group: create\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: change:centrepay-deductions\n\
  \  group: change\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:agreements\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: view:smartflex-data\n  group: view\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: amend:payments\n  group: amend\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:customer-flexibility-campaigns\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:goods-products\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:loyalty-enrollment-eligibility\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:workflows\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:fit-installations\n  group:\
  \ query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: create:goods-quotes\n  group: create\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:contribution-agreements\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: configure:auto-topup-config\n  group: configure\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:payment-preferences\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: manage:payment-schedules\n  group: manage\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: update:ssd\n  group: update\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:businesses\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: view:detailed-usage\n  group: view\n\
  \  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: create:repayment-request\n  group: create\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:fit-schedules\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: join:campaign-events\n  group: join\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: create:complaints\n  group: create\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: update:sensitive-customer-information\n  group: update\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: manage:product-enrolment\n  group: manage\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:property\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:devices\n  group: query\n  sources:\n\
  \  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:mfa-device\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:account-campaigns\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: cancel:centrepay-deductions\n  group: cancel\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:electricity-meter-point-details\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: stop:automated-payments\n  group: stop\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: occupy:accounts\n  group: occupy\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: update:user-details\n  group: update\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: accept:terms-and-conditions\n  group: accept\n  sources:\n\
  \  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: review:quote\n  group: review\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:account-payments\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: manage:account-renewals\n  group: manage\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: join:campaigns\n  group: join\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:account-reminders\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: update:account-details\n  group: update\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: update:smart-meter-data-preferences\n  group: update\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: report:move-out\n  group: report\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n\
  - scope: process:move-outs\n  group: process\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:establishments\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:payment-instructions\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: create:quoting-offer-group\n  group: create\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:portfolios\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: view:api-key\n  group: view\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:user-details\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: access:customer-queries\n  group: access\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:account-applications\n\
  \  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: manage:goods-purchases\n  group: manage\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: edit:customer-marketing-preference\n  group: edit\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: provide:missing-meter-point-details\n  group: provide\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: accept:fit-schedules\n  group: accept\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: cancel:enrollment\n  group: cancel\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:loyalty-points-ledger-entry\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: create:mfa-device\n  group: create\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: request:consumption-data\n\
  \  group: request\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: create:payment-action-intents\n  group: create\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:personally-identifiable-information\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: create:customer-feedback\n  group: create\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: create:centrepay-deductions\n  group: create\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: view:sensitive-customer-information\n  group: view\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: accept:fit-terms-and-conditions\n  group: accept\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: create:property\n  group: create\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n\
  - scope: submit:customer-feedback\n  group: submit\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: view:account-type\n  group: view\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: add:credit-to-smart-meter\n  group: add\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: escalate:ink-conversation\n  group: escalate\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:contracts\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: submit:fit-meter-readings\n  group: submit\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: add:campaign-to-account\n  group: add\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: view:campaign-dashboards\n  group: view\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope:\
  \ send:loss-objection-for-change-of-supplier\n  group: send\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:customer-assets\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: register:smartflex-devices\n  group: register\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:property-meters\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:billing-information\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: manage:customer-assets\n  group: manage\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: verify:customer-details\n  group: verify\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: view:account-user-permissions\n  group: view\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n\
  - scope: view:account-number\n  group: view\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: view:ev-data\n  group: view\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: update:reading-consent-granularity\n  group: update\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: book:smart-meter-appointments\n  group: book\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: checkout:quote\n  group: checkout\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: update:dd-day\n  group: update\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: transfer:loyalty-points\n  group: transfer\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: set:loyalty-points-user\n  group: set\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: manage:ink-live-chat\n\
  \  group: manage\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: update:dd-amount\n  group: update\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:complaints\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: submit:meter-readings\n  group: submit\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:authorized-applications\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: validate:mfa-device\n  group: validate\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: initiate:standalone-payments\n  group: initiate\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: view:customer-communications\n  group: view\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: view:customer-marketing-preference\n\
  \  group: view\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: manage:contribution-agreements\n  group: manage\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: delete:mfa-device\n  group: delete\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: cancel:siteworks-appointments\n  group: cancel\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: set:payment-preference\n  group: set\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:goods-quotes\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:auto-topup-config\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: manage:ev\n  group: manage\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: create:payment-instructions\n  group:\
  \ create\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: redeem:loyalty-points\n  group: redeem\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:loyalty-points-balance\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: update:smart-meter-interest\n  group: update\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\n- scope: query:lifecycle-processes\n  group: query\n  sources:\n  - well-known/origin-energy-kraken-openid-configuration.json\ncdr_scopes:\n  note: Consumer Data Right consent scopes for the energy sector (energy:accounts.basic:read, energy:billing:read,\n    energy:electricity.usage:read, ...) are defined by the Data Standards Body and negotiated through\n    the CDR consent flow, not advertised on any anonymously reachable Origin endpoint. No Origin-hosted\n    CDR OIDC discovery document was found (public.mydata.cdr.originenergy.com.au/.well-known/openid-configuration\n\
  \    returned 404 on 2026-07-27), so they are deliberately not enumerated here.\n  docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/scopes/origin-energy-scopes.yml
summary_line: 113 scopes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- Smart Metering
- Solar
- DER
- Demand Response
- Energy Markets
token_urls: []
---
