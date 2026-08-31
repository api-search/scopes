---
api_specs:
- filename: musicbrainz-areas-api-openapi.yml
  format: yaml
  label: MusicBrainz Areas API
  slug: musicbrainz-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-areas-api-openapi.yml
- filename: musicbrainz-artists-api-openapi.yml
  format: yaml
  label: MusicBrainz Artists API
  slug: musicbrainz-artists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-artists-api-openapi.yml
- filename: musicbrainz-collections-api-openapi.yml
  format: yaml
  label: MusicBrainz Collections API
  slug: musicbrainz-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-collections-api-openapi.yml
- filename: musicbrainz-events-api-openapi.yml
  format: yaml
  label: MusicBrainz Events API
  slug: musicbrainz-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-events-api-openapi.yml
- filename: musicbrainz-genres-api-openapi.yml
  format: yaml
  label: MusicBrainz Genres API
  slug: musicbrainz-genres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-genres-api-openapi.yml
- filename: musicbrainz-identifiers-api-openapi.yml
  format: yaml
  label: MusicBrainz Identifiers API
  slug: musicbrainz-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-identifiers-api-openapi.yml
- filename: musicbrainz-instruments-api-openapi.yml
  format: yaml
  label: MusicBrainz Instruments API
  slug: musicbrainz-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-instruments-api-openapi.yml
- filename: musicbrainz-labels-api-openapi.yml
  format: yaml
  label: MusicBrainz Labels API
  slug: musicbrainz-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-labels-api-openapi.yml
- filename: musicbrainz-places-api-openapi.yml
  format: yaml
  label: MusicBrainz Places API
  slug: musicbrainz-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-places-api-openapi.yml
- filename: musicbrainz-recordings-api-openapi.yml
  format: yaml
  label: MusicBrainz Recordings API
  slug: musicbrainz-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-recordings-api-openapi.yml
- filename: musicbrainz-release-groups-api-openapi.yml
  format: yaml
  label: MusicBrainz Release Groups API
  slug: musicbrainz-release-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-release-groups-api-openapi.yml
- filename: musicbrainz-releases-api-openapi.yml
  format: yaml
  label: MusicBrainz Releases API
  slug: musicbrainz-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-releases-api-openapi.yml
- filename: musicbrainz-series-api-openapi.yml
  format: yaml
  label: MusicBrainz Series API
  slug: musicbrainz-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-series-api-openapi.yml
- filename: musicbrainz-submission-api-openapi.yml
  format: yaml
  label: MusicBrainz Submission API
  slug: musicbrainz-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-submission-api-openapi.yml
- filename: musicbrainz-urls-api-openapi.yml
  format: yaml
  label: MusicBrainz URLs API
  slug: musicbrainz-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-urls-api-openapi.yml
- filename: musicbrainz-works-api-openapi.yml
  format: yaml
  label: MusicBrainz Works API
  slug: musicbrainz-works-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/openapi/musicbrainz-works-api-openapi.yml
authorization_urls:
- https://musicbrainz.org/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Musicbrainz Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MusicBrainz publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MusicBrainz API on a user''s behalf.


  Tokens are issued from https://musicbrainz.org/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MusicBrainz
provider_slug: musicbrainz
schemes:
- description: OAuth 2.0 authentication via the MusicBrainz OAuth server.
  flows:
  - authorizationUrl: https://musicbrainz.org/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://musicbrainz.org/oauth2/token
  name: OAuth2
  source: openapi/musicbrainz-web-service-openapi.yml
scope_count: 7
scope_names:
- collection
- email
- profile
- rating
- submit_barcode
- submit_isrc
- tag
scopes:
- description: Manage collections
  flows:
  - authorizationCode
  scope: collection
- description: Access user email
  flows:
  - authorizationCode
  scope: email
- description: Access user profile
  flows:
  - authorizationCode
  scope: profile
- description: Submit ratings
  flows:
  - authorizationCode
  scope: rating
- description: Submit release barcodes
  flows:
  - authorizationCode
  scope: submit_barcode
- description: Submit recording ISRCs
  flows:
  - authorizationCode
  scope: submit_isrc
- description: Submit tags
  flows:
  - authorizationCode
  scope: tag
slug: musicbrainz-scopes
source_filename: musicbrainz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/musicbrainz-web-service-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/musicbrainz-web-service-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://musicbrainz.org/oauth2/authorize\n    tokenUrl: https://musicbrainz.org/oauth2/token\n  description: OAuth 2.0 authentication via the MusicBrainz OAuth server.\nscopes:\n- scope: collection\n  description: Manage collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/musicbrainz-web-service-openapi.yml\n- scope: email\n  description: Access user email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/musicbrainz-web-service-openapi.yml\n- scope: profile\n  description: Access user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/musicbrainz-web-service-openapi.yml\n- scope: rating\n  description: Submit ratings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/musicbrainz-web-service-openapi.yml\n\
  - scope: submit_barcode\n  description: Submit release barcodes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/musicbrainz-web-service-openapi.yml\n- scope: submit_isrc\n  description: Submit recording ISRCs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/musicbrainz-web-service-openapi.yml\n- scope: tag\n  description: Submit tags\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/musicbrainz-web-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/musicbrainz/refs/heads/main/scopes/musicbrainz-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Music
- Metadata
- Encyclopedia
- Open Data
- Catalog
- Identifiers
- ISRC
- ISWC
- MBID
- DiscID
- Artists
- Releases
- Recordings
- Works
- Labels
- Cover Art
- Open-Source
- Non Profit
token_urls:
- https://musicbrainz.org/oauth2/token
---
