---
authorization_urls:
- https://oauth.oclc.org/auth
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Worldcat Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'WorldCat publishes 26 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the WorldCat API on a user''s behalf.


  Tokens are issued from https://oauth.oclc.org/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: WorldCat
provider_slug: worldcat
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.oclc.org/token
  - authorizationUrl: https://oauth.oclc.org/auth
    flow: authorizationCode
    tokenUrl: https://oauth.oclc.org/token
  name: entity_data_auth
  source: openapi/worldcat-entities-api.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.oclc.org/token
  - authorizationUrl: https://oauth.oclc.org/auth
    flow: authorizationCode
    tokenUrl: https://oauth.oclc.org/token
  name: worldcat_metadata_auth
  source: openapi/worldcat-metadata-api.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.oclc.org/token
  - authorizationUrl: https://oauth.oclc.org/auth
    flow: authorizationCode
    tokenUrl: https://oauth.oclc.org/token
  name: worldcat_search_auth
  source: openapi/worldcat-search-api.yml
scope_count: 26
scope_names:
- WorldCatMetadataAPI
- WorldCatMetadataAPI:get_holding_codes
- WorldCatMetadataAPI:manage_bibs
- WorldCatMetadataAPI:manage_institution_holdings
- WorldCatMetadataAPI:manage_institution_lbds
- WorldCatMetadataAPI:manage_institution_lhrs
- WorldCatMetadataAPI:match_bibs
- WorldCatMetadataAPI:view_bib
- WorldCatMetadataAPI:view_brief_bib
- WorldCatMetadataAPI:view_marc_bib
- WorldCatMetadataAPI:view_my_holdings
- WorldCatMetadataAPI:view_my_holdings_private_notes
- WorldCatMetadataAPI:view_my_local_bib_data
- WorldCatMetadataAPI:view_retained_holdings
- WorldCatMetadataAPI:view_summary_holdings
- enhMetadataAPI:fieldTransfer
- publicEntities:read_brief_entities
- publicEntities:read_references
- wcapi:view_bib
- wcapi:view_brief_bib
- wcapi:view_holdings
- wcapi:view_institution_holdings
- wcapi:view_my_holdings
- wcapi:view_my_holdings_private_notes
- wcapi:view_retained_holdings
- wcapi:view_summary_holdings
scopes:
- description: ''
  flows: []
  scope: WorldCatMetadataAPI
- description: retrieve holding codes
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:get_holding_codes
- description: manage bibliographic data
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:manage_bibs
- description: manage institution holdings
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:manage_institution_holdings
- description: manage institution local bibliographic data records
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:manage_institution_lbds
- description: manage institution local holdings data records
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:manage_institution_lhrs
- description: match bibliographic records
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:match_bibs
- description: view full bibliographic data
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:view_bib
- description: view brief bibliographic data
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:view_brief_bib
- description: view marc bibliographic data
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:view_marc_bib
- description: view detailed information about the authentication institution's holdings
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:view_my_holdings
- description: view private notes in holdings data
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:view_my_holdings_private_notes
- description: view local bibliographic data from the authenticate institution
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:view_my_local_bib_data
- description: view holdings which libraries have chosen to retain
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:view_retained_holdings
- description: view summary information about library holdings
  flows:
  - authorizationCode
  - clientCredentials
  scope: WorldCatMetadataAPI:view_summary_holdings
- description: field transfer functionality
  flows:
  - authorizationCode
  - clientCredentials
  scope: enhMetadataAPI:fieldTransfer
- description: read brief entity data
  flows:
  - authorizationCode
  - clientCredentials
  scope: publicEntities:read_brief_entities
- description: read entity references
  flows:
  - authorizationCode
  - clientCredentials
  scope: publicEntities:read_references
- description: view bibliographic data
  flows:
  - authorizationCode
  - clientCredentials
  scope: wcapi:view_bib
- description: view brief bibliographic data
  flows:
  - authorizationCode
  - clientCredentials
  scope: wcapi:view_brief_bib
- description: view detailed information about library holdings
  flows:
  - authorizationCode
  - clientCredentials
  scope: wcapi:view_holdings
- description: view information about what library holds an item
  flows:
  - authorizationCode
  - clientCredentials
  scope: wcapi:view_institution_holdings
- description: view detailed information about the authentication institution's holdings
  flows:
  - authorizationCode
  - clientCredentials
  scope: wcapi:view_my_holdings
- description: view private notes in the authentication institution's holdings
  flows:
  - authorizationCode
  - clientCredentials
  scope: wcapi:view_my_holdings_private_notes
- description: view holdings which libraries have chosen to retain
  flows:
  - authorizationCode
  - clientCredentials
  scope: wcapi:view_retained_holdings
- description: view summary information about library holdings
  flows:
  - authorizationCode
  - clientCredentials
  scope: wcapi:view_summary_holdings
slug: worldcat-scopes
source_filename: worldcat-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/worldcat-entities-api.yml, openapi/worldcat-metadata-api.yml, openapi/worldcat-search-api.yml\nschemes:\n- name: entity_data_auth\n  source: openapi/worldcat-entities-api.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.oclc.org/token\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.oclc.org/auth\n    tokenUrl: https://oauth.oclc.org/token\n- name: worldcat_metadata_auth\n  source: openapi/worldcat-metadata-api.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.oclc.org/token\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.oclc.org/auth\n    tokenUrl: https://oauth.oclc.org/token\n- name: worldcat_search_auth\n  source: openapi/worldcat-search-api.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.oclc.org/token\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.oclc.org/auth\n    tokenUrl: https://oauth.oclc.org/token\n\
  scopes:\n- scope: WorldCatMetadataAPI\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:get_holding_codes\n  description: retrieve holding codes\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:manage_bibs\n  description: manage bibliographic data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:manage_institution_holdings\n  description: manage institution holdings\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:manage_institution_lbds\n  description: manage institution local bibliographic data records\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:manage_institution_lhrs\n  description: manage institution\
  \ local holdings data records\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:match_bibs\n  description: match bibliographic records\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:view_bib\n  description: view full bibliographic data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:view_brief_bib\n  description: view brief bibliographic data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:view_marc_bib\n  description: view marc bibliographic data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:view_my_holdings\n  description: view detailed information\
  \ about the authentication institution's holdings\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:view_my_holdings_private_notes\n  description: view private notes in holdings data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:view_my_local_bib_data\n  description: view local bibliographic data from the authenticate institution\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:view_retained_holdings\n  description: view holdings which libraries have chosen to retain\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: WorldCatMetadataAPI:view_summary_holdings\n  description: view summary information about library holdings\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: enhMetadataAPI:fieldTransfer\n  description: field transfer functionality\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-metadata-api.yml\n- scope: publicEntities:read_brief_entities\n  description: read brief entity data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-entities-api.yml\n- scope: publicEntities:read_references\n  description: read entity references\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-entities-api.yml\n- scope: wcapi:view_bib\n  description: view bibliographic data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-search-api.yml\n- scope: wcapi:view_brief_bib\n  description: view brief bibliographic data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-search-api.yml\n- scope: wcapi:view_holdings\n\
  \  description: view detailed information about library holdings\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-search-api.yml\n- scope: wcapi:view_institution_holdings\n  description: view information about what library holds an item\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-search-api.yml\n- scope: wcapi:view_my_holdings\n  description: view detailed information about the authentication institution's holdings\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-search-api.yml\n- scope: wcapi:view_my_holdings_private_notes\n  description: view private notes in the authentication institution's holdings\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-search-api.yml\n- scope: wcapi:view_retained_holdings\n  description: view holdings which libraries have chosen to retain\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/worldcat-search-api.yml\n- scope: wcapi:view_summary_holdings\n  description: view summary information about library holdings\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/worldcat-search-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldcat/refs/heads/main/scopes/worldcat-scopes.yml
summary_line: 26 scopes · clientCredentials/authorizationCode
tags:
- Libraries
- Bibliographic Records
- WorldCat
- OCLC
- Cataloging
- Metadata
- Discovery
- Books
- Media
- Linked Data
token_urls:
- https://oauth.oclc.org/token
---
