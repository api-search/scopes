---
api_specs:
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Members API
  slug: yourmembership-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Events API
  slug: yourmembership-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Certifications API
  slug: yourmembership-certifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YMCareers API
  slug: yourmembership-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Content and Community API
  slug: yourmembership-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
- filename: yourmembership-openapi.yml
  format: yaml
  label: YourMembership Commerce and Sales API
  slug: yourmembership-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/openapi/yourmembership-openapi.yml
authorization_urls:
- https://{your-ym-site}/lock.aspx
description: ''
docs: https://www.yourmembership.com/wp-content/uploads/2021/02/YM_Getting_Started_OAuth_2021.pdf
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Yourmembership Scopes
name_suffix: OAuth Scopes
note: These two scopes are the only ones published in YourMembership's Getting Started with OAuth guide; the REST API also exposes a GET /Ams/{ClientID}/OAuthScopes metadata operation (ScopeID, ScopeName, DisplayName, IsDefault, GranularScope) indicating scopes are managed per-site in OAuth Management, but no additional scope values are publicly documented.
overview: 'YourMembership publishes 2 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the YourMembership API on a user''s behalf.


  Tokens are issued from https://ws.yourmembership.com/Ams/Authenticate.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: YourMembership
provider_slug: yourmembership
schemes:
- description: OAuth authentication for the YM REST API, established via POST /Ams/Authenticate. OAuth apps are configured in YM (API Configuration > OAuth Management); the member authorizes the app at the site's lock.aspx page with app_id, redirect_uri, and scope parameters, the returned code is exchanged at POST /OAuth/GetAccessToken, and the access token is passed to POST /Ams/Authenticate to create the API session (X-SS-ID header). The YMCareers API instead uses an API_ACCESS_TOKEN (15-minute) Authorization header or a non-expiring X-API-KEY header.
  flows:
  - flow: clientCredentials
    tokenUrl: https://ws.yourmembership.com/Ams/Authenticate
  - authorizationUrl: https://{your-ym-site}/lock.aspx
    flow: authorizationCode
    source: https://www.yourmembership.com/wp-content/uploads/2021/02/YM_Getting_Started_OAuth_2021.pdf
    tokenUrl: https://ws.yourmembership.com/OAuth/GetAccessToken
  name: oauth2
  source: openapi/yourmembership-openapi.yml
scope_count: 2
scope_names:
- basic_profile
- full_profile
scopes:
- description: Grants access to the authorized member's basic profile information via the BasicMemberProfile service (GET /Ams/{ClientID}/Member/{MemberID}/BasicMemberProfile).
  flows: []
  scope: basic_profile
- description: Grants access to the authorized member's full profile information via the MemberProfile service; required when an app needs more than the basic profile fields.
  flows: []
  scope: full_profile
slug: yourmembership-scopes
source_filename: yourmembership-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/yourmembership-openapi.yml\ndocs: https://www.yourmembership.com/wp-content/uploads/2021/02/YM_Getting_Started_OAuth_2021.pdf\nschemes:\n- name: oauth2\n  source: openapi/yourmembership-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ws.yourmembership.com/Ams/Authenticate\n  - flow: authorizationCode\n    authorizationUrl: https://{your-ym-site}/lock.aspx\n    tokenUrl: https://ws.yourmembership.com/OAuth/GetAccessToken\n    source: https://www.yourmembership.com/wp-content/uploads/2021/02/YM_Getting_Started_OAuth_2021.pdf\n  description: OAuth authentication for the YM REST API, established via POST /Ams/Authenticate.\n    OAuth apps are configured in YM (API Configuration > OAuth Management); the member authorizes\n    the app at the site's lock.aspx page with app_id, redirect_uri, and scope parameters, the\n    returned code is exchanged at POST /OAuth/GetAccessToken, and the access token\
  \ is passed to\n    POST /Ams/Authenticate to create the API session (X-SS-ID header). The YMCareers API instead\n    uses an API_ACCESS_TOKEN (15-minute) Authorization header or a non-expiring X-API-KEY header.\nscopes:\n- scope: basic_profile\n  description: Grants access to the authorized member's basic profile information via the\n    BasicMemberProfile service (GET /Ams/{ClientID}/Member/{MemberID}/BasicMemberProfile).\n  sources:\n  - https://www.yourmembership.com/wp-content/uploads/2021/02/YM_Getting_Started_OAuth_2021.pdf\n- scope: full_profile\n  description: Grants access to the authorized member's full profile information via the\n    MemberProfile service; required when an app needs more than the basic profile fields.\n  sources:\n  - https://www.yourmembership.com/wp-content/uploads/2021/02/YM_Getting_Started_OAuth_2021.pdf\nnote: These two scopes are the only ones published in YourMembership's Getting Started with\n  OAuth guide; the REST API also exposes a GET /Ams/{ClientID}/OAuthScopes\
  \ metadata operation\n  (ScopeID, ScopeName, DisplayName, IsDefault, GranularScope) indicating scopes are managed\n  per-site in OAuth Management, but no additional scope values are publicly documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yourmembership/refs/heads/main/scopes/yourmembership-scopes.yml
summary_line: 2 scopes · clientCredentials/authorizationCode
tags:
- Membership Management
- Association Management
- AMS
- Nonprofit
- Events
- Careers
- Community Brands
- Momentive Software
token_urls:
- https://ws.yourmembership.com/Ams/Authenticate
- https://ws.yourmembership.com/OAuth/GetAccessToken
---
