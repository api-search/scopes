---
api_specs:
- filename: wiktionary-mediawiki-action-api-openapi-original.yml
  format: yaml
  label: MediaWiki Action API (Wiktionary)
  slug: mediawiki-action-api-wiktionary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-mediawiki-action-api-openapi-original.yml
- filename: wiktionary-rest-api-openapi-original.yml
  format: yaml
  label: Wikimedia REST API (Wiktionary)
  slug: wikimedia-rest-api-wiktionary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-rest-api-openapi-original.yml
- filename: wiktionary-core-rest-api-openapi-original.yml
  format: yaml
  label: MediaWiki Core REST API (Wiktionary)
  slug: mediawiki-core-rest-api-wiktionary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-core-rest-api-openapi-original.yml
authorization_urls:
- https://meta.wikimedia.org/w/rest.php/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wiktionary Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wiktionary publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wiktionary API on a user''s behalf.


  Tokens are issued from https://meta.wikimedia.org/w/rest.php/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wiktionary
provider_slug: wiktionary
schemes:
- description: OAuth 2.0 access tokens issued via api.wikimedia.org.
  flows:
  - authorizationUrl: https://meta.wikimedia.org/w/rest.php/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://meta.wikimedia.org/w/rest.php/oauth2/access_token
  name: oauth2
  source: openapi/wiktionary-core-rest-api-openapi-original.yml
- description: OAuth 2.0 access tokens issued via api.wikimedia.org.
  flows:
  - authorizationUrl: https://meta.wikimedia.org/w/rest.php/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://meta.wikimedia.org/w/rest.php/oauth2/access_token
  name: oauth2
  source: openapi/wiktionary-mediawiki-action-api-openapi-original.yml
scope_count: 3
scope_names:
- basic
- createeditmovepage
- highvolume
scopes:
- description: Basic read access to user identity
  flows:
  - authorizationCode
  scope: basic
- description: Create, edit, and move pages
  flows:
  - authorizationCode
  scope: createeditmovepage
- description: Higher rate limits for bot use
  flows:
  - authorizationCode
  scope: highvolume
slug: wiktionary-scopes
source_filename: wiktionary-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wiktionary-core-rest-api-openapi-original.yml, openapi/wiktionary-mediawiki-action-api-openapi-original.yml\nschemes:\n- name: oauth2\n  source: openapi/wiktionary-core-rest-api-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://meta.wikimedia.org/w/rest.php/oauth2/authorize\n    tokenUrl: https://meta.wikimedia.org/w/rest.php/oauth2/access_token\n  description: OAuth 2.0 access tokens issued via api.wikimedia.org.\n- name: oauth2\n  source: openapi/wiktionary-mediawiki-action-api-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://meta.wikimedia.org/w/rest.php/oauth2/authorize\n    tokenUrl: https://meta.wikimedia.org/w/rest.php/oauth2/access_token\n  description: OAuth 2.0 access tokens issued via api.wikimedia.org.\nscopes:\n- scope: basic\n  description: Basic read access to user identity\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/wiktionary-core-rest-api-openapi-original.yml\n  - openapi/wiktionary-mediawiki-action-api-openapi-original.yml\n- scope: createeditmovepage\n  description: Create, edit, and move pages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wiktionary-mediawiki-action-api-openapi-original.yml\n- scope: highvolume\n  description: Higher rate limits for bot use\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wiktionary-mediawiki-action-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/scopes/wiktionary-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Dictionaries
- Open Source
- Wikimedia
- MediaWiki
- Linguistics
- Open Data
- Public APIs
token_urls:
- https://meta.wikimedia.org/w/rest.php/oauth2/access_token
---
