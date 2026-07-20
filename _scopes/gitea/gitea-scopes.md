---
api_specs:
- filename: swagger
  format: yaml
  label: Gitea REST API
  slug: gitea-rest-api
  spec_type: OpenAPI
  url: https://demo.gitea.com/api/swagger
authorization_urls: []
description: ''
docs: https://docs.gitea.com/development/oauth2-provider
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Gitea Scopes
name_suffix: OAuth Scopes
note: Gitea exposes two distinct scope systems. (1) OAuth2 / OpenID Connect provider scopes returned in the live openid-configuration. (2) Personal Access Token (PAT) permission scopes, formatted <read|write>:<category>, plus a special `all` scope. The Swagger 2.0 spec declares only apiKey/basic securityDefinitions (no oauth2 flow object), so these scopes are documented rather than derivable from the spec.
overview: 'Gitea uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gitea
provider_slug: gitea
schemes:
- authorizationUrl: https://gitea.com/login/oauth/authorize
  grantTypes:
  - authorization_code
  - refresh_token
  introspectionUrl: https://gitea.com/login/oauth/introspect
  issuer: https://gitea.com
  jwksUri: https://gitea.com/login/oauth/keys
  name: OpenIDConnect
  pkce:
  - plain
  - S256
  source: well-known/gitea-openid-configuration.json
  tokenUrl: https://gitea.com/login/oauth/access_token
  type: openIdConnect
  userinfoUrl: https://gitea.com/login/oauth/userinfo
scope_count: 0
scope_names: []
scopes: []
slug: gitea-scopes
source_filename: gitea-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: well-known/gitea-openid-configuration.json\ndocs: https://docs.gitea.com/development/oauth2-provider\nnote: >-\n  Gitea exposes two distinct scope systems. (1) OAuth2 / OpenID Connect provider\n  scopes returned in the live openid-configuration. (2) Personal Access Token\n  (PAT) permission scopes, formatted <read|write>:<category>, plus a special\n  `all` scope. The Swagger 2.0 spec declares only apiKey/basic securityDefinitions\n  (no oauth2 flow object), so these scopes are documented rather than derivable\n  from the spec.\nschemes:\n  - name: OpenIDConnect\n    type: openIdConnect\n    issuer: https://gitea.com\n    authorizationUrl: https://gitea.com/login/oauth/authorize\n    tokenUrl: https://gitea.com/login/oauth/access_token\n    userinfoUrl: https://gitea.com/login/oauth/userinfo\n    introspectionUrl: https://gitea.com/login/oauth/introspect\n    jwksUri: https://gitea.com/login/oauth/keys\n    grantTypes: [authorization_code,\
  \ refresh_token]\n    pkce: [plain, S256]\n    source: well-known/gitea-openid-configuration.json\noidc_scopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token.\n  - scope: profile\n    description: Access to the user's profile claims (name, preferred_username, picture, website, locale).\n  - scope: email\n    description: Access to the user's email and email_verified claims.\n  - scope: groups\n    description: Access to the user's group membership claim.\npat_scope_categories:\n  note: >-\n    Each category is grantable at read or write level, e.g. read:repository,\n    write:issue. The `all` scope grants read+write across every category.\n  levels: [read, write]\n  categories:\n    - activitypub\n    - admin\n    - issue\n    - misc\n    - notification\n    - organization\n    - package\n    - repository\n    - user\n  special:\n    - scope: all\n      description: Grants both read and write permission across all categories.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/scopes/gitea-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Git
- Source Control
- DevOps
- CI/CD
- Code Hosting
- Open Source
- Self Hosted
- Package Registry
- Issue Tracking
- Pull Requests
token_urls: []
---
