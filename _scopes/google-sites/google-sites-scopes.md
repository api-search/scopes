---
authorization_urls: []
description: ''
docs: https://developers.google.com/workspace/sites/docs/1.0/developers_guide_protocol
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Google Sites Scopes
name_suffix: OAuth Scopes
note: 'Authored from the API''s own protocol guide, not derived - there is no OpenAPI or discovery document to read oauth2 securitySchemes from. The guide states a single scope for the whole API: "Here''s the OAuth 2.0 scope information for the Google Sites Data API: https://sites.google.com/feeds/". The Sites Data API predates the granular per-method scopes Google ships on its modern Workspace APIs; one coarse scope grants read AND write across all five feeds.'
overview: 'Google Sites uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Sites
provider_slug: google-sites
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: google-sites-scopes
source_filename: google-sites-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://developers.google.com/workspace/sites/docs/1.0/developers_guide_protocol\ndocs: https://developers.google.com/workspace/sites/docs/1.0/developers_guide_protocol\nnote: >-\n  Authored from the API's own protocol guide, not derived - there is no OpenAPI or\n  discovery document to read oauth2 securitySchemes from. The guide states a single\n  scope for the whole API: \"Here's the OAuth 2.0 scope information for the Google\n  Sites Data API: https://sites.google.com/feeds/\". The Sites Data API predates the\n  granular per-method scopes Google ships on its modern Workspace APIs; one coarse\n  scope grants read AND write across all five feeds.\ngranularity: coarse\nscope_count: 1\nscopes:\n  - name: https://sites.google.com/feeds/\n    description: >-\n      Full access to the Google Sites Data API. Grants read and write across the Site,\n      Content, Revision, Activity and ACL feeds for classic Google Sites the user\
  \ owns\n      or can view, including creating and copying sites on a Google Workspace domain,\n      uploading and downloading attachments, and modifying sharing permissions.\n    read: true\n    write: true\n    sensitive: true\n    feeds:\n      - site\n      - content\n      - revision\n      - activity\n      - acl\ngaps:\n  - >-\n    No read-only variant is published. An agent that only needs to list sites or read\n    content must still be granted a scope that can delete pages and change ACLs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-sites/refs/heads/main/scopes/google-sites-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Collaboration
- Content Management
- Google Workspace
- Websites
- Website Builder
- CMS
- Publishing
- Productivity
- Deprecated APIs
- GData
token_urls: []
---
