---
authorization_urls: []
description: Scopes named in the auth-code-grant example URL (scopes=account:balance,account:statement,bets). The docs say an application may request any subset of the scopes it has access to; no full scope reference was retrievable. Live TAB Studio docs (www.studio.tab.com.au) answered 403 Akamai Access Denied (geo-restricted) on 2026-10-22; content read from the Internet Archive snapshot of the provider's own docs, captured February 2017, and may be out of date.
docs: https://studio.tab.com.au/intro/authentication/auth-code-grant.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Tabcorp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tabcorp publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tabcorp API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tabcorp
provider_slug: tabcorp
schemes:
- authorizationUrl: https://api.beta.tab.com.au/oauth/authorize
  grant_types:
  - authorization_code
  - refresh_token
  name: TAB Digital API OAuth 2.0
  tokenUrl: https://api.beta.tab.com.au/oauth/token
  type: oauth2
scope_count: 3
scope_names:
- account:balance
- account:statement
- bets
scopes:
- description: Named in the documented authorize URL example; no description published.
  flows: []
  scope: account:balance
- description: Named in the documented authorize URL example; no description published.
  flows: []
  scope: account:statement
- description: Named in the documented authorize URL example; no description published.
  flows: []
  scope: bets
slug: tabcorp-scopes
source_filename: tabcorp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://web.archive.org/web/20170219083244/https://studio.tab.com.au/intro/authentication/auth-code-grant.html\ndocs: https://studio.tab.com.au/intro/authentication/auth-code-grant.html\ndescription: \"Scopes named in the auth-code-grant example URL (scopes=account:balance,account:statement,bets). The docs say an application may request any subset of the scopes it has access to; no full scope reference was retrievable. Live TAB Studio docs (www.studio.tab.com.au) answered 403 Akamai Access Denied (geo-restricted) on 2026-10-22; content read from the Internet Archive snapshot of the provider's own docs, captured February 2017, and may be out of date.\"\nschemes:\n- name: TAB Digital API OAuth 2.0\n  type: oauth2\n  grant_types: [authorization_code, refresh_token]\n  authorizationUrl: https://api.beta.tab.com.au/oauth/authorize\n  tokenUrl: https://api.beta.tab.com.au/oauth/token\nscopes:\n- scope: account:balance\n  description:\
  \ Named in the documented authorize URL example; no description published.\n  schemes: [TAB Digital API OAuth 2.0]\n- scope: account:statement\n  description: Named in the documented authorize URL example; no description published.\n  schemes: [TAB Digital API OAuth 2.0]\n- scope: bets\n  description: Named in the documented authorize URL example; no description published.\n  schemes: [TAB Digital API OAuth 2.0]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabcorp/refs/heads/main/scopes/tabcorp-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Wagering
- Betting
- Gaming
- Media
- Racing
- Australia
token_bound: false
token_urls: []
---
