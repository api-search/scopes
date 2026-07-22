---
authorization_urls: []
description: ''
docs: https://dev.proof.com/docs/oauth-client-credentials
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Notarize Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Notarize publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Notarize API on a user''s behalf.


  Tokens are issued from https://api.proof.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Notarize
provider_slug: notarize
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.proof.com/oauth/v2/token
  name: OAuth2
  source: https://dev.proof.com/docs/oauth-client-credentials
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to Proof API resources.
  flows:
  - clientCredentials
  scope: read
- description: Write access to create and modify Proof API resources.
  flows:
  - clientCredentials
  scope: write
slug: notarize-scopes
source_filename: notarize-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://dev.proof.com/docs/oauth-client-credentials\ndocs: https://dev.proof.com/docs/oauth-client-credentials\nnotes: >-\n  Proof's OAuth 2.0 client_credentials grant issues tokens with a coarse\n  read/write scope pair (seen in the token and token/info responses:\n  \"scope\":\"read write\"). Proof does not publish a fine-grained per-resource\n  scope catalog; access is primarily differentiated by API-key access level\n  (Full Access vs Client Only) rather than OAuth scopes.\nschemes:\n  - name: OAuth2\n    source: https://dev.proof.com/docs/oauth-client-credentials\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.proof.com/oauth/v2/token\nscopes:\n  - scope: read\n    description: Read access to Proof API resources.\n    flows: [clientCredentials]\n    sources: [https://dev.proof.com/docs/oauth-client-credentials]\n  - scope: write\n    description: Write access to create and modify Proof API resources.\n\
  \    flows: [clientCredentials]\n    sources: [https://dev.proof.com/docs/oauth-client-credentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/scopes/notarize-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Proptech
- Notarization
- Remote Online Notarization
- Identity Verification
- eSignature
- Digital Credentials
- Real Estate
- Mortgage
- Legal Tech
token_urls:
- https://api.proof.com/oauth/v2/token
---
