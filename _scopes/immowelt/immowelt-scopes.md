---
authorization_urls: []
description: ''
docs: https://227098cb35ba.eu.kongportals.com/apis/import-listings-v1/docs/m2m-authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Immowelt Scopes
name_suffix: OAuth Scopes
note: The Listings Management (import-listings) spec's info.description publishes an "Available scopes" table; the specs themselves declare only an http bearer securityScheme, not oauth2 scopes. The IWT Pro delegation guide names clim:listings:* (Listings Management API) and sklh:webhooks:* (Seeker Leads API) as the currently supported delegation scope values. No scope list is published for Export Listings or Seeker Leads Ingest.
overview: 'Immowelt publishes 15 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Immowelt API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Immowelt
provider_slug: immowelt
schemes: []
scope_count: 15
scope_names:
- clim:listings:*
- clim:medias:*
- clim:listings:create
- clim:listings:read
- clim:listings:update
- clim:listings:delete
- clim:medias:create
- clim:projects:*
- clim:projects:create
- clim:projects:read
- clim:projects:update
- clim:projects:delete
- clim:projects:assign
- clim:projects:unassign
- sklh:webhooks:*
scopes:
- description: View and manage your listing across this API
  flows: []
  scope: clim:listings:*
- description: Manage your media data across this API
  flows: []
  scope: clim:medias:*
- description: Manage your POST listing endpoint (/listings)
  flows: []
  scope: clim:listings:create
- description: Manage your GET listing endpoint (/listings, /listings/{externalListingId})
  flows: []
  scope: clim:listings:read
- description: Manage your PUT listing endpoint (/listings/{externalListingId})
  flows: []
  scope: clim:listings:update
- description: Manage your DELETE listing endpoint (/listings/{externalListingId})
  flows: []
  scope: clim:listings:delete
- description: Manage your POST media endpoint (/medias)
  flows: []
  scope: clim:medias:create
- description: View and manage your projects across this API
  flows: []
  scope: clim:projects:*
- description: Manage your POST project endpoint (/projects)
  flows: []
  scope: clim:projects:create
- description: Manage your GET project endpoint (/projects, /projects/{externalProjectId})
  flows: []
  scope: clim:projects:read
- description: Manage your PUT project endpoint (/projects/{externalProjectId})
  flows: []
  scope: clim:projects:update
- description: Manage your DELETE project endpoint (/projects/{externalProjectId})
  flows: []
  scope: clim:projects:delete
- description: listed in the spec's scope table for the project assign endpoint
  flows: []
  scope: clim:projects:assign
- description: listed in the spec's scope table for the project unassign endpoint
  flows: []
  scope: clim:projects:unassign
- description: Delegation scope for the Seeker Leads API named in the IWT Pro guide
  flows: []
  scope: sklh:webhooks:*
slug: immowelt-scopes
source_filename: immowelt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: 'generated: ''2026-10-28''

  method: searched

  source: openapi/_original/import-listings-v1.json

  docs: https://227098cb35ba.eu.kongportals.com/apis/import-listings-v1/docs/m2m-authentication

  note: The Listings Management (import-listings) spec''s info.description publishes an "Available scopes" table; the specs themselves declare only an http bearer securityScheme, not oauth2 scopes. The IWT Pro delegation guide names clim:listings:* (Listings Management API) and sklh:webhooks:* (Seeker Leads API) as the currently supported delegation scope values. No scope list is published for Export Listings or Seeker Leads Ingest.

  scopes:

  - {name: ''clim:listings:*'', api: Listings Management, description: View and manage your listing across this API}

  - {name: ''clim:medias:*'', api: Listings Management, description: Manage your media data across this API}

  - {name: ''clim:listings:create'', api: Listings Management, description: Manage your POST listing endpoint (/listings), operations: [createListing]}

  - {name: ''clim:listings:read'', api: Listings Management, description: ''Manage your GET listing endpoint (/listings, /listings/{externalListingId})'', operations: [getListings, getListing]}

  - {name: ''clim:listings:update'', api: Listings Management, description: ''Manage your PUT listing endpoint (/listings/{externalListingId})'', operations: [updateListing]}

  - {name: ''clim:listings:delete'', api: Listings Management, description: ''Manage your DELETE listing endpoint (/listings/{externalListingId})'', operations: [deleteListing]}

  - {name: ''clim:medias:create'', api: Listings Management, description: Manage your POST media endpoint (/medias), operations: [requestPresignedUrlMedia]}

  - {name: ''clim:projects:*'', api: Listings Management, description: View and manage your projects across this API}

  - {name: ''clim:projects:create'', api: Listings Management, description: Manage your POST project endpoint (/projects), operations: [createProject]}

  - {name: ''clim:projects:read'', api: Listings Management, description: ''Manage your GET project endpoint (/projects, /projects/{externalProjectId})'', operations: [getProjects, getProject]}

  - {name: ''clim:projects:update'', api: Listings Management, description: ''Manage your PUT project endpoint (/projects/{externalProjectId})'', operations: [updateProject]}

  - {name: ''clim:projects:delete'', api: Listings Management, description: ''Manage your DELETE project endpoint (/projects/{externalProjectId})'', operations: [deleteProject]}

  - {name: ''clim:projects:assign'', api: Listings Management, description: listed in the spec''s scope table for the project assign endpoint, operations: [assignListingsToProject]}

  - {name: ''clim:projects:unassign'', api: Listings Management, description: listed in the spec''s scope table for the project unassign endpoint, operations: [unassignListingsFromProject]}

  - {name: ''sklh:webhooks:*'', api: Seeker Leads, description: Delegation scope for the Seeker Leads API named in the IWT Pro guide, docs: https://www.developers.immowelt.de/guides/how-to-onboard-on-immowelt-apis/onboarding-process-iwt-pro}

  '
source_yaml_url: https://artifacts.apis.io/immowelt/scopes/immowelt-scopes.yml
summary_line: 15 scopes
tags:
- Real Estate
- Marketplace
- Germany
- Austria
- Property Listings
token_bound: false
token_urls: []
---
