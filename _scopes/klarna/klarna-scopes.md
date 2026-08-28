---
api_specs:
- filename: klarna-payments-api-openapi.yml
  format: yaml
  label: Klarna Payments API
  slug: klarna-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payments-api-openapi.yml
- filename: klarna-checkout-api-openapi.yml
  format: yaml
  label: Klarna Checkout API
  slug: klarna-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-checkout-api-openapi.yml
- filename: klarna-customer-token-api-openapi.yml
  format: yaml
  label: Klarna Customer Token API
  slug: klarna-customer-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-customer-token-api-openapi.yml
- filename: klarna-push-notifications-asyncapi.yml
  format: yaml
  label: Klarna Push Notifications
  slug: klarna-push-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/asyncapi/klarna-push-notifications-asyncapi.yml
- filename: klarna-captures-api-openapi.yml
  format: yaml
  label: Klarna Captures API
  slug: klarna-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-captures-api-openapi.yml
- filename: klarna-checkout-api-openapi.yml
  format: yaml
  label: Klarna Checkout API
  slug: klarna-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-checkout-api-openapi.yml
- filename: klarna-customer-token-api-openapi.yml
  format: yaml
  label: Klarna Customer Token API
  slug: klarna-customer-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-customer-token-api-openapi.yml
- filename: klarna-hpp-api-openapi.yml
  format: yaml
  label: Klarna Hpp API
  slug: klarna-hpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-hpp-api-openapi.yml
- filename: klarna-merchant-urls-address-update-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.address Update API
  slug: klarna-merchant-urls-address-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-address-update-api-openapi.yml
- filename: klarna-merchant-urls-country-change-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.country Change API
  slug: klarna-merchant-urls-country-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-country-change-api-openapi.yml
- filename: klarna-merchant-urls-shipping-option-update-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.shipping Option Update API
  slug: klarna-merchant-urls-shipping-option-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-shipping-option-update-api-openapi.yml
- filename: klarna-merchant-urls-validation-api-openapi.yml
  format: yaml
  label: Klarna Merchant Urls.validation API
  slug: klarna-merchant-urls-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchant-urls-validation-api-openapi.yml
- filename: klarna-merchantcard-api-openapi.yml
  format: yaml
  label: Klarna Merchantcard API
  slug: klarna-merchantcard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-merchantcard-api-openapi.yml
- filename: klarna-orders-api-openapi.yml
  format: yaml
  label: Klarna Orders API
  slug: klarna-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-orders-api-openapi.yml
- filename: klarna-payments-api-openapi.yml
  format: yaml
  label: Klarna Payments API
  slug: klarna-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payments-api-openapi.yml
- filename: klarna-payouts-api-openapi.yml
  format: yaml
  label: Klarna Payouts API
  slug: klarna-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payouts-api-openapi.yml
- filename: klarna-refunds-api-openapi.yml
  format: yaml
  label: Klarna Refunds API
  slug: klarna-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-refunds-api-openapi.yml
- filename: klarna-reports-api-openapi.yml
  format: yaml
  label: Klarna Reports API
  slug: klarna-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-reports-api-openapi.yml
- filename: klarna-transactions-api-openapi.yml
  format: yaml
  label: Klarna Transactions API
  slug: klarna-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-transactions-api-openapi.yml
authorization_urls:
- https://login.klarna.com/oauth2/auth
description: OAuth 2.0 / OIDC scopes for Sign in with Klarna, read verbatim from Klarna's own OpenID Connect discovery document at login.klarna.com. Klarna's server-to-server REST APIs (Payments, Order Management, Settlements) do NOT use OAuth — they authenticate with HTTP Basic and an API key, so no scope surface exists there. Every scope below belongs to the consumer-authorization surface.
docs: https://docs.klarna.com/conversion-boosters/sign-in-with-klarna/before-you-start/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Klarna Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Klarna publishes 34 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Klarna API on a user''s behalf.


  Tokens are issued from https://login.klarna.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Klarna
provider_slug: klarna
schemes:
- flows:
  - authorizationUrl: https://login.klarna.com/oauth2/auth
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    revocationUrl: https://login.klarna.com/oauth2/revoke
    tokenUrl: https://login.klarna.com/oauth2/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
    - private_key_jwt
    - none
    userinfoUrl: https://login.klarna.com/userinfo
  issuer: https://login.klarna.com
  jwks_uri: https://login.klarna.com/.well-known/jwks.json
  name: SignInWithKlarna
  source: https://login.klarna.com/.well-known/openid-configuration
  type: openIdConnect
scope_count: 34
scope_names:
- openid
- offline_access
- default
- profile
- email
- phone
- billing_address
- national_identification_number
- create_payment_session
- profile:name
- profile:date_of_birth
- profile:locale
- profile:email
- profile:phone
- profile:billing_address
- profile:shipping_address
- profile:national_id
- profile:national_identification
- profile:country
- profile:gender
- profile:customer_id
- profile:verified:name
- profile:verified:date_of_birth
- personalization:interests
- payment:request:create
- payment:recurring
- payment:authorization:list
- customer:purchase_power
- customer:account_management
- customer:purchase_management
- customer:prequalified_offers
- customer:login
- payment:customer_present
- payment:customer_not_present
scopes:
- description: Required OIDC scope; issues an ID token identifying the Klarna consumer.
  flows:
  - authorizationCode
  scope: openid
- description: Issue a refresh token so the merchant can act after the browser session ends.
  flows:
  - authorizationCode
  scope: offline_access
- description: Klarna default scope bundle.
  flows:
  - authorizationCode
  scope: default
- description: Basic consumer profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Consumer email address (email, email_verified claims).
  flows:
  - authorizationCode
  scope: email
- description: Consumer phone number (phone, phone_verified claims).
  flows:
  - authorizationCode
  scope: phone
- description: Consumer billing address claim.
  flows:
  - authorizationCode
  scope: billing_address
- description: National identification number (and its issuing country).
  flows:
  - authorizationCode
  scope: national_identification_number
- description: Create a Klarna payment session on behalf of the signed-in consumer.
  flows:
  - authorizationCode
  scope: create_payment_session
- description: given_name / family_name claims.
  flows:
  - authorizationCode
  scope: profile:name
- description: date_of_birth claim.
  flows:
  - authorizationCode
  scope: profile:date_of_birth
- description: locale claim.
  flows:
  - authorizationCode
  scope: profile:locale
- description: Email claim, granular form.
  flows:
  - authorizationCode
  scope: profile:email
- description: Phone claim, granular form.
  flows:
  - authorizationCode
  scope: profile:phone
- description: Billing address claim, granular form.
  flows:
  - authorizationCode
  scope: profile:billing_address
- description: Shipping address claim.
  flows:
  - authorizationCode
  scope: profile:shipping_address
- description: National identification number, granular form.
  flows:
  - authorizationCode
  scope: profile:national_id
- description: National identification, granular form.
  flows:
  - authorizationCode
  scope: profile:national_identification
- description: country claim.
  flows:
  - authorizationCode
  scope: profile:country
- description: Gender claim.
  flows:
  - authorizationCode
  scope: profile:gender
- description: Klarna customer identifier.
  flows:
  - authorizationCode
  scope: profile:customer_id
- description: Name claim with Klarna verification status (name_verified).
  flows:
  - authorizationCode
  scope: profile:verified:name
- description: Date of birth with Klarna verification status (date_of_birth_verified).
  flows:
  - authorizationCode
  scope: profile:verified:date_of_birth
- description: Consumer interest signals for personalization.
  flows:
  - authorizationCode
  scope: personalization:interests
- description: Create a payment request for the signed-in consumer.
  flows:
  - authorizationCode
  scope: payment:request:create
- description: Initiate recurring / merchant-initiated payments.
  flows:
  - authorizationCode
  scope: payment:recurring
- description: List the consumer payment authorizations.
  flows:
  - authorizationCode
  scope: payment:authorization:list
- description: Read the consumer purchase power / spending capacity.
  flows:
  - authorizationCode
  scope: customer:purchase_power
- description: Manage the consumer Klarna account.
  flows:
  - authorizationCode
  scope: customer:account_management
- description: Manage the consumer purchases.
  flows:
  - authorizationCode
  scope: customer:purchase_management
- description: Read prequalified financing offers for the consumer.
  flows:
  - authorizationCode
  scope: customer:prequalified_offers
- description: Authenticate the consumer (Sign in with Klarna).
  flows:
  - authorizationCode
  scope: customer:login
- description: Customer-present payment flow.
  flows:
  - authorizationCode
  scope: payment:customer_present
- description: Customer-not-present (off-session) payment flow.
  flows:
  - authorizationCode
  scope: payment:customer_not_present
slug: klarna-scopes
source_filename: klarna-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://login.klarna.com/.well-known/openid-configuration\ndocs: https://docs.klarna.com/conversion-boosters/sign-in-with-klarna/before-you-start/\ndescription: OAuth 2.0 / OIDC scopes for Sign in with Klarna, read verbatim from Klarna's own OpenID Connect\n  discovery document at login.klarna.com. Klarna's server-to-server REST APIs (Payments, Order Management,\n  Settlements) do NOT use OAuth — they authenticate with HTTP Basic and an API key, so no scope surface\n  exists there. Every scope below belongs to the consumer-authorization surface.\napplies_to: Sign in with Klarna (consumer OAuth/OIDC), not the merchant REST APIs\nschemes:\n- name: SignInWithKlarna\n  type: openIdConnect\n  source: https://login.klarna.com/.well-known/openid-configuration\n  issuer: https://login.klarna.com\n  jwks_uri: https://login.klarna.com/.well-known/jwks.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.klarna.com/oauth2/auth\n\
  \    tokenUrl: https://login.klarna.com/oauth2/token\n    revocationUrl: https://login.klarna.com/oauth2/revoke\n    userinfoUrl: https://login.klarna.com/userinfo\n    pkce:\n    - S256\n    grant_types:\n    - authorization_code\n    - refresh_token\n    token_endpoint_auth_methods:\n    - client_secret_post\n    - client_secret_basic\n    - private_key_jwt\n    - none\nclaims_supported:\n- sub\n- email\n- email_verified\n- phone\n- phone_verified\n- given_name\n- family_name\n- date_of_birth\n- date_of_birth_verified\n- name_verified\n- country\n- billing_address\n- shipping_address\n- locale\n- national_identification_number\n- national_identification_number_country\nscope_count: 34\nscopes:\n- scope: openid\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Required OIDC scope; issues an ID token identifying the Klarna consumer.\n- scope: offline_access\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n\
  \  description: Issue a refresh token so the merchant can act after the browser session ends.\n- scope: default\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Klarna default scope bundle.\n- scope: profile\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Basic consumer profile claims.\n- scope: email\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Consumer email address (email, email_verified claims).\n- scope: phone\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Consumer phone number (phone, phone_verified claims).\n- scope: billing_address\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Consumer billing address\
  \ claim.\n- scope: national_identification_number\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: National identification number (and its issuing country).\n- scope: create_payment_session\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Create a Klarna payment session on behalf of the signed-in consumer.\n- scope: profile:name\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: given_name / family_name claims.\n- scope: profile:date_of_birth\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: date_of_birth claim.\n- scope: profile:locale\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: locale claim.\n- scope: profile:email\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Email claim, granular form.\n- scope: profile:phone\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Phone claim, granular form.\n- scope: profile:billing_address\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Billing address claim, granular form.\n- scope: profile:shipping_address\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Shipping address claim.\n- scope: profile:national_id\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: National identification number, granular form.\n- scope: profile:national_identification\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ https://login.klarna.com/.well-known/openid-configuration\n  description: National identification, granular form.\n- scope: profile:country\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: country claim.\n- scope: profile:gender\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Gender claim.\n- scope: profile:customer_id\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Klarna customer identifier.\n- scope: profile:verified:name\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Name claim with Klarna verification status (name_verified).\n- scope: profile:verified:date_of_birth\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description:\
  \ Date of birth with Klarna verification status (date_of_birth_verified).\n- scope: personalization:interests\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Consumer interest signals for personalization.\n- scope: payment:request:create\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Create a payment request for the signed-in consumer.\n- scope: payment:recurring\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Initiate recurring / merchant-initiated payments.\n- scope: payment:authorization:list\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: List the consumer payment authorizations.\n- scope: customer:purchase_power\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n\
  \  description: Read the consumer purchase power / spending capacity.\n- scope: customer:account_management\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Manage the consumer Klarna account.\n- scope: customer:purchase_management\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Manage the consumer purchases.\n- scope: customer:prequalified_offers\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Read prequalified financing offers for the consumer.\n- scope: customer:login\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Authenticate the consumer (Sign in with Klarna).\n- scope: payment:customer_present\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n\
  \  description: Customer-present payment flow.\n- scope: payment:customer_not_present\n  flows:\n  - authorizationCode\n  sources:\n  - https://login.klarna.com/.well-known/openid-configuration\n  description: Customer-not-present (off-session) payment flow.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/scopes/klarna-scopes.yml
summary_line: 34 scopes · authorizationCode
tags:
- Fintech
- BNPL
- Payments
- Cards
- Shopping
- Banking
- Checkout
- Order Management
- Settlement
- Open Banking
- PSD2
- Consumer Credit
- Sweden
token_urls:
- https://login.klarna.com/oauth2/token
---
