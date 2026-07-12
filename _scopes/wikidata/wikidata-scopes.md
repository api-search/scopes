---
authorization_urls:
- https://www.mediawiki.org/w/index.php?title=Special:OAuth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wikidata Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wikidata publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wikidata API on a user''s behalf.


  Tokens are issued from https://www.mediawiki.org/w/index.php?title=Special:OAuth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wikidata
provider_slug: wikidata
schemes:
- flows:
  - authorizationUrl: https://www.mediawiki.org/w/index.php?title=Special:OAuth/authorize
    flow: authorizationCode
    tokenUrl: https://www.mediawiki.org/w/index.php?title=Special:OAuth/token
  name: OAuth2
  source: openapi/wikidata-mediawiki-openapi.yml
scope_count: 2
scope_names:
- createeditmovepage
- editpage
scopes:
- description: Create new items
  flows:
  - authorizationCode
  scope: createeditmovepage
- description: Edit Wikidata items
  flows:
  - authorizationCode
  scope: editpage
slug: wikidata-scopes
source_filename: wikidata-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wikidata-mediawiki-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/wikidata-mediawiki-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.mediawiki.org/w/index.php?title=Special:OAuth/authorize\n    tokenUrl: https://www.mediawiki.org/w/index.php?title=Special:OAuth/token\nscopes:\n- scope: createeditmovepage\n  description: Create new items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wikidata-mediawiki-openapi.yml\n- scope: editpage\n  description: Edit Wikidata items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wikidata-mediawiki-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikidata/refs/heads/main/scopes/wikidata-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Knowledge Graph
- Linked Data
- Open Data
- Semantic Web
- SPARQL
- Wikipedia
token_urls:
- https://www.mediawiki.org/w/index.php?title=Special:OAuth/token
---
