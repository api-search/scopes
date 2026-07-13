---
api_specs:
- filename: paylocity-openapi.yml
  format: yaml
  label: Paylocity Integrations REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paylocity/refs/heads/main/openapi/paylocity-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.paylocity.com/integrations/reference/authentication-weblink
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Paylocity Scopes
name_suffix: OAuth Scopes
note: Paylocity's Next Gen Integrations API authentication docs (https://developer.paylocity.com/integrations/reference/authentication) use the OAuth 2.0 client credentials grant without documenting granular scopes; WebLinkAPI is the only documented scope value, required for the legacy Weblink API token request.
overview: 'Paylocity publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Paylocity API on a user''s behalf.


  Tokens are issued from https://api.paylocity.com/IdentityServer/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paylocity
provider_slug: paylocity
schemes:
- description: OAuth 2.0 client credentials grant. Credentials are provisioned by Paylocity.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.paylocity.com/IdentityServer/connect/token
  name: oauth2ClientCredentials
  source: openapi/paylocity-openapi.yml
scope_count: 1
scope_names:
- WebLinkAPI
scopes:
- description: Required scope for token requests to the Paylocity Weblink API via the client credentials grant; the scope parameter of the token request must be set to WebLinkAPI.
  flows: []
  scope: WebLinkAPI
slug: paylocity-scopes
source_filename: paylocity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/paylocity-openapi.yml\ndocs: https://developer.paylocity.com/integrations/reference/authentication-weblink\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/paylocity-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.paylocity.com/IdentityServer/connect/token\n  description: OAuth 2.0 client credentials grant. Credentials are provisioned by Paylocity.\nscopes:\n- scope: WebLinkAPI\n  description: Required scope for token requests to the Paylocity Weblink API via\n    the client credentials grant; the scope parameter of the token request must be\n    set to WebLinkAPI.\n  sources:\n  - https://developer.paylocity.com/integrations/reference/authentication-weblink\nnote: Paylocity's Next Gen Integrations API authentication docs (https://developer.paylocity.com/integrations/reference/authentication)\n  use the OAuth 2.0 client credentials grant without documenting granular scopes;\n\
  \  WebLinkAPI is the only documented scope value, required for the legacy Weblink API\n  token request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paylocity/refs/heads/main/scopes/paylocity-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- HR
- Payroll
- HCM
- Benefits
- Workforce Management
- Time Tracking
token_urls:
- https://api.paylocity.com/IdentityServer/connect/token
---
