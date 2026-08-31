---
api_specs:
- filename: university-of-warwick-administration-api-openapi.yml
  format: yaml
  label: University of Warwick Administration API
  slug: university-of-warwick-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-administration-api-openapi.yml
- filename: university-of-warwick-jobs-api-openapi.yml
  format: yaml
  label: University of Warwick Jobs API
  slug: university-of-warwick-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-jobs-api-openapi.yml
- filename: university-of-warwick-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Warwick OAI PMH API
  slug: university-of-warwick-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-oai-pmh-api-openapi.yml
- filename: university-of-warwick-timetabling-api-openapi.yml
  format: yaml
  label: University of Warwick Timetabling API
  slug: university-of-warwick-timetabling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-timetabling-api-openapi.yml
authorization_urls:
- https://websignon.warwick.ac.uk/oauth/authorise
description: ''
docs: ''
flows:
- threeLegged
kind: oauth-scopes
layout: scope
method: searched
name: University Of Warwick Oauth Scopes
name_suffix: OAuth Scopes
note: These scope strings are read verbatim from Warwick's own published OAuth scopes table. Warwick states the list is non-exhaustive and that not all APIs for each service are available through OAuth. The scope values are Warwick's; the descriptions are ours. The `scope` parameter is Warwick-specific and is NOT defined in the OAuth 1.0a standard. It cannot be sent in the Authorization header — it must go in the query string or the POST body. Multiple scopes are joined with a `+` and passed as a single parameter. There is no machine-readable discovery document for these scopes. They exist only as an HTML table on the documentation page, which is why this artifact is `searched` rather than `probed`.
overview: 'University of Warwick publishes 9 OAuth 2.0 scopes via the threeLegged flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the University of Warwick API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Warwick
provider_slug: university-of-warwick
schemes:
- flows:
  - accessTokenUrl: https://websignon.warwick.ac.uk/oauth/accessToken
    authorizationUrl: https://websignon.warwick.ac.uk/oauth/authorise
    flow: threeLegged
    requestTokenUrl: https://websignon.warwick.ac.uk/oauth/requestToken
  name: warwick-websignon-oauth1
  signature_algorithms:
  - RSA-SHA1
  - HMAC-SHA1
  source: https://warwick.ac.uk/services/its/servicessupport/web/sign-on/help/oauth/apis/
  version: OAuth 1.0a
scope_count: 9
scope_names:
- urn:www2.warwick.ac.uk:sitebuilder2:read:service
- urn:sitebuilder.warwick.ac.uk:sitebuilder2:edit:service
- urn:search.warwick.ac.uk:search:service
- urn:files.warwick.ac.uk:files:service
- urn:blogs.warwick.ac.uk:blogbuilder:service
- urn:forums.warwick.ac.uk:forums:service
- urn:examtimetable.warwick.ac.uk:examtimetable:service
- urn:printercredits.warwick.ac.uk:printcredit:service
- urn:websignon.warwick.ac.uk:sso:service
scopes:
- description: Read access to Sitebuilder, Warwick's own institutional web content management system.
  flows:
  - threeLegged
  scope: urn:www2.warwick.ac.uk:sitebuilder2:read:service
- description: Edit access to Sitebuilder pages and content.
  flows:
  - threeLegged
  scope: urn:sitebuilder.warwick.ac.uk:sitebuilder2:edit:service
- description: Access to Warwick Search, the institution's own site and people search service.
  flows:
  - threeLegged
  scope: urn:search.warwick.ac.uk:search:service
- description: Access to the Files.Warwick file storage service on the user's behalf.
  flows:
  - threeLegged
  scope: urn:files.warwick.ac.uk:files:service
- description: Access to Warwick Blogs (BlogBuilder), the institution's own blogging platform.
  flows:
  - threeLegged
  scope: urn:blogs.warwick.ac.uk:blogbuilder:service
- description: Access to Warwick Forums on the user's behalf.
  flows:
  - threeLegged
  scope: urn:forums.warwick.ac.uk:forums:service
- description: Access to the user's exam timetable.
  flows:
  - threeLegged
  scope: urn:examtimetable.warwick.ac.uk:examtimetable:service
- description: Access to the user's campus printing credit balance.
  flows:
  - threeLegged
  scope: urn:printercredits.warwick.ac.uk:printcredit:service
- description: Access to the user's Web Sign-on identity attributes.
  flows:
  - threeLegged
  scope: urn:websignon.warwick.ac.uk:sso:service
slug: university-of-warwick-oauth-scopes
source_filename: university-of-warwick-oauth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: https://warwick.ac.uk/services/its/servicessupport/web/sign-on/help/oauth/apis/\nx-operator: institution\nnote: >-\n  These scope strings are read verbatim from Warwick's own published OAuth scopes table. Warwick\n  states the list is non-exhaustive and that not all APIs for each service are available through\n  OAuth. The scope values are Warwick's; the descriptions are ours.\n\n\n  The `scope` parameter is Warwick-specific and is NOT defined in the OAuth 1.0a standard. It\n  cannot be sent in the Authorization header — it must go in the query string or the POST body.\n  Multiple scopes are joined with a `+` and passed as a single parameter.\n\n\n  There is no machine-readable discovery document for these scopes. They exist only as an HTML\n  table on the documentation page, which is why this artifact is `searched` rather than `probed`.\nschemes:\n  - name: warwick-websignon-oauth1\n    source: https://warwick.ac.uk/services/its/servicessupport/web/sign-on/help/oauth/apis/\n\
  \    version: OAuth 1.0a\n    signature_algorithms: [RSA-SHA1, HMAC-SHA1]\n    flows:\n      - flow: threeLegged\n        requestTokenUrl: https://websignon.warwick.ac.uk/oauth/requestToken\n        authorizationUrl: https://websignon.warwick.ac.uk/oauth/authorise\n        accessTokenUrl: https://websignon.warwick.ac.uk/oauth/accessToken\nscopes:\n  - scope: urn:www2.warwick.ac.uk:sitebuilder2:read:service\n    service: Sitebuilder\n    description: Read access to Sitebuilder, Warwick's own institutional web content management system.\n    flows: [threeLegged]\n  - scope: urn:sitebuilder.warwick.ac.uk:sitebuilder2:edit:service\n    service: Sitebuilder\n    description: Edit access to Sitebuilder pages and content.\n    flows: [threeLegged]\n  - scope: urn:search.warwick.ac.uk:search:service\n    service: Warwick Search\n    description: Access to Warwick Search, the institution's own site and people search service.\n    flows: [threeLegged]\n  - scope: urn:files.warwick.ac.uk:files:service\n\
  \    service: Files.Warwick\n    description: Access to the Files.Warwick file storage service on the user's behalf.\n    flows: [threeLegged]\n  - scope: urn:blogs.warwick.ac.uk:blogbuilder:service\n    service: Warwick Blogs\n    description: Access to Warwick Blogs (BlogBuilder), the institution's own blogging platform.\n    flows: [threeLegged]\n  - scope: urn:forums.warwick.ac.uk:forums:service\n    service: Warwick Forums\n    description: Access to Warwick Forums on the user's behalf.\n    flows: [threeLegged]\n  - scope: urn:examtimetable.warwick.ac.uk:examtimetable:service\n    service: Exam Timetabling\n    description: Access to the user's exam timetable.\n    flows: [threeLegged]\n  - scope: urn:printercredits.warwick.ac.uk:printcredit:service\n    service: Printer Credits\n    description: Access to the user's campus printing credit balance.\n    flows: [threeLegged]\n  - scope: urn:websignon.warwick.ac.uk:sso:service\n    service: Web Sign-on\n    description: Access to the\
  \ user's Web Sign-on identity attributes.\n    flows: [threeLegged]\ncoverage:\n  scopes_total: 9\n  documented_by_provider: true\n  machine_readable: false\n  exhaustive: false\n  note: >-\n    Warwick explicitly labels its own table non-exhaustive. Further detail on retrieving user\n    information from Web Sign-on sits behind an access-restricted page open only to University\n    members and registered Web Sign-on developers, so the public scope inventory stops here.\nx-evidence:\n  - url: https://warwick.ac.uk/services/its/servicessupport/web/sign-on/help/oauth/apis/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/scopes/university-of-warwick-oauth-scopes.yml
summary_line: 9 scopes · threeLegged
tags:
- University
- Higher Education
- Education
- Research
- United Kingdom
- Russell Group
- Identity Federation
- Research Repository
- Course Catalog
- Timetabling
- Student Information System
- Open Data
token_urls: []
---
