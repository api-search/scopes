---
api_specs:
- filename: google-pagespeed-analysis-api-openapi.yml
  format: yaml
  label: Google PageSpeed Analysis API
  slug: google-pagespeed-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pagespeed/refs/heads/main/openapi/google-pagespeed-analysis-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.google.com/speed/docs/insights/v5/get-started#APIKey
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Google Pagespeed Scopes
name_suffix: OAuth Scopes
note: The refined OpenAPI in this repo declares only apiKey security, so the mechanical derivation (derive-oauth-scopes.py) found zero oauth2 schemes. Google's own Discovery document — revision 20260811, probed 2026-08-13 — does declare an oauth2 block, with a single scope, and attaches that scope to the one method. The documented and recommended path is still the API key; OAuth here only carries an identity assertion, not a resource permission.
overview: 'Google PageSpeed publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google PageSpeed API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google PageSpeed
provider_slug: google-pagespeed
schemes:
- declared_in: auth.oauth2.scopes
  flow_note: Google Discovery documents list scopes without flow definitions; the flows are Google's standard OAuth 2.0 endpoints at accounts.google.com, not published in this document.
  flows: []
  name: oauth2
  source: https://pagespeedonline.googleapis.com/$discovery/rest?version=v5
scope_count: 1
scope_names:
- openid
scopes:
- description: Associate you with your personal info on Google
  flows: []
  scope: openid
slug: google-pagespeed-scopes
source_filename: google-pagespeed-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://pagespeedonline.googleapis.com/$discovery/rest?version=v5\ndocs: https://developers.google.com/speed/docs/insights/v5/get-started#APIKey\nnote: >-\n  The refined OpenAPI in this repo declares only apiKey security, so the mechanical\n  derivation (derive-oauth-scopes.py) found zero oauth2 schemes. Google's own Discovery\n  document — revision 20260811, probed 2026-08-13 — does declare an oauth2 block, with a\n  single scope, and attaches that scope to the one method. The documented and recommended\n  path is still the API key; OAuth here only carries an identity assertion, not a\n  resource permission.\nschemes:\n  - name: oauth2\n    source: https://pagespeedonline.googleapis.com/$discovery/rest?version=v5\n    declared_in: auth.oauth2.scopes\n    flows: []\n    flow_note: >-\n      Google Discovery documents list scopes without flow definitions; the flows are\n      Google's standard OAuth 2.0 endpoints at accounts.google.com,\
  \ not published in this\n      document.\nscopes:\n  - scope: openid\n    description: Associate you with your personal info on Google\n    applies_to: [pagespeedonline.pagespeedapi.runpagespeed]\n    sources:\n      - https://pagespeedonline.googleapis.com/$discovery/rest?version=v5\n    note: >-\n      This is the OIDC identity scope, not a PageSpeed resource permission. The API grants\n      no read/write scope surface — analysis is performed on public URLs and there is no\n      user-owned data to authorize against.\nsummary:\n  scope_count: 1\n  resource_scopes: 0\n  identity_scopes: 1\n  primary_auth: api-key\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-pagespeed/refs/heads/main/scopes/google-pagespeed-scopes.yml
summary_line: 1 scope
tags:
- Core Web Vitals
- Google
- Lighthouse
- Page Speed
- SEO
- Web Performance
token_urls: []
---
