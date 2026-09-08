---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Venn Scopes
name_suffix: OAuth Scopes
note: 'Venn publishes no scopes or permissions reference. The scopes below are the standard OpenID Connect scopes advertised by the AWS Cognito user pool that Venn''s own operator dashboard names as its identity provider — they are identity scopes, not API authorization scopes. Venn''s tenant GraphQL API does not use OAuth scopes to authorize data access; the schema models authorization as role rows (`Role`) scoped to a community (`hood`), so there is nothing scope-like in the contract to enumerate. Nothing here is invented: no custom resource server scopes were advertised, and none are asserted.'
overview: 'Venn uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Venn
provider_slug: venn
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: venn-scopes
source_filename: venn-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_cH7XNjcIx/.well-known/openid-configuration\nnote: >-\n  Venn publishes no scopes or permissions reference. The scopes below are the\n  standard OpenID Connect scopes advertised by the AWS Cognito user pool that\n  Venn's own operator dashboard names as its identity provider — they are identity\n  scopes, not API authorization scopes. Venn's tenant GraphQL API does not use\n  OAuth scopes to authorize data access; the schema models authorization as\n  role rows (`Role`) scoped to a community (`hood`), so there is nothing scope-like\n  in the contract to enumerate. Nothing here is invented: no custom resource\n  server scopes were advertised, and none are asserted.\nauthorization_model: role-based (Role rows scoped to hood/community), not scope-based\noauth:\n  issuer: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_cH7XNjcIx\n  authorization_endpoint: https://admin-tool.auth.eu-central-1.amazoncognito.com/oauth2/authorize\n\
  \  token_endpoint: https://admin-tool.auth.eu-central-1.amazoncognito.com/oauth2/token\n  userinfo_endpoint: https://admin-tool.auth.eu-central-1.amazoncognito.com/oauth2/userInfo\n  revocation_endpoint: https://admin-tool.auth.eu-central-1.amazoncognito.com/oauth2/revoke\nscopes:\n  - name: openid\n    description: Standard OIDC scope. Requests an ID token identifying the end user.\n    source: cognito-openid-configuration\n  - name: email\n    description: Standard OIDC scope. Releases the email and email_verified claims.\n    source: cognito-openid-configuration\n  - name: phone\n    description: Standard OIDC scope. Releases the phone_number and phone_number_verified claims.\n    source: cognito-openid-configuration\n  - name: profile\n    description: Standard OIDC scope. Releases the basic profile claims.\n    source: cognito-openid-configuration\ncustom_scopes: []\ncustom_scopes_note: >-\n  No custom (resource-server) scopes are advertised by the pool's discovery\n  document. If\
  \ Venn defines any, they are not publicly discoverable.\nscope_count: 4\ndocs: null\ndocs_note: No public scopes/permissions reference page exists on any Venn host.\nx-evidence:\n  checked: '2026-09-02'\n  evidence:\n    - url: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_cH7XNjcIx/.well-known/openid-configuration\n      status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venn/refs/heads/main/scopes/venn-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Real Estate
- Property Management
- Multifamily
- Resident Experience
- Proptech
- Leasing
- Community
- Payments
- GraphQL
- Mobile Apps
token_urls: []
---
