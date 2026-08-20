---
authorization_urls: []
description: The only scopes Botkeeper publishes anywhere are the four standard OpenID Connect scopes advertised by its production Amazon Cognito user pool's discovery document. Botkeeper documents no resource-server scopes, no permission model, and no scope reference page. Nothing below is invented — the list is verbatim from scopes_supported in the discovery document.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Botkeeper Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Botkeeper uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Botkeeper
provider_slug: botkeeper
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: botkeeper-scopes
source_filename: botkeeper-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_MZqyuuurX/.well-known/openid-configuration\nname: Botkeeper OAuth / OIDC scopes\ndescription: >-\n  The only scopes Botkeeper publishes anywhere are the four standard OpenID\n  Connect scopes advertised by its production Amazon Cognito user pool's\n  discovery document. Botkeeper documents no resource-server scopes, no\n  permission model, and no scope reference page. Nothing below is invented — the\n  list is verbatim from scopes_supported in the discovery document.\n\nauthorization_server:\n  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_MZqyuuurX\n  authorization_endpoint: https://login.auth.firm.ai/oauth2/authorize\n  token_endpoint: https://login.auth.firm.ai/oauth2/token\n  flows: [authorization_code, implicit]\n  response_types_supported: [code, token]\n\nscopes:\n  - name: openid\n    description: Standard OIDC scope — requests an ID token for the authenticated\
  \ user.\n    standard: true\n  - name: email\n    description: Standard OIDC scope — releases the email and email_verified claims.\n    standard: true\n  - name: phone\n    description: Standard OIDC scope — releases the phone_number and phone_number_verified claims.\n    standard: true\n  - name: profile\n    description: Standard OIDC scope — releases the standard profile claims.\n    standard: true\n\ncustom_scopes: []\n\ndocs: null\n\ngaps:\n  - >-\n    No resource-server (custom) scopes are advertised. The Botkeeper Partner\n    Platform API on ipa.botkeeper.com is protected by an API Gateway authorizer,\n    but no scope taxonomy for it is published.\n  - No scopes/permissions reference page exists on botkeeper.com.\n  - >-\n    Least-privilege delegation is therefore not expressible against Botkeeper —\n    a third party can only receive whole-user identity, not a scoped grant.\n\nx-evidence:\n  fetched: '2026-08-08'\n  probes:\n    - url: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_MZqyuuurX/.well-known/openid-configuration\n\
  \      status: 200\n      content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botkeeper/refs/heads/main/scopes/botkeeper-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Accounting
- Bookkeeping
- Financial-Services
- Artificial Intelligence
- Automation
- Software-as-a-Service
- Banking Data
- Practice Management
- Small Business
token_urls: []
---
