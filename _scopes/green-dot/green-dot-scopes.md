---
authorization_urls: []
description: ''
docs: https://developer.greendot.com/embedded-finance/docs/baas-api-authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Green Dot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Green Dot Corporation publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Green Dot Corporation API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Green Dot Corporation
provider_slug: green-dot
schemes:
- flow: clientCredentials
  name: oauth2ClientCredentials
  scope_parameter: optional
  scope_style: space-delimited
  token_endpoint: '{BaasUrl}/authentication'
scope_count: 3
scope_names:
- general
- demo
- post:webhook
scopes:
- description: Baseline granted scope observed in the documented authentication example token response. Exact grants are partner/program specific.
  flows: []
  scope: general
- description: Demo/sandbox scope observed in the documented example token response.
  flows: []
  scope: demo
- description: Scope used to obtain a token for the partner-hosted webhook delivery surface (bank-events auth), per the Webhooks Overview.
  flows: []
  scope: post:webhook
slug: green-dot-scopes
source_filename: green-dot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.greendot.com/embedded-finance/docs/baas-api-authentication\ndocs: https://developer.greendot.com/embedded-finance/docs/baas-api-authentication\nsummary: >-\n  Green Dot BaaS OAuth 2.0 uses the client-credentials flow with an optional,\n  space-delimited scope parameter on the token request; the granted scope is\n  returned on the token response (e.g. \"general demo\"). The public developer\n  portal does not publish a full scope catalog — scopes are provisioned per\n  partner/program during commercial onboarding and constrain a credential to\n  its authorized product surface (\"out of credential scopes\" 401 on overreach).\n  Webhook delivery uses a distinct token scope (post:webhook).\nschemes:\n  - name: oauth2ClientCredentials\n    flow: clientCredentials\n    token_endpoint: '{BaasUrl}/authentication'\n    scope_parameter: optional\n    scope_style: space-delimited\nscopes:\n  - scope: general\n    description:\
  \ >-\n      Baseline granted scope observed in the documented authentication example\n      token response. Exact grants are partner/program specific.\n    source: docs\n  - scope: demo\n    description: Demo/sandbox scope observed in the documented example token response.\n    source: docs\n  - scope: 'post:webhook'\n    description: >-\n      Scope used to obtain a token for the partner-hosted webhook delivery\n      surface (bank-events auth), per the Webhooks Overview.\n    source: https://developer.greendot.com/embedded-finance/docs/webhooks-overview\nnotes: >-\n  No exhaustive scope/permission reference is published publicly; the full set\n  is defined per partner program. This artifact captures the scope MODEL and the\n  scopes named in Green Dot's own documentation — no scopes were invented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-dot/refs/heads/main/scopes/green-dot-scopes.yml
summary_line: 3 scopes
tags:
- Fintech
- Banking as a Service
- Embedded Finance
- Prepaid Cards
- Banking
- Payments
- Money Movement
- United States
token_urls: []
---
