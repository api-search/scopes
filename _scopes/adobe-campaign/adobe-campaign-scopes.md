---
api_specs:
- filename: adobe-campaign-custom-resources-api-openapi.yml
  format: yaml
  label: Adobe Campaign Custom Resources API
  slug: adobe-campaign-custom-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-custom-resources-api-openapi.yml
- filename: adobe-campaign-data-management-api-openapi.yml
  format: yaml
  label: Adobe Campaign Data Management API
  slug: adobe-campaign-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-data-management-api-openapi.yml
- filename: adobe-campaign-delivery-api-openapi.yml
  format: yaml
  label: Adobe Campaign Delivery API
  slug: adobe-campaign-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-delivery-api-openapi.yml
- filename: adobe-campaign-marketing-history-api-openapi.yml
  format: yaml
  label: Adobe Campaign Marketing History API
  slug: adobe-campaign-marketing-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-marketing-history-api-openapi.yml
- filename: adobe-campaign-metadata-api-openapi.yml
  format: yaml
  label: Adobe Campaign Metadata API
  slug: adobe-campaign-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-metadata-api-openapi.yml
- filename: adobe-campaign-organizational-units-api-openapi.yml
  format: yaml
  label: Adobe Campaign Organizational Units API
  slug: adobe-campaign-organizational-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-organizational-units-api-openapi.yml
- filename: adobe-campaign-privacy-api-openapi.yml
  format: yaml
  label: Adobe Campaign Privacy API
  slug: adobe-campaign-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-privacy-api-openapi.yml
- filename: adobe-campaign-profileandservices-api-openapi.yml
  format: yaml
  label: Adobe Campaign ProfileAndServices API
  slug: adobe-campaign-profileandservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-profileandservices-api-openapi.yml
- filename: adobe-campaign-profiles-api-openapi.yml
  format: yaml
  label: Adobe Campaign Profiles API
  slug: adobe-campaign-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-profiles-api-openapi.yml
- filename: adobe-campaign-query-definition-api-openapi.yml
  format: yaml
  label: Adobe Campaign Query Definition API
  slug: adobe-campaign-query-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-query-definition-api-openapi.yml
- filename: adobe-campaign-real-time-events-api-openapi.yml
  format: yaml
  label: Adobe Campaign Real-Time Events API
  slug: adobe-campaign-real-time-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-real-time-events-api-openapi.yml
- filename: adobe-campaign-session-management-api-openapi.yml
  format: yaml
  label: Adobe Campaign Session Management API
  slug: adobe-campaign-session-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-session-management-api-openapi.yml
- filename: adobe-campaign-subscription-api-openapi.yml
  format: yaml
  label: Adobe Campaign Subscription API
  slug: adobe-campaign-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-subscription-api-openapi.yml
- filename: adobe-campaign-subscriptions-api-openapi.yml
  format: yaml
  label: Adobe Campaign Subscriptions API
  slug: adobe-campaign-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-subscriptions-api-openapi.yml
- filename: adobe-campaign-transactional-messages-api-openapi.yml
  format: yaml
  label: Adobe Campaign Transactional Messages API
  slug: adobe-campaign-transactional-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-transactional-messages-api-openapi.yml
- filename: adobe-campaign-workflow-api-openapi.yml
  format: yaml
  label: Adobe Campaign Workflow API
  slug: adobe-campaign-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-workflow-api-openapi.yml
- filename: adobe-campaign-workflows-api-openapi.yml
  format: yaml
  label: Adobe Campaign Workflows API
  slug: adobe-campaign-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-workflows-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/implementation/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Adobe Campaign Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Adobe Campaign uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: adobe-campaign-scopes
source_filename: adobe-campaign-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://ims-na1.adobelogin.com/.well-known/openid-configuration (HTTP 200, 2026-08-13)\ndocs: https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/implementation/\nnotes: >-\n  Adobe Campaign's own OpenAPI files declare no oauth2 securityScheme — the\n  Classic specs carry only the session-token apiKey scheme. The OAuth surface is\n  therefore recorded from the authorization server itself: Adobe IMS, which\n  Campaign Standard / Campaign v8 REST calls authenticate against. The IMS\n  discovery document advertises only the three OIDC identity scopes below.\n  Product-level entitlement for Campaign is NOT expressed as an OAuth scope\n  string — it is granted by adding the Adobe Campaign service to an Adobe\n  Developer Console project and is carried in the token's organization claim,\n  which is why there is no per-resource scope catalog to publish. Recording that\n  absence is the\
  \ finding; it is not a gap in our harvest.\nauthorization_server:\n  issuer: https://ims-na1.adobelogin.com\n  authorization_endpoint: https://ims-na1.adobelogin.com/ims/authorize/v2\n  token_endpoint: https://ims-na1.adobelogin.com/ims/token/v3\n  revocation_endpoint: https://ims-na1.adobelogin.com/ims/revoke\n  userinfo_endpoint: https://ims-na1.adobelogin.com/ims/userinfo/v2\n  jwks_uri: https://ims-na1.adobelogin.com/ims/keys\n  registration_endpoint: https://ims-na1.adobelogin.com/ims/register\n  grant_types_supported:\n    - authorization_code\n    - implicit_grant\n    - refresh_token\n  code_challenge_methods_supported:\n    - S256\n    - plain\n  token_endpoint_auth_methods_supported:\n    - client_secret_basic\n    - client_secret_post\nscope_count: 3\nscopes:\n  - name: openid\n    description: OIDC identity scope. Requests an ID token for the authenticated Adobe identity.\n    source: ims discovery scopes_supported\n  - name: email\n    description: Releases the email claim\
  \ on the ID token / userinfo response.\n    source: ims discovery scopes_supported\n  - name: profile\n    description: >-\n      Releases the profile claims (sub, given_name, family_name, name) on the ID\n      token / userinfo response. Unrelated to Adobe Campaign \"profile\" records.\n    source: ims discovery scopes_supported\nnot_scoped:\n  - surface: Campaign Classic SOAP-over-HTTP\n    reason: >-\n      Session-token authentication (xtk:session#Logon) has no OAuth layer and\n      therefore no scopes.\n  - surface: Campaign REST resource permissions\n    reason: >-\n      Campaign APIs run in the administrator context and are excluded from the\n      role context by default, so resource access is not narrowed by a token\n      scope. See authentication/adobe-campaign-authentication.yml#tenancy.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/scopes/adobe-campaign-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
- Transactional Messaging
- Customer Data
- Adobe Experience Cloud
- SMS
- Push Notifications
- Workflow-Automation
- Privacy
token_urls: []
---
