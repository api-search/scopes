---
authorization_urls:
- https://app.netlify.com/authorize
description: ''
docs: https://docs.netlify.com/api-and-cli-guides/api-guides/get-started-with-api/
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Netlify Scopes
name_suffix: OAuth Scopes
note: Netlify OAuth2 does not use granular scopes - tokens (OAuth or personal access tokens) carry full account access, and Netlify staff confirm only a single public scope exists (https://answers.netlify.com/t/netlify-oauth-scopes/112113).
overview: 'Netlify uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Netlify
provider_slug: netlify
schemes:
- flows:
  - authorizationUrl: https://app.netlify.com/authorize
    flow: implicit
  name: netlifyAuth
  source: openapi/netlify-openapi-original.yml
scope_count: 0
scope_names: []
scopes: []
slug: netlify-scopes
source_filename: netlify-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/netlify-openapi-original.yml\ndocs: https://docs.netlify.com/api-and-cli-guides/api-guides/get-started-with-api/\nnote: Netlify OAuth2 does not use granular scopes - tokens (OAuth or personal access\n  tokens) carry full account access, and Netlify staff confirm only a single public\n  scope exists (https://answers.netlify.com/t/netlify-oauth-scopes/112113).\nschemes:\n- name: netlifyAuth\n  source: openapi/netlify-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://app.netlify.com/authorize\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netlify/refs/heads/main/scopes/netlify-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- CDN
- Cloud
- Continuous Deployment
- Edge Computing
- JAMstack
- Serverless
- Serverless Functions
- Static Sites
- Web Hosting
- Websites
token_urls: []
---
