---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Adobe Photoshop API
  slug: adobe-photoshop-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/photoshop/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Adobe Lightroom API
  slug: adobe-lightroom-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/lightroom/api/openapi/
- filename: adobe-suite-firefly-illustrator-openapi.json
  format: json
  label: Adobe Illustrator API
  slug: adobe-illustrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-illustrator-openapi.json
- filename: adobe-suite-firefly-indesign-openapi.json
  format: json
  label: Adobe InDesign API
  slug: adobe-indesign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-indesign-openapi.json
- filename: openapi.yaml
  format: yaml
  label: Adobe PDF Services API
  slug: adobe-pdf-services-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/document-services/docs/apis/
- filename: openapi.yaml
  format: yaml
  label: Adobe PDF Extract API
  slug: adobe-pdf-extract-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/document-services/docs/apis/
- filename: openapi.yaml
  format: yaml
  label: Adobe PDF Accessibility Auto-Tag API
  slug: adobe-pdf-accessibility-auto-tag-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/document-services/docs/apis/
- filename: adobe-suite-analytics-openapi.json
  format: json
  label: Adobe Analytics API
  slug: adobe-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-analytics-openapi.json
- filename: adobe-suite-firefly-openapi.json
  format: json
  label: Adobe Firefly API
  slug: adobe-firefly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-openapi.json
- filename: adobe-suite-firefly-audio-video-openapi.json
  format: json
  label: Adobe Firefly Audio/Video APIs
  slug: adobe-firefly-audiovideo-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-audio-video-openapi.json
- filename: adobe-suite-cc-libraries-openapi.json
  format: json
  label: Adobe Creative Cloud Libraries API
  slug: adobe-creative-cloud-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-cc-libraries-openapi.json
- filename: adobe-suite-firefly-express-openapi.json
  format: json
  label: Adobe Express Embed SDK
  slug: adobe-express-embed-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-express-openapi.json
- filename: adobe-suite-aep-schema-registry-openapi.yaml
  format: yaml
  label: Adobe Experience Platform API
  slug: adobe-experience-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-aep-schema-registry-openapi.yaml
- filename: adobe-suite-marketo-identity-openapi.json
  format: json
  label: Adobe Marketo Engage API
  slug: adobe-marketo-engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-marketo-identity-openapi.json
- filename: adobe-suite-commerce-rest-guest-openapi.yaml
  format: yaml
  label: Adobe Commerce API
  slug: adobe-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-commerce-rest-guest-openapi.yaml
- filename: adobe-suite-cloud-manager-openapi.yaml
  format: yaml
  label: Adobe Cloud Manager API
  slug: adobe-cloud-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-cloud-manager-openapi.yaml
- filename: adobe-suite-journey-optimizer-campaigns-retrieve-openapi.yaml
  format: yaml
  label: Adobe Journey Optimizer API
  slug: adobe-journey-optimizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-journey-optimizer-campaigns-retrieve-openapi.yaml
- filename: adobe-suite-workfront-workflow-openapi.json
  format: json
  label: Adobe Workfront API
  slug: adobe-workfront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-workfront-workflow-openapi.json
- filename: adobe-suite-firefly-substance-3d-openapi.yaml
  format: yaml
  label: Adobe Substance 3D API
  slug: adobe-substance-3d-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-firefly-substance-3d-openapi.yaml
- filename: adobe-suite-data-collection-openapi.yaml
  format: yaml
  label: Adobe Experience Platform Edge Network API
  slug: adobe-experience-platform-edge-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-data-collection-openapi.yaml
- filename: adobe-suite-status-openapi.yaml
  format: yaml
  label: Adobe Status API
  slug: adobe-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-status-openapi.yaml
- filename: adobe-suite-vip-marketplace-partners-openapi.json
  format: json
  label: Adobe VIP Marketplace Partner API
  slug: adobe-vip-marketplace-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/openapi/adobe-suite-vip-marketplace-partners-openapi.json
authorization_urls: []
description: ''
docs: https://developer.adobe.com/developer-console/docs/guides/authentication/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Adobe Suite Scopes
name_suffix: OAuth Scopes
note: 'None of the 70 harvested Adobe OpenAPI documents declares an `oauth2` securityScheme — every spec models auth as an apiKey header (`x-api-key`) plus an HTTP bearer token, so a spec-only derivation would report zero scopes. The scopes below are real: they are quoted from Adobe''s own Firefly Services getting-started guide and corroborated by the live OIDC discovery document at ims-na1.adobelogin.com. This is the gap worth naming — Adobe runs a full OAuth 2.0 / OIDC authorization server (IMS) but does not express it in any published contract.'
overview: 'Adobe Suite publishes 10 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Adobe Suite API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adobe Suite
provider_slug: adobe-suite
schemes:
- grant: client_credentials
  name: Adobe IMS OAuth Server-to-Server
  request_verbatim: curl -X POST 'https://ims-na1.adobelogin.com/ims/token/v3' -d 'grant_type=client_credentials&client_id=<YOUR_CLIENT_ID>&client_secret=<YOUR_CLIENT_SECRET>&scope=openid,AdobeID,session,additional_info,read_organizations,firefly_api,ff_apis'
  source: https://raw.githubusercontent.com/AdobeDocs/ff-services-docs/main/src/pages/guides/get-started.md
  token_endpoint: https://ims-na1.adobelogin.com/ims/token/v3
  token_lifetime: 24 hours
- authorization_endpoint: https://ims-na1.adobelogin.com/ims/authorize/v2
  grant: authorization_code
  name: Adobe IMS User Authentication (OAuth Web / SPA / Native App)
  source: https://developer.adobe.com/developer-console/docs/guides/authentication/
  token_endpoint: https://ims-na1.adobelogin.com/ims/token/v3
scope_count: 10
scope_names:
- openid
- AdobeID
- session
- additional_info
- read_organizations
- firefly_api
- ff_apis
- email
- profile
- additional_info.projectedProductContext
scopes:
- description: Standard OIDC scope. Returns an ID token identifying the authenticated principal.
  flows:
  - client_credentials
  - authorization_code
  scope: openid
- description: Core Adobe identity scope. Required on virtually every Adobe API integration.
  flows:
  - client_credentials
  - authorization_code
  scope: AdobeID
- description: Establishes an Adobe IMS session alongside the issued token.
  flows:
  - client_credentials
  scope: session
- description: Returns additional profile information on the token/userinfo response.
  flows:
  - client_credentials
  scope: additional_info
- description: Read the Adobe organizations (IMS Orgs) the credential is entitled to act on behalf of.
  flows:
  - client_credentials
  scope: read_organizations
- description: Access to the Adobe Firefly generative APIs (image, video, custom models).
  flows:
  - client_credentials
  scope: firefly_api
- description: Access to the wider Firefly Services API family (Photoshop, Lightroom, Illustrator, InDesign, Express, Substance 3D, audio/video).
  flows:
  - client_credentials
  scope: ff_apis
- description: OIDC email claim.
  flows:
  - authorization_code
  scope: email
- description: OIDC profile claims.
  flows:
  - authorization_code
  scope: profile
- description: Returns the product context array for the authenticated user — which Adobe products and entitlements they hold. Widely required by Experience Cloud APIs (Analytics, Target, Experience Platform).
  flows:
  - authorization_code
  - client_credentials
  scope: additional_info.projectedProductContext
slug: adobe-suite-scopes
source_filename: adobe-suite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://raw.githubusercontent.com/AdobeDocs/ff-services-docs/main/src/pages/guides/get-started.md\ndocs: https://developer.adobe.com/developer-console/docs/guides/authentication/\ndiscovery: https://ims-na1.adobelogin.com/.well-known/openid-configuration\nnote: >-\n  None of the 70 harvested Adobe OpenAPI documents declares an `oauth2` securityScheme —\n  every spec models auth as an apiKey header (`x-api-key`) plus an HTTP bearer token, so\n  a spec-only derivation would report zero scopes. The scopes below are real: they are\n  quoted from Adobe's own Firefly Services getting-started guide and corroborated by the\n  live OIDC discovery document at ims-na1.adobelogin.com. This is the gap worth naming —\n  Adobe runs a full OAuth 2.0 / OIDC authorization server (IMS) but does not express it\n  in any published contract.\nauthorization_server:\n  issuer: https://ims-na1.adobelogin.com\n  authorization_endpoint: https://ims-na1.adobelogin.com/ims/authorize/v2\n\
  \  token_endpoint: https://ims-na1.adobelogin.com/ims/token/v3\n  jwks_uri: https://ims-na1.adobelogin.com/ims/keys\n  revocation_endpoint: https://ims-na1.adobelogin.com/ims/revoke\n  userinfo_endpoint: https://ims-na1.adobelogin.com/ims/userinfo/v2\n  registration_endpoint: https://ims-na1.adobelogin.com/ims/register\n  grant_types_supported: [authorization_code, implicit_grant, refresh_token]\n  code_challenge_methods_supported: [S256, plain]\n  discovery_scopes_supported: [openid, email, profile]\n  note: >-\n    `discovery_scopes_supported` is what RFC 8414 discovery advertises. It is a strict\n    subset of what Adobe actually documents for API access (below) — the product scopes\n    are not published in the discovery document.\nschemes:\n- name: Adobe IMS OAuth Server-to-Server\n  grant: client_credentials\n  token_endpoint: https://ims-na1.adobelogin.com/ims/token/v3\n  token_lifetime: 24 hours\n  source: https://raw.githubusercontent.com/AdobeDocs/ff-services-docs/main/src/pages/guides/get-started.md\n\
  \  request_verbatim: >-\n    curl -X POST 'https://ims-na1.adobelogin.com/ims/token/v3' -d\n    'grant_type=client_credentials&client_id=<YOUR_CLIENT_ID>&client_secret=<YOUR_CLIENT_SECRET>&scope=openid,AdobeID,session,additional_info,read_organizations,firefly_api,ff_apis'\n- name: Adobe IMS User Authentication (OAuth Web / SPA / Native App)\n  grant: authorization_code\n  authorization_endpoint: https://ims-na1.adobelogin.com/ims/authorize/v2\n  token_endpoint: https://ims-na1.adobelogin.com/ims/token/v3\n  source: https://developer.adobe.com/developer-console/docs/guides/authentication/\nscopes:\n- scope: openid\n  description: Standard OIDC scope. Returns an ID token identifying the authenticated principal.\n  flows: [client_credentials, authorization_code]\n  sources: [ims-openid-configuration, ff-services-docs]\n- scope: AdobeID\n  description: Core Adobe identity scope. Required on virtually every Adobe API integration.\n  flows: [client_credentials, authorization_code]\n  sources:\
  \ [ff-services-docs]\n- scope: session\n  description: Establishes an Adobe IMS session alongside the issued token.\n  flows: [client_credentials]\n  sources: [ff-services-docs]\n- scope: additional_info\n  description: Returns additional profile information on the token/userinfo response.\n  flows: [client_credentials]\n  sources: [ff-services-docs]\n- scope: read_organizations\n  description: Read the Adobe organizations (IMS Orgs) the credential is entitled to act on behalf of.\n  flows: [client_credentials]\n  sources: [ff-services-docs]\n- scope: firefly_api\n  description: Access to the Adobe Firefly generative APIs (image, video, custom models).\n  flows: [client_credentials]\n  sources: [ff-services-docs]\n- scope: ff_apis\n  description: Access to the wider Firefly Services API family (Photoshop, Lightroom, Illustrator, InDesign, Express, Substance 3D, audio/video).\n  flows: [client_credentials]\n  sources: [ff-services-docs]\n- scope: email\n  description: OIDC email claim.\n\
  \  flows: [authorization_code]\n  sources: [ims-openid-configuration]\n- scope: profile\n  description: OIDC profile claims.\n  flows: [authorization_code]\n  sources: [ims-openid-configuration]\n- scope: additional_info.projectedProductContext\n  description: >-\n    Returns the product context array for the authenticated user — which Adobe products and\n    entitlements they hold. Widely required by Experience Cloud APIs (Analytics, Target,\n    Experience Platform).\n  flows: [authorization_code, client_credentials]\n  sources: [adobe-developer-console-docs]\ngaps:\n- >-\n  Adobe documents \"View scopes per service\" as an interactive control inside the Developer\n  Console rather than as a published scope reference page, so the complete per-product scope\n  list is only visible to a signed-in developer with a project. The scopes above are the ones\n  Adobe publishes in open documentation.\n- >-\n  No OpenAPI in openapi/ declares an oauth2 securityScheme, so no operation-level scope\n\
  \  requirement can be derived. An agent cannot compute least-privilege from Adobe's contracts.\nsummary:\n  scope_count: 10\n  oauth2_in_openapi: false\n  oidc_discovery_live: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-suite/refs/heads/main/scopes/adobe-suite-scopes.yml
summary_line: 10 scopes
tags:
- Artificial Intelligence
- Analytics
- Automation
- Commerce
- Creative
- Design
- Documents
- Experience
- Marketing
- Personalization
- Video
token_urls: []
---
