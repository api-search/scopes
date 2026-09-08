---
api_specs:
- filename: citi-authentication-api-1-openapi.yaml
  format: yaml
  label: Citi API Authentication Services
  slug: citi-api-authentication-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-authentication-api-1-openapi.yaml
- filename: citi-blocksandfilters-openapi.yaml
  format: yaml
  label: Citi Account Reporting APIs
  slug: citi-account-reporting-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-blocksandfilters-openapi.yaml
- filename: citi-digitalpaymentscollectionsv12-openapi.yaml
  format: yaml
  label: Citi Outgoing Payments APIs
  slug: citi-outgoing-payments-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-digitalpaymentscollectionsv12-openapi.yaml
- filename: citi-brazillocalmandate-openapi.yaml
  format: yaml
  label: Citi Payment Acceptance APIs
  slug: citi-payment-acceptance-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-brazillocalmandate-openapi.yaml
- filename: citi-marqueta-openapi.yaml
  format: yaml
  label: Citi Commercial Cards and Virtual Card Accounts APIs
  slug: citi-commercial-cards-and-virtual-card-accounts-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-marqueta-openapi.yaml
- filename: citi-fx-authentication-api-openapi.yaml
  format: yaml
  label: CitiFX Gateway and Instant FX APIs
  slug: citifx-gateway-and-instant-fx-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-fx-authentication-api-openapi.yaml
- filename: citi-custody-billing-openapi.yaml
  format: yaml
  label: Citi Custody and Securities Services APIs
  slug: citi-custody-and-securities-services-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-custody-billing-openapi.yaml
- filename: citi-transfer-agency-accounts-openapi.yaml
  format: yaml
  label: Citi Funds Transfer Agency APIs
  slug: citi-funds-transfer-agency-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-transfer-agency-accounts-openapi.yaml
- filename: citi-ukraine-bank-data-sharing-api-openapi.yaml
  format: yaml
  label: Citi Open Banking APIs
  slug: citi-open-banking-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-ukraine-bank-data-sharing-api-openapi.yaml
- filename: citi-finance-undertaking-api-openapi.yaml
  format: yaml
  label: CitiConnect Trade Services APIs
  slug: citiconnect-trade-services-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-finance-undertaking-api-openapi.yaml
- filename: citi-marketplace-management-openapi.yaml
  format: yaml
  label: Citi Gateway Services API
  slug: citi-gateway-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-marketplace-management-openapi.yaml
- filename: citi-self-service-api-openapi.yaml
  format: yaml
  label: Citi Additional Payment Services APIs
  slug: citi-additional-payment-services-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-self-service-api-openapi.yaml
authorization_urls:
- /authenticationservices/v3/oauth/token
- /authenticationservices/v2/oauth/token
- https://tts.apib2b.citi.com/tts/api/v1/oauth2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Citi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Citi publishes 24 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Citi API on a user''s behalf.


  Tokens are issued from https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Citi
provider_slug: citi
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-account-balance-inquiry-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-account-notifications-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-accounts-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth
  source: openapi/citi-accountsv5-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - authorizationUrl: /authenticationservices/v3/oauth/token
    flow: authorizationCode
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-add-on-service-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: Client Credentials
  source: openapi/citi-addonservice-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-balances-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-beneficiary-search-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-blocksandfilters-openapi.yaml
- flows:
  - authorizationUrl: /authenticationservices/v3/oauth/token
    flow: authorizationCode
    tokenUrl: /authenticationservices/v3/oauth/token
  name: OAuth2
  source: openapi/citi-brazillocalmandate-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-bulk-payments-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/api/oauth2/token
  name: ClientCredentials
  source: openapi/citi-card-disputes-openapi.yaml
- description: This API uses OAuth 2 with the client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /markets/api/oauth2/token
  name: client-Credential-Oauth-Security-Schema
  source: openapi/citi-cash-balances-openapi.yaml
- description: This API uses OAuth 2 with the client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /markets/api/oauth2/token
  name: client-Credential-Oauth-Security-Schema
  source: openapi/citi-cash-transactions-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-clearing-exception-report-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - authorizationUrl: /authenticationservices/v3/oauth/token
    flow: authorizationCode
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-contractstatusinquiry-openapi.yaml
- description: This API uses OAuth 2 with the client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /markets/api/oauth2/token
  name: client-Credential-Oauth-Security-Schema
  source: openapi/citi-custody-billing-openapi.yaml
- description: This API uses OAuth 2 with the client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /markets/api/oauth2/token
  name: client-Credential-Oauth-Security-Schema
  source: openapi/citi-custody-fx-transactions-openapi.yaml
- description: This API uses OAuth 2 with the client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /markets/api/oauth2/token
  name: client-Credential-Oauth-Security-Schema
  source: openapi/citi-custody-penalties-openapi.yaml
- flows:
  - authorizationUrl: /authenticationservices/v3/oauth/token
    flow: authorizationCode
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth2
  source: openapi/citi-digitalpaymentscollectionsv12-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.sandbox.apib2b.citi.com/citiconnect/sb/authenticationservices/v1/oauth/token
  name: clientCredentials
  source: openapi/citi-direct-debit-api-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: cobVWriteSample
  source: openapi/citi-due-date-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: cobVReadSample
  source: openapi/citi-due-date-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.sit.apib2b.citi.com/citiconnect/sit5/authenticationservices/v1/oauth/token
  name: clientCredentials
  source: openapi/citi-e-mandate-api-v1-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.sandbox.apib2b.citi.com/citiconnect/sb/authenticationservices/v1/oauth/token
  name: clientCredentials
  source: openapi/citi-e-mandate-api-v2-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - authorizationUrl: /authenticationservices/v3/oauth/token
    flow: authorizationCode
    tokenUrl: /authenticationservices/v3/oauth/token
  name: Client Credentials
  source: openapi/citi-entityid-openapi.yaml
- flows:
  - authorizationUrl: /authenticationservices/v3/oauth/token
    flow: authorizationCode
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth2
  source: openapi/citi-express-payments-api-openapi.yaml
- flows:
  - authorizationUrl: /authenticationservices/v3/oauth/token
    flow: authorizationCode
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth2
  source: openapi/citi-express-payments-webhooks-openapi.yaml
- description: This API uses OAuth2 with the client credentials grant type for service provider API gateway integration.
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: oAuth2
  source: openapi/citi-finance-undertaking-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-benchmark-async-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-benchmark-sync-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-cancel-async-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-cancel-sync-api-openapi.yaml
- description: client_credential
  flows:
  - flow: clientCredentials
    tokenUrl: https://icg.api.citigroup.net/markets/internal/cv/api/fx/oauth2/token
  name: client_credential
  source: openapi/citi-fx-ecommerce-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-gateway-reporting-async-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-gateway-reporting-sync-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-market-async-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-market-sync-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-orders-async-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-orders-sync-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-quote-async-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-quote-sync-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-reporting-async-api-openapi.yaml
- description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. See <a href="../../fx/authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token
  name: OAuth2
  source: openapi/citi-fx-reporting-sync-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-grace-iva-openapi.yaml
- description: 'All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.<br><br>Sandbox Token URL: https://tts.sandbox.apib2b.citi.com/tts/api/oauth2/token<br>'
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/oauth2/token
  name: clientCredentials
  source: openapi/citi-id-provisioning-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - authorizationUrl: /authenticationservices/v3/oauth/token
    flow: authorizationCode
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-idd-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: cobWriteSample
  source: openapi/citi-immediate-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: cobReadSample
  source: openapi/citi-immediate-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://b2b.api.icg.citi.com/authenticationservices/v3/oauth/token
  name: oAuth2
  source: openapi/citi-marketplace-management-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-marqueta-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/mvca/v1/token-lifecycle-events/cv/api/oauth2/token
  name: clientCredentials
  source: openapi/citi-mobile-wallets-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-mobilecardonboarding-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-mobilevirtuallifecycle-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: Client Credentials
  source: openapi/citi-online-payment-acceptance-api-openapi.yaml
- description: "Client applications must supply an\n authentication token with every request, and therefore must first\n authenticate before it can proceed. A client can use the OAuth 2 client\n credential grant flow to obtain a time limited access token. To get an\n access token send a HTTP Post request to the token endpoint using basic\n authentication with the client key and secret.<br><br>**Request**<br><br>```POST {baseURL}/tts/api/v1/oauth2/token HTTPS/1.1\n Authorization: Basic base64(key:secret) \n Content-Type:application/x-www-form-urlencoded\n {\n  scope=/api&grant_type=client_credentials\n }```<br><br>\n **Response**<br><br>```\n   {\n     \"token_type\": \"bearer\", \n     \"access_token\": <access token>, \n     \"expires_in\": <seconds until expiry>, \n     \"consented_on\":<timestamp>, \n     \"scope\": \"api\"\n   }```    <br><br>The bearer token is valid for 1800 seconds (30 minutes) after which it will expire. At this point, you would need to re-authenticate.<br><br>"
  flows:
  - flow: clientCredentials
    tokenUrl: /tts/api/v1/oauth2/token
  name: Authorization
  source: openapi/citi-order-approval-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: authenticationservices/v3/oauth/token
  name: oAuth2
  source: openapi/citi-payerid-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See the Citi Authentication API Reference for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v1/oauth/token
  name: clientCredentials
  source: openapi/citi-payment-reconfirmation-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See the Citi Authentication API Reference for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v1/oauth/token
  name: clientCredentials
  source: openapi/citi-payment-refund-openapi.yaml
- description: All CitiConnect APIs use the OAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See the Citi Authentication API Reference for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: $(catalog.url)/authenticationservices/v1/oauth/token
  name: clientCredentials
  source: openapi/citi-payment-status-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.sit.apib2b.citi.com/citiconnect/sit5/authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-paymentcancellation-json-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.sit.apib2b.citi.com/citiconnect/sit5/authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-paymentcancellation-xml-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-paymentenhancedinquiry-json-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-paymentenhancedinquiry-xml-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-paymentinitiation-pacs008-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-paymentinitiation-pacs009-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-paymentinitiation-pain102-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-paymentinitiation-pain103-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-payto-openapi.yaml
- description: "Client applications must supply an authentication token with every request, and therefore must first authenticate before it can proceed. A client can use the OAuth 2 client credential grant flow to obtain a time limited access token. To get an access token send a HTTP Post request to the token endpoint using basic authentication with the client key and secret.<br><br>**Request**<br><br>```POST {baseURL}/tts/api/v1/oauth2/token HTTPS/1.1 Authorization: Basic base64(key:secret)  Content-Type:application/x-www-form-urlencoded {\n scope=/api&grant_type=client_credentials\n}```<br><br> **Response**<br><br>```\n  {\n    \"token_type\": \"bearer\", \n    \"access_token\": <access token>, \n    \"expires_in\": <seconds until expiry>, \n    \"consented_on\":<timestamp>, \n    \"scope\": \"api\"\n  }```    <br><br>The bearer token is valid for 1800 seconds (30 minutes) after which it will expire. At this point, you would need to re-authenticate.<br><br>"
  flows:
  - flow: clientCredentials
    tokenUrl: /tts/api/v1/oauth2/token
  name: Authentication
  source: openapi/citi-portfolio-listing-openapi.yaml
- description: OAuth2 Authorization Code Flow
  flows:
  - authorizationUrl: /authenticationservices/v3/oauth/token
    flow: authorizationCode
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth2
  source: openapi/citi-proof-of-payment-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-purchase-openapi.yaml
- description: 'All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.<br><br>Sandbox Token URL: https://tts.sandbox.apib2b.citi.com/tts/api/oauth2/token<br>'
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/oauth2/token
  name: clientCredentials
  source: openapi/citi-reporting-get-2-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/citiconnect/prod/requesttopayservice/v1/validate/address/authenticationservices/v1/oauth/token
  name: clientCredentials
  source: openapi/citi-request-to-pay-openapi.yaml
- description: This API uses OAuth 2 with the client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /markets/api/oauth2/token
  name: client-Credential-Oauth-Security-Schema
  source: openapi/citi-safekeeping-accounts-openapi.yaml
- description: This API uses OAuth 2 with the client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /markets/api/oauth2/token
  name: client-Credential-Oauth-Security-Schema
  source: openapi/citi-safekeeping-positions-openapi.yaml
- description: This API uses OAuth 2 with the client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /markets/api/oauth2/token
  name: client-Credential-Oauth-Security-Schema
  source: openapi/citi-securitytransactionsaccounts-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.sandbox.apib2b.citi.com/citiconnect/sb/authenticationservices/v1/oauth/token
  name: clientCredentials
  source: openapi/citi-self-service-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-statement-transactions-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v1/oauth/token
  name: clientCredentials
  source: openapi/citi-statements-api-openapi.yaml
- flows:
  - authorizationUrl: /authenticationservices/v2/oauth/token
    flow: authorizationCode
    tokenUrl: authenticationservices/v2/oauth/token
  name: oAuth2
  source: openapi/citi-statementsv2-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - authorizationUrl: /authenticationservices/v3/oauth/token
    flow: authorizationCode
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-static-openapi.yaml
- description: All APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /tts/internal/api/oauth2
  name: clientCredentials
  source: openapi/citi-submit-action-openapi.yaml
- description: This API uses OAuth 2 with the client credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: /markets/api/oauth2/token
  name: client-Credential-Oauth-Security-Schema
  source: openapi/citi-tax-reclaims-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-trade-api-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth2
  source: openapi/citi-transfer-agency-accounts-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth2
  source: openapi/citi-transfer-agency-holding-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth2
  source: openapi/citi-transfer-agency-investors-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth2
  source: openapi/citi-transfer-agency-transactions-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth
  source: openapi/citi-ukraine-bank-data-sharing-api-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://secure.api-preprod.bkm.com.tr/oauth-provider/oauth2/token
  name: auth
  source: openapi/citi-ukraine-bank-data-sharing-api-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth
  source: openapi/citi-ukraine-payment-service-initiation-api-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://secure.api-preprod.bkm.com.tr/oauth-provider/oauth2/token
  name: auth
  source: openapi/citi-ukraine-payment-service-initiation-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-vamanagement-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-vca-api-openapi.yaml
- description: OAuth2 Client Credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.sandbox.apib2b.citi.com/tts/cards/api/oauth2/token
  name: ClientCredentials
  source: openapi/citi-vcaeventssubscriptions-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/token
  name: ClientCredentials
  source: openapi/citi-vcagetnotifications-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-virtual-cards-lifecycle-v1-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/token
  name: ClientCredentials
  source: openapi/citi-virtual-cards-lifecycle-v4-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-virtual-cards-notifications-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.sandbox.apib2b.citi.com/citiconnect/sb/authenticationservices/v1/oauth/token
  name: clientCredentials
  source: openapi/citi-virtual-cards-pi-openapi.yaml
- description: OAuth 2.0 Client Credentials flow for API authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/token
  name: ClientCredentials
  source: openapi/citi-virtual-cards-pi-v2-openapi.yaml
- flows:
  - authorizationUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/token
  name: OAuth2
  source: openapi/citi-virtual-cards-pi-webhooks-openapi.yaml
- description: 'All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.<br><br>Sandbox Token URL: https://tts.sandbox.apib2b.citi.com/tts/api/v1/oauth2/token<br>'
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-virtual-cards-reporting-openapi.yaml
- description: 'All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.<br><br>Sandbox Token URL: https://tts.sandbox.apib2b.citi.com/tts/api/v1/oauth2/token<br>'
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/token
  name: clientCredentials
  source: openapi/citi-virtual-cards-reporting-v1-openapi.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: oAuth2
  source: openapi/citi-worldlink-ir-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-worldlink-v1-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-worldlink-v2-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: /authenticationservices/v3/oauth/token
  name: clientCredentials
  source: openapi/citi-worldlink-v3-api-openapi.yaml
- description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer token to authenticate your API call. The Token URL includes the version of authentication used by this API. See <a href="../../authentication/authentication-api-reference/" target="_blank">the Citi Authentication API reference</a> for information on requesting a token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://tts.sandbox.apib2b.citi.com/citiconnect/sb/authenticationservices/v1/oauth/token
  name: clientCredentials
  source: openapi/citi-worldlink-v5-api-openapi.yaml
scope_count: 24
scope_names:
- /api
- /authenticationservices/v1
- /dod
- /fxapi
- account_information
- addonservices
- admin
- authenticationservices/v1
- authenticationservices/v2
- authenticationservices/v3
- cob.read
- cob.write
- cobv.read
- cobv.write
- directDebitService
- emandateservices
- fxapi
- payment_order
- paymentservices
- read
- selfservices
- webhook.write
- webhookcobr.write
- write
scopes:
- description: Access to ETF Order API
  flows:
  - clientCredentials
  scope: /api
- description: Access to Accounts, Balances, Transactions Information
  flows:
  - clientCredentials
  scope: /authenticationservices/v1
- description: Access to Cash Balances Information
  flows:
  - clientCredentials
  scope: /dod
- description: ''
  flows:
  - clientCredentials
  scope: /fxapi
- description: Account Information
  flows:
  - clientCredentials
  scope: account_information
- description: Grant read-only access to add-on services
  flows:
  - authorizationCode
  scope: addonservices
- description: Grants read and write access to administrative information
  flows:
  - authorizationCode
  scope: admin
- description: Grant read-only access to payment initation service
  flows:
  - authorizationCode
  - clientCredentials
  scope: authenticationservices/v1
- description: API Access for
  flows:
  - authorizationCode
  scope: authenticationservices/v2
- description: Grant read-only access to WorldLink FX service
  flows:
  - authorizationCode
  scope: authenticationservices/v3
- description: Permission to consult Immediate collection
  flows:
  - clientCredentials
  scope: cob.read
- description: Permission to change Immediate collection
  flows:
  - clientCredentials
  scope: cob.write
- description: Authenticates to retrieve collection item with due date
  flows:
  - clientCredentials
  scope: cobv.read
- description: Authenticates to update collection with due date
  flows:
  - clientCredentials
  scope: cobv.write
- description: Grant read-only access to emandate initation service
  flows:
  - authorizationCode
  scope: directDebitService
- description: Grant read-only access to emandate initation service
  flows:
  - clientCredentials
  scope: emandateservices
- description: ''
  flows:
  - clientCredentials
  scope: fxapi
- description: Payment Order
  flows:
  - clientCredentials
  scope: payment_order
- description: Grant read-only access to payment initiation service
  flows:
  - authorizationCode
  scope: paymentservices
- description: Grants read access
  flows:
  - authorizationCode
  - clientCredentials
  scope: read
- description: Grant read-only access to beneficiary validation
  flows:
  - authorizationCode
  scope: selfservices
- description: ''
  flows: []
  scope: webhook.write
- description: ''
  flows: []
  scope: webhookcobr.write
- description: Grants write access
  flows:
  - authorizationCode
  - clientCredentials
  scope: write
slug: citi-scopes
source_filename: citi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/citi-account-balance-inquiry-api-openapi.yaml, openapi/citi-account-notifications-api-openapi.yaml,\n  openapi/citi-accounts-openapi.yaml, openapi/citi-accountsv5-openapi.yaml, openapi/citi-add-on-service-openapi.yaml,\n  openapi/citi-addonservice-openapi.yaml, openapi/citi-balances-api-openapi.yaml, openapi/citi-beneficiary-search-openapi.yaml,\n  openapi/citi-blocksandfilters-openapi.yaml, openapi/citi-brazillocalmandate-openapi.yaml,\n  openapi/citi-bulk-payments-openapi.yaml, openapi/citi-card-disputes-openapi.yaml, openapi/citi-cash-balances-openapi.yaml,\n  openapi/citi-cash-transactions-openapi.yaml, openapi/citi-clearing-exception-report-openapi.yaml,\n  openapi/citi-contractstatusinquiry-openapi.yaml, openapi/citi-custody-billing-openapi.yaml,\n  openapi/citi-custody-fx-transactions-openapi.yaml, openapi/citi-custody-penalties-openapi.yaml,\n  openapi/citi-digitalpaymentscollectionsv12-openapi.yaml, openapi/citi-direct-debit-api-openapi.yaml,\n\
  \  openapi/citi-due-date-openapi.yaml, openapi/citi-e-mandate-api-v1-openapi.yaml, openapi/citi-e-mandate-api-v2-openapi.yaml,\n  openapi/citi-entityid-openapi.yaml, openapi/citi-express-payments-api-openapi.yaml, openapi/citi-express-payments-webhooks-openapi.yaml,\n  openapi/citi-finance-undertaking-api-openapi.yaml, openapi/citi-fx-benchmark-async-api-openapi.yaml,\n  openapi/citi-fx-benchmark-sync-api-openapi.yaml, openapi/citi-fx-cancel-async-api-openapi.yaml,\n  openapi/citi-fx-cancel-sync-api-openapi.yaml, openapi/citi-fx-ecommerce-api-openapi.yaml,\n  openapi/citi-fx-gateway-reporting-async-api-openapi.yaml, openapi/citi-fx-gateway-reporting-sync-api-openapi.yaml,\n  openapi/citi-fx-market-async-api-openapi.yaml, openapi/citi-fx-market-sync-api-openapi.yaml,\n  openapi/citi-fx-orders-async-api-openapi.yaml, openapi/citi-fx-orders-sync-api-openapi.yaml,\n  openapi/citi-fx-quote-async-api-openapi.yaml, openapi/citi-fx-quote-sync-api-openapi.yaml,\n  openapi/citi-fx-reporting-async-api-openapi.yaml,\
  \ openapi/citi-fx-reporting-sync-api-openapi.yaml,\n  openapi/citi-grace-iva-openapi.yaml, openapi/citi-id-provisioning-openapi.yaml, openapi/citi-idd-openapi.yaml,\n  openapi/citi-immediate-openapi.yaml, openapi/citi-marketplace-management-openapi.yaml, openapi/citi-marqueta-openapi.yaml,\n  openapi/citi-mobile-wallets-openapi.yaml, openapi/citi-mobilecardonboarding-openapi.yaml,\n  openapi/citi-mobilevirtuallifecycle-openapi.yaml, openapi/citi-online-payment-acceptance-api-openapi.yaml,\n  openapi/citi-order-approval-openapi.yaml, openapi/citi-payerid-api-openapi.yaml, openapi/citi-payment-reconfirmation-openapi.yaml,\n  openapi/citi-payment-refund-openapi.yaml, openapi/citi-payment-status-openapi.yaml, openapi/citi-paymentcancellation-json-openapi.yaml,\n  openapi/citi-paymentcancellation-xml-openapi.yaml, openapi/citi-paymentenhancedinquiry-json-openapi.yaml,\n  openapi/citi-paymentenhancedinquiry-xml-openapi.yaml, openapi/citi-paymentinitiation-pacs008-openapi.yaml,\n  openapi/citi-paymentinitiation-pacs009-openapi.yaml,\
  \ openapi/citi-paymentinitiation-pain102-openapi.yaml,\n  openapi/citi-paymentinitiation-pain103-openapi.yaml, openapi/citi-payto-openapi.yaml, openapi/citi-portfolio-listing-openapi.yaml,\n  openapi/citi-proof-of-payment-openapi.yaml, openapi/citi-purchase-openapi.yaml, openapi/citi-reporting-get-2-openapi.yaml,\n  openapi/citi-request-to-pay-openapi.yaml, openapi/citi-safekeeping-accounts-openapi.yaml,\n  openapi/citi-safekeeping-positions-openapi.yaml, openapi/citi-securitytransactionsaccounts-openapi.yaml,\n  openapi/citi-self-service-api-openapi.yaml, openapi/citi-statement-transactions-openapi.yaml,\n  openapi/citi-statements-api-openapi.yaml, openapi/citi-statementsv2-api-openapi.yaml, openapi/citi-static-openapi.yaml,\n  openapi/citi-submit-action-openapi.yaml, openapi/citi-tax-reclaims-openapi.yaml, openapi/citi-trade-api-openapi.yaml,\n  openapi/citi-transfer-agency-accounts-openapi.yaml, openapi/citi-transfer-agency-holding-openapi.yaml,\n  openapi/citi-transfer-agency-investors-openapi.yaml,\
  \ openapi/citi-transfer-agency-transactions-openapi.yaml,\n  openapi/citi-ukraine-bank-data-sharing-api-openapi.yaml, openapi/citi-ukraine-payment-service-initiation-api-openapi.yaml,\n  openapi/citi-vamanagement-openapi.yaml, openapi/citi-vca-api-openapi.yaml, openapi/citi-vcaeventssubscriptions-openapi.yaml,\n  openapi/citi-vcagetnotifications-openapi.yaml, openapi/citi-virtual-cards-lifecycle-v1-openapi.yaml,\n  openapi/citi-virtual-cards-lifecycle-v4-openapi.yaml, openapi/citi-virtual-cards-notifications-openapi.yaml,\n  openapi/citi-virtual-cards-pi-openapi.yaml, openapi/citi-virtual-cards-pi-v2-openapi.yaml,\n  openapi/citi-virtual-cards-pi-webhooks-openapi.yaml, openapi/citi-virtual-cards-reporting-openapi.yaml,\n  openapi/citi-virtual-cards-reporting-v1-openapi.yaml, openapi/citi-worldlink-ir-api-openapi.yaml,\n  openapi/citi-worldlink-v1-api-openapi.yaml, openapi/citi-worldlink-v2-api-openapi.yaml, openapi/citi-worldlink-v3-api-openapi.yaml,\n  openapi/citi-worldlink-v5-api-openapi.yaml\n\
  schemes:\n- name: clientCredentials\n  source: openapi/citi-account-balance-inquiry-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token\n- name: clientCredentials\n  source: openapi/citi-account-notifications-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-accounts-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2\
  \ authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: oAuth\n  source: openapi/citi-accountsv5-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n- name: clientCredentials\n  source: openapi/citi-add-on-service-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /authenticationservices/v3/oauth/token\n    tokenUrl: /authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\"\
  \ target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: Client Credentials\n  source: openapi/citi-addonservice-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-balances-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes\
  \ the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-beneficiary-search-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-blocksandfilters-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n- name: OAuth2\n\
  \  source: openapi/citi-brazillocalmandate-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /authenticationservices/v3/oauth/token\n    tokenUrl: /authenticationservices/v3/oauth/token\n- name: clientCredentials\n  source: openapi/citi-bulk-payments-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n- name: ClientCredentials\n  source: openapi/citi-card-disputes-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.apib2b.citi.com/api/oauth2/token\n- name: client-Credential-Oauth-Security-Schema\n  source: openapi/citi-cash-balances-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /markets/api/oauth2/token\n  description: This API uses OAuth 2 with the client credentials flow\n- name: client-Credential-Oauth-Security-Schema\n  source: openapi/citi-cash-transactions-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /markets/api/oauth2/token\n  description:\
  \ This API uses OAuth 2 with the client credentials flow\n- name: clientCredentials\n  source: openapi/citi-clearing-exception-report-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-contractstatusinquiry-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /authenticationservices/v3/oauth/token\n    tokenUrl: /authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to\
  \ authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: client-Credential-Oauth-Security-Schema\n  source: openapi/citi-custody-billing-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /markets/api/oauth2/token\n  description: This API uses OAuth 2 with the client credentials flow\n- name: client-Credential-Oauth-Security-Schema\n  source: openapi/citi-custody-fx-transactions-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /markets/api/oauth2/token\n  description: This API uses OAuth 2 with the client credentials flow\n- name: client-Credential-Oauth-Security-Schema\n  source: openapi/citi-custody-penalties-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /markets/api/oauth2/token\n  description: This API\
  \ uses OAuth 2 with the client credentials flow\n- name: oAuth2\n  source: openapi/citi-digitalpaymentscollectionsv12-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /authenticationservices/v3/oauth/token\n    tokenUrl: /authenticationservices/v3/oauth/token\n- name: clientCredentials\n  source: openapi/citi-direct-debit-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.sandbox.apib2b.citi.com/citiconnect/sb/authenticationservices/v1/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: cobVWriteSample\n  source: openapi/citi-due-date-openapi.yaml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: /authenticationservices/v3/oauth/token\n- name: cobVReadSample\n  source: openapi/citi-due-date-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n- name: clientCredentials\n  source: openapi/citi-e-mandate-api-v1-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.sit.apib2b.citi.com/citiconnect/sit5/authenticationservices/v1/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-e-mandate-api-v2-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.sandbox.apib2b.citi.com/citiconnect/sb/authenticationservices/v1/oauth/token\n\
  \  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: Client Credentials\n  source: openapi/citi-entityid-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /authenticationservices/v3/oauth/token\n    tokenUrl: /authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n\
  - name: oAuth2\n  source: openapi/citi-express-payments-api-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /authenticationservices/v3/oauth/token\n    tokenUrl: /authenticationservices/v3/oauth/token\n- name: oAuth2\n  source: openapi/citi-express-payments-webhooks-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /authenticationservices/v3/oauth/token\n    tokenUrl: /authenticationservices/v3/oauth/token\n- name: oAuth2\n  source: openapi/citi-finance-undertaking-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: This API uses OAuth2 with the client credentials grant type for service provider\n    API gateway integration.\n- name: OAuth2\n  source: openapi/citi-fx-benchmark-async-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme,\
  \ which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi Authentication API reference</a> for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-benchmark-sync-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi Authentication API reference</a> for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-cancel-async-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication\
  \ scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi Authentication API reference</a> for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-cancel-sync-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi Authentication API reference</a> for information on requesting\n    a token.\n- name: client_credential\n  source: openapi/citi-fx-ecommerce-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://icg.api.citigroup.net/markets/internal/cv/api/fx/oauth2/token\n  description: client_credential\n\
  - name: OAuth2\n  source: openapi/citi-fx-gateway-reporting-async-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi Authentication API reference</a> for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-gateway-reporting-sync-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi Authentication API reference</a>\
  \ for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-market-async-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi Authentication API reference</a> for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-market-sync-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi Authentication\
  \ API reference</a> for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-orders-async-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi Authentication API reference</a> for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-orders-sync-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi\
  \ Authentication API reference</a> for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-quote-async-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi Authentication API reference</a> for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-quote-sync-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\"\
  >the Citi Authentication API reference</a> for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-reporting-async-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"_blank\">the Citi Authentication API reference</a> for information on requesting\n    a token.\n- name: OAuth2\n  source: openapi/citi-fx-reporting-sync-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.citivelocity.com/markets/cv/api/fx/oauth2/token\n  description: Citi Velocity APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. See <a href=\"../../fx/authentication/authentication-api-reference/\"\n    target=\"\
  _blank\">the Citi Authentication API reference</a> for information on requesting\n    a token.\n- name: clientCredentials\n  source: openapi/citi-grace-iva-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-id-provisioning-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/oauth2/token\n  description: 'All CitiConnect APIs use the oAuth2 authentication scheme, which requires a\n    bearer token to authenticate your API call.\
  \ The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.<br><br>Sandbox\n    Token URL: https://tts.sandbox.apib2b.citi.com/tts/api/oauth2/token<br>'\n- name: clientCredentials\n  source: openapi/citi-idd-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /authenticationservices/v3/oauth/token\n    tokenUrl: /authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: cobWriteSample\n  source: openapi/citi-immediate-openapi.yaml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n- name: cobReadSample\n  source: openapi/citi-immediate-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n- name: oAuth2\n  source: openapi/citi-marketplace-management-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://b2b.api.icg.citi.com/authenticationservices/v3/oauth/token\n- name: clientCredentials\n  source: openapi/citi-marqueta-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information\
  \ on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-mobile-wallets-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.apib2b.citi.com/tts/cards/mvca/v1/token-lifecycle-events/cv/api/oauth2/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-mobilecardonboarding-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/token\n- name: clientCredentials\n  source: openapi/citi-mobilevirtuallifecycle-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.apib2b.citi.com/tts/api/v1/oauth2/token\n\
  - name: Client Credentials\n  source: openapi/citi-online-payment-acceptance-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: Authorization\n  source: openapi/citi-order-approval-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /tts/api/v1/oauth2/token\n  description: \"Client applications must supply an\\n authentication token with every request,\\\n    \\ and therefore must first\\n authenticate before it can proceed. A client can use the OAuth\\\n    \\ 2 client\\n credential grant flow to obtain a time limited access\
  \ token. To get an\\n access\\\n    \\ token send a HTTP Post request to the token endpoint using basic\\n authentication with\\\n    \\ the client key and secret.<br><br>**Request**<br><br>```POST {baseURL}/tts/api/v1/oauth2/token\\\n    \\ HTTPS/1.1\\n Authorization: Basic base64(key:secret) \\n Content-Type:application/x-www-form-urlencoded\\n\\\n    \\ {\\n  scope=/api&grant_type=client_credentials\\n }```<br><br>\\n **Response**<br><br>```\\n\\\n    \\   {\\n     \\\"token_type\\\": \\\"bearer\\\", \\n     \\\"access_token\\\": <access token>, \\n    \\\n    \\ \\\"expires_in\\\": <seconds until expiry>, \\n     \\\"consented_on\\\":<timestamp>, \\n     \\\"\\\n    scope\\\": \\\"api\\\"\\n   }```    <br><br>The bearer token is valid for 1800 seconds (30 minutes)\\\n    \\ after which it will expire. At this point, you would need to re-authenticate.<br><br>\"\n- name: oAuth2\n  source: openapi/citi-payerid-api-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: authenticationservices/v3/oauth/token\n\
  - name: clientCredentials\n  source: openapi/citi-payment-reconfirmation-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v1/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See the Citi Authentication API Reference for information on requesting\n    a token.\n- name: clientCredentials\n  source: openapi/citi-payment-refund-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v1/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See the Citi Authentication API Reference for information on requesting\n    a token.\n- name: clientCredentials\n  source: openapi/citi-payment-status-openapi.yaml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: $(catalog.url)/authenticationservices/v1/oauth/token\n  description: All CitiConnect APIs use the OAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See the Citi Authentication API Reference for information on requesting\n    a token.\n- name: clientCredentials\n  source: openapi/citi-paymentcancellation-json-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.sit.apib2b.citi.com/citiconnect/sit5/authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information\
  \ on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-paymentcancellation-xml-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tts.sit.apib2b.citi.com/citiconnect/sit5/authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-paymentenhancedinquiry-json-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the\
  \ version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-paymentenhancedinquiry-xml-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authenticationservices/v3/oauth/token\n  description: All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API. See <a href=\"../../authentication/authentication-api-reference/\" target=\"_blank\">the\n    Citi Authentication API reference</a> for information on requesting a token.\n- name: clientCredentials\n  source: openapi/citi-paymentinitiation-pacs008-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /authenticationservices/v3/oauth/token\n  description:\
  \ All CitiConnect APIs use the oAuth2 authentication scheme, which requires a bearer\n    token to authenticate your API call. The Token URL includes the version of authentication\n    used by this API\n\n# --- truncated at 32 KB (57 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/scopes/citi-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/scopes/citi-scopes.yml
summary_line: 24 scopes · clientCredentials/authorizationCode
tags:
- Banking
- Financial-Services
- Open Banking
- Payments
- Treasury
- ISO 20022
- Commercial Cards
- Foreign Exchange
- Custody
- Trade Finance
- Corporate Banking
- API Gateway
token_urls:
- https://tts.apib2b.citi.com/tts/cards/api/v1/oauth2/token
- /authenticationservices/v3/oauth/token
- https://tts.apib2b.citi.com/api/oauth2/token
- /markets/api/oauth2/token
- https://tts.sandbox.apib2b.citi.com/citiconnect/sb/authenticationservices/v1/oauth/token
- https://tts.sit.apib2b.citi.com/citiconnect/sit5/authenticationservices/v1/oauth/token
- /v1/oauth2/token
- https://api.citivelocity.com/markets/cv/api/fx/oauth2/token
- https://sandbox.api.citivelocity.com/markets/cv/api/fx/oauth2/token
- https://icg.api.citigroup.net/markets/internal/cv/api/fx/oauth2/token
- https://tts.apib2b.citi.com/tts/cards/api/oauth2/token
- https://b2b.api.icg.citi.com/authenticationservices/v3/oauth/token
- https://tts.apib2b.citi.com/tts/cards/mvca/v1/token-lifecycle-events/cv/api/oauth2/token
- https://tts.apib2b.citi.com/tts/api/v1/oauth2/token
- /tts/api/v1/oauth2/token
- authenticationservices/v3/oauth/token
- /authenticationservices/v1/oauth/token
- $(catalog.url)/authenticationservices/v1/oauth/token
- https://tts.sit.apib2b.citi.com/citiconnect/sit5/authenticationservices/v3/oauth/token
- https://authenticationservices/v3/oauth/token
- https://tts.apib2b.citi.com/citiconnect/prod/requesttopayservice/v1/validate/address/authenticationservices/v1/oauth/token
- https://tts.apib2b.citi.com/api/v1/oauth2/token
- authenticationservices/v2/oauth/token
- /tts/internal/api/oauth2
- https://secure.api-preprod.bkm.com.tr/oauth-provider/oauth2/token
- https://tts.sandbox.apib2b.citi.com/tts/cards/api/oauth2/token
---
