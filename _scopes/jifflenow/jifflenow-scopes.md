---
authorization_urls: []
description: ''
docs: https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Jifflenow Scopes
name_suffix: OAuth Scopes
note: 'Jifflenow documents OAuth 2.0 but publishes no scope reference page and no OpenAPI, so there is no enumerable scope catalog. Scopes are granted implicitly: at integration setup the tenant admin picks which Jifflenow APIs the integration may call and the docs state that this "adds the required scopes to your credentials". The only scope value the documentation actually shows is the one returned in the sample token response.'
overview: 'Jifflenow publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jifflenow API on a user''s behalf.


  Tokens are issued from https://<companyname>.jifflenow.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jifflenow
provider_slug: jifflenow
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://<companyname>.jifflenow.com/api/oauth/token
  name: OAuth2 Client Credentials
  source: https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started
scope_count: 1
scope_names:
- public
scopes:
- description: The scope value shown in the documented sample token response. The docs gloss it as "limited access to public resources". No other scope string appears anywhere in the published reference.
  flows:
  - clientCredentials
  scope: public
slug: jifflenow-scopes
source_filename: jifflenow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started\ndocs: https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started\nnote: >-\n  Jifflenow documents OAuth 2.0 but publishes no scope reference page and no OpenAPI, so there is no\n  enumerable scope catalog. Scopes are granted implicitly: at integration setup the tenant admin\n  picks which Jifflenow APIs the integration may call and the docs state that this \"adds the\n  required scopes to your credentials\". The only scope value the documentation actually shows is the\n  one returned in the sample token response.\nschemes:\n  - name: OAuth2 Client Credentials\n    source: https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://<companyname>.jifflenow.com/api/oauth/token\nscopes:\n  - scope: public\n    description: >-\n      The scope value shown\
  \ in the documented sample token response. The docs gloss it as \"limited\n      access to public resources\". No other scope string appears anywhere in the published reference.\n    flows: [clientCredentials]\n    sources: [https://developers.cvent.com/docs/legacy-api/jifflenow-api/getting-started]\nscope_model:\n  enumerable: false\n  granted_by: >-\n    Per-integration API selection in the Jifflenow admin UI (Settings -> Integrations), not by a\n    scope string the client requests.\n  reference_page: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jifflenow/refs/heads/main/scopes/jifflenow-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Automation
- Event
- Meetings
- Scheduling
- Event Marketing
- B2B
- Sales
- Trade Shows
- Meeting Automation
- Appointments
- Badge Scanning
token_urls:
- https://<companyname>.jifflenow.com/api/oauth/token
---
