---
authorization_urls: []
description: ''
docs: https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Emarsys Scopes
name_suffix: OAuth Scopes
note: Emarsys v3 API uses OAuth 2.0 client credentials (OpenID Connect/JWT) without a scope parameter; access is governed by named endpoint permissions enabled per API user in Security Settings, documented at https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings.
overview: 'SAP Emarsys publishes 156 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAP Emarsys API on a user''s behalf.


  Tokens are issued from https://api.emarsys.net/api/v3/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP Emarsys
provider_slug: emarsys
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.emarsys.net/api/v3/auth/token
  name: OAuth2
  source: openapi/emarsys-openapi.yml
scope_count: 156
scope_names:
- administrator.list
- administrator.update
- administrator.delete
- administrator.get
- administrator.accesslevel.list
- administrator.session.create
- administrator.interfacelanguage.list
- administrator.startpage.list
- administrator.fetch
- administrator.create
- autoimport.list
- autoimport.get
- autoimport.delete
- autoimport.create
- blacklist.get
- blocklist.get
- campaign.create
- campaign.list
- campaign.get
- campaign.source.update
- campaign.update
- campaign.delete
- campaign.version.create
- campaign.finalize
- campaign.copy
- campaign.preview
- campaign.sendtestmail
- campaign.launch
- campaign.broadcast
- campaign.stop
- campaign.getdeliverystatus
- campaign.responses
- campaign.responses.get
- campaign.responsesummary
- campaign.getlaunchesofemail
- campaign.personalization
- campaign.url
- campaign.unsubscribe
- campaign.trackedlink.create
- campaign.trackedlink.get
- campaign.linkcategory.list
- campaign.trackedlink.update
- campaign.trackedlink.delete
- campaign.section.create
- campaign.section.list
- campaign.section.get
- campaign.section.update
- campaign.section.delete
- campaign.language.list
- campaign.category.list
- campaign.condition.list
- campaign.template.list
- campaign.template.get
- campaign.delete.alias
- campaign.program.list
- campaign.response.get
- campaign.responsesummary.filter
- campaign.version.list
- campaign.trackedlink.list
- campaigns.get
- combinedsegment.list
- combinedsegment.get
- combinedsegment.create
- combinedsegment.update
- combinedsegment.universal.list
- combinedsegment.universal.get
- combinedsegment.universal.create
- combinedsegment.universal.update
- combinedsegment.test.get
- combinedsegment.test.create
- combinedsegment.test.update
- contact.batchUpdate
- contact.changes.get
- contact.changes.list
- contact.contactid.verify
- contact.create
- contact.delete
- contact.get
- contact.getdata
- contact.history.filter
- contact.history.list
- contact.list
- contact.lookup
- contact.merge
- contact.singleUpdate
- contact.update
- contactlist.contact.add
- contactlist.contact.count
- contactlist.contact.delete
- contactlist.contact.ids
- contactlist.create
- contactlist.delete
- contactlist.list
- contactlist.rename
- contactlist.replace
- customer.settings
- customer.settings.corporatedomain
- customer.settings.deliverability
- customer.settings.iprestrictions
- customer.settings.languages
- export.contact.changed
- export.contact.registrations
- export.contactlist
- export.download
- export.responses
- export.segment
- export.status
- externalevent.create
- externalevent.delete
- externalevent.get
- externalevent.list
- externalevent.trigger
- externalevent.update
- externalevent.usages
- field.create
- field.delete
- field.get
- field.list
- field.multichoice.list
- field.singlechoice.get
- field.singlechoice.lang.list
- field.singlechoice.trans.list
- form.list
- form.trigger
- keyring.key.delete
- keyring.key.list
- mediadb.file.create
- mediadb.file.delete
- mediadb.file.get
- mediadb.file.list
- mediadb.folder.create
- mediadb.folder.list
- program.abort
- program.delete
- program.get
- program.start
- programresource.list
- segment.contact.count
- segment.contact.list
- segment.contact.lookup
- segment.contact.run
- segment.contact.run.status
- segment.contacts.run
- segment.contacts.run.status
- segment.contacts.run.status.deprecated
- segment.create
- segment.criteria.get
- segment.criteria.update
- segment.delete
- segment.get
- segment.list
- source.create
- source.delete
- source.get
- trendreporting.launches.get
- wishlist.update
scopes:
- description: Endpoint permission (administrator) enabling GET /v2/administrator.
  flows: []
  scope: administrator.list
- description: Endpoint permission (administrator) enabling POST /v2/administrator/{administratorId}/patch.
  flows: []
  scope: administrator.update
- description: Endpoint permission (administrator) enabling POST /v2/administrator/{administratorId}/delete.
  flows: []
  scope: administrator.delete
- description: Endpoint permission (administrator) enabling GET /v2/administrator/query/{administratorId}.
  flows: []
  scope: administrator.get
- description: Endpoint permission (administrator) enabling GET /v2/administrator/getaccesslevels.
  flows: []
  scope: administrator.accesslevel.list
- description: Endpoint permission (administrator) enabling POST /v2/administrator/{administratorId}/session.
  flows: []
  scope: administrator.session.create
- description: Endpoint permission (administrator) enabling GET /v2/administrator/getinterfacelanguages.
  flows: []
  scope: administrator.interfacelanguage.list
- description: Endpoint permission (administrator) enabling GET /v2/administrator/getstartpages.
  flows: []
  scope: administrator.startpage.list
- description: Endpoint permission (administrator) enabling GET /v2/administrator/{administratorId}.
  flows: []
  scope: administrator.fetch
- description: Endpoint permission (administrator) enabling POST /v2/administrator.
  flows: []
  scope: administrator.create
- description: Endpoint permission (autoimport) enabling GET /v2/settings/autoimports.
  flows: []
  scope: autoimport.list
- description: Endpoint permission (autoimport) enabling GET /v2/settings/autoimports/{profileId}.
  flows: []
  scope: autoimport.get
- description: Endpoint permission (autoimport) enabling POST /v2/settings/autoimports/{profileId}/delete.
  flows: []
  scope: autoimport.delete
- description: Endpoint permission (autoimport) enabling POST /v2/settings/autoimports.
  flows: []
  scope: autoimport.create
- description: Endpoint permission (blocklist) enabling POST /v2/blacklist.
  flows: []
  scope: blacklist.get
- description: Endpoint permission (blocklist) enabling POST /v2/blocklist.
  flows: []
  scope: blocklist.get
- description: Endpoint permission (campaign) enabling POST /v2/email.
  flows: []
  scope: campaign.create
- description: Endpoint permission (campaign) enabling GET /v2/email.
  flows: []
  scope: campaign.list
- description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}.
  flows: []
  scope: campaign.get
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/updatesource.
  flows: []
  scope: campaign.source.update
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/patch.
  flows: []
  scope: campaign.update
- description: Endpoint permission (campaign) enabling POST /v2/email/delete.
  flows: []
  scope: campaign.delete
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/version.
  flows: []
  scope: campaign.version.create
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/finalize.
  flows: []
  scope: campaign.finalize
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/copy.
  flows: []
  scope: campaign.copy
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/preview.
  flows: []
  scope: campaign.preview
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/sendtestmail.
  flows: []
  scope: campaign.sendtestmail
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/launch.
  flows: []
  scope: campaign.launch
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/broadcast.
  flows: []
  scope: campaign.broadcast
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/stop.
  flows: []
  scope: campaign.stop
- description: Endpoint permission (campaign) enabling POST /v2/email/getdeliverystatus.
  flows: []
  scope: campaign.getdeliverystatus
- description: Endpoint permission (campaign) enabling POST /v2/email/responses.
  flows: []
  scope: campaign.responses
- description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/responses.
  flows: []
  scope: campaign.responses.get
- description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/responsesummary.
  flows: []
  scope: campaign.responsesummary
- description: Endpoint permission (campaign) enabling POST /v2/email/getlaunchesofemail.
  flows: []
  scope: campaign.getlaunchesofemail
- description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/personalization.
  flows: []
  scope: campaign.personalization
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/url.
  flows: []
  scope: campaign.url
- description: Endpoint permission (campaign) enabling POST /v2/email/unsubscribe.
  flows: []
  scope: campaign.unsubscribe
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/trackedlinks.
  flows: []
  scope: campaign.trackedlink.create
- description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/trackedlinks/{linkId}.
  flows: []
  scope: campaign.trackedlink.get
- description: Endpoint permission (campaign) enabling GET /v2/settings/linkcategories.
  flows: []
  scope: campaign.linkcategory.list
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/trackedlinks/{linkId}.
  flows: []
  scope: campaign.trackedlink.update
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/deletetrackedlinks/{linkId}.
  flows: []
  scope: campaign.trackedlink.delete
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/sections.
  flows: []
  scope: campaign.section.create
- description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/sections.
  flows: []
  scope: campaign.section.list
- description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/sections/{sectionId}.
  flows: []
  scope: campaign.section.get
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/sections/{sectionId}.
  flows: []
  scope: campaign.section.update
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/sections/{sectionId}/delete.
  flows: []
  scope: campaign.section.delete
- description: Endpoint permission (campaign) enabling GET /v2/language.
  flows: []
  scope: campaign.language.list
- description: Endpoint permission (campaign) enabling GET /v2/emailcategory.
  flows: []
  scope: campaign.category.list
- description: Endpoint permission (campaign) enabling GET /v2/condition.
  flows: []
  scope: campaign.condition.list
- description: Endpoint permission (campaign) enabling GET /v2/email/templates.
  flows: []
  scope: campaign.template.list
- description: Endpoint permission (campaign) enabling GET /v2/email/templates/{templateId}.
  flows: []
  scope: campaign.template.get
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/delete.
  flows: []
  scope: campaign.delete.alias
- description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/programs.
  flows: []
  scope: campaign.program.list
- description: Endpoint permission (campaign) enabling GET /v2/email/responses/{responseId}.
  flows: []
  scope: campaign.response.get
- description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/responsesummary.
  flows: []
  scope: campaign.responsesummary.filter
- description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/versions.
  flows: []
  scope: campaign.version.list
- description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/trackedlinks.
  flows: []
  scope: campaign.trackedlink.list
- description: Endpoint permission (campaign) enabling GET /v2/campaigns.
  flows: []
  scope: campaigns.get
- description: Endpoint permission (combinedsegment) enabling GET /v2/combinedsegments.
  flows: []
  scope: combinedsegment.list
- description: Endpoint permission (combinedsegment) enabling GET /v2/combinedsegments/{combinedSegmentId}.
  flows: []
  scope: combinedsegment.get
- description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments.
  flows: []
  scope: combinedsegment.create
- description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments/{combinedSegmentId}.
  flows: []
  scope: combinedsegment.update
- description: Endpoint permission (combinedsegment) enabling GET /v2/combinedsegments/universal.
  flows: []
  scope: combinedsegment.universal.list
- description: Endpoint permission (combinedsegment) enabling GET /v2/combinedsegments/universal/{combinedSegmentId}.
  flows: []
  scope: combinedsegment.universal.get
- description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments/universal.
  flows: []
  scope: combinedsegment.universal.create
- description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments/universal/{combinedSegmentId}.
  flows: []
  scope: combinedsegment.universal.update
- description: Endpoint permission (combinedsegment) enabling GET /v2/combinedsegments/test/{combinedSegmentId}.
  flows: []
  scope: combinedsegment.test.get
- description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments/test.
  flows: []
  scope: combinedsegment.test.create
- description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments/test/{combinedSegmentId}.
  flows: []
  scope: combinedsegment.test.update
- description: Endpoint permission (contact / contactlist) enabling PUT /v2/contact/update.
  flows: []
  scope: contact.batchUpdate
- description: Endpoint permission (contact / contactlist) enabling GET /v2/contact/last_change.
  flows: []
  scope: contact.changes.get
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/last_change.
  flows: []
  scope: contact.changes.list
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/checkids.
  flows: []
  scope: contact.contactid.verify
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contact.
  flows: []
  scope: contact.create
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/delete.
  flows: []
  scope: contact.delete
- description: Endpoint permission (contact / contactlist) enabling GET /v2/contact.
  flows: []
  scope: contact.get
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/getdata.
  flows: []
  scope: contact.getdata
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/getcontacthistory.
  flows: []
  scope: contact.history.filter
- description: Endpoint permission (contact / contactlist) enabling GET /v2/contact/getcontacthistory.
  flows: []
  scope: contact.history.list
- description: Endpoint permission (contact / contactlist) enabling GET /v2/contact/query.
  flows: []
  scope: contact.list
- description: Endpoint permission (contact / contactlist) enabling GET /v2/contact/getdata.
  flows: []
  scope: contact.lookup
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/merge.
  flows: []
  scope: contact.merge
- description: Endpoint permission (contact / contactlist) enabling PUT /v2/contact/{contactId}.
  flows: []
  scope: contact.singleUpdate
- description: Endpoint permission (contact / contactlist) enabling PUT /v2/contact.
  flows: []
  scope: contact.update
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contactlist/{listId}/add.
  flows: []
  scope: contactlist.contact.add
- description: Endpoint permission (contact / contactlist) enabling GET /v2/contactlist/{listId}/count.
  flows: []
  scope: contactlist.contact.count
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contactlist/{listId}/delete.
  flows: []
  scope: contactlist.contact.delete
- description: Endpoint permission (contact / contactlist) enabling GET /v2/contactlist/{contactlistId}/contactIds.
  flows: []
  scope: contactlist.contact.ids
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contactlist.
  flows: []
  scope: contactlist.create
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contactlist/{listId}/deletelist.
  flows: []
  scope: contactlist.delete
- description: Endpoint permission (contact / contactlist) enabling GET /v2/contactlist.
  flows: []
  scope: contactlist.list
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contactlist/{listId}/rename.
  flows: []
  scope: contactlist.rename
- description: Endpoint permission (contact / contactlist) enabling POST /v2/contactlist/{listId}/replace.
  flows: []
  scope: contactlist.replace
- description: Endpoint permission (customer) enabling GET /v2/settings.
  flows: []
  scope: customer.settings
- description: Endpoint permission (customer) enabling GET /v2/settings/corporatedomain.
  flows: []
  scope: customer.settings.corporatedomain
- description: Endpoint permission (customer) enabling GET /v2/settings/deliverability.
  flows: []
  scope: customer.settings.deliverability
- description: Endpoint permission (customer) enabling GET /v2/settings/iprestrictions.
  flows: []
  scope: customer.settings.iprestrictions
- description: Endpoint permission (customer) enabling GET /v2/settings/languages/translation/en.
  flows: []
  scope: customer.settings.languages
- description: Endpoint permission (export) enabling POST /v2/contact/getchanges.
  flows: []
  scope: export.contact.changed
- description: Endpoint permission (export) enabling POST /v2/contact/getregistrations.
  flows: []
  scope: export.contact.registrations
- description: Endpoint permission (export) enabling POST /v2/email/getcontacts.
  flows: []
  scope: export.contactlist
- description: Endpoint permission (export) enabling GET /v2/export/{exportId}/data.
  flows: []
  scope: export.download
- description: Endpoint permission (export) enabling POST /v2/email/getresponses.
  flows: []
  scope: export.responses
- description: Endpoint permission (export) enabling POST /v2/export/filter.
  flows: []
  scope: export.segment
- description: Endpoint permission (export) enabling GET /v2/export/{exportId}.
  flows: []
  scope: export.status
- description: Endpoint permission (externalevent) enabling POST /v2/event.
  flows: []
  scope: externalevent.create
- description: Endpoint permission (externalevent) enabling POST /v2/event/{eventId}/delete.
  flows: []
  scope: externalevent.delete
- description: Endpoint permission (externalevent) enabling GET /v2/event/{eventId}.
  flows: []
  scope: externalevent.get
- description: Endpoint permission (externalevent) enabling GET /v2/event.
  flows: []
  scope: externalevent.list
- description: Endpoint permission (externalevent) enabling POST /v2/event/{eventId}/trigger.
  flows: []
  scope: externalevent.trigger
- description: Endpoint permission (externalevent) enabling POST /v2/event/{eventId}.
  flows: []
  scope: externalevent.update
- description: Endpoint permission (externalevent) enabling GET /v2/event/{eventId}/usages.
  flows: []
  scope: externalevent.usages
- description: Endpoint permission (field) enabling POST /v2/field.
  flows: []
  scope: field.create
- description: Endpoint permission (field) enabling DELETE /v2/field/{fieldId}.
  flows: []
  scope: field.delete
- description: Endpoint permission (field) enabling GET /v2/field.
  flows: []
  scope: field.get
- description: Endpoint permission (field) enabling GET /v2/field/translate/{languageId}.
  flows: []
  scope: field.list
- description: Endpoint permission (field) enabling GET /v2/field/choices.
  flows: []
  scope: field.multichoice.list
- description: Endpoint permission (field) enabling GET /v2/field/{fieldId}/choice.
  flows: []
  scope: field.singlechoice.get
- description: Endpoint permission (field) enabling GET /v2/field/{fieldId}/choice/lang/{languageId}.
  flows: []
  scope: field.singlechoice.lang.list
- description: Endpoint permission (field) enabling GET /v2/field/{fieldId}/choice/translate/{languageId}.
  flows: []
  scope: field.singlechoice.trans.list
- description: Endpoint permission (form) enabling GET /v2/form.
  flows: []
  scope: form.list
- description: Endpoint permission (form) enabling POST /v2/form/{formId}/trigger.
  flows: []
  scope: form.trigger
- description: Endpoint permission (keyring) enabling POST /v2/keyring/keys/{keyId}/delete.
  flows: []
  scope: keyring.key.delete
- description: Endpoint permission (keyring) enabling POST /v2/keyring/keys.
  flows: []
  scope: keyring.key.list
- description: Endpoint permission (mediadb) enabling POST /v2/file.
  flows: []
  scope: mediadb.file.create
- description: Endpoint permission (mediadb) enabling POST /v2/file/{fileId}/delete.
  flows: []
  scope: mediadb.file.delete
- description: Endpoint permission (mediadb) enabling GET /v2/file/{fileId}.
  flows: []
  scope: mediadb.file.get
- description: Endpoint permission (mediadb) enabling GET /v2/file.
  flows: []
  scope: mediadb.file.list
- description: Endpoint permission (mediadb) enabling POST /v2/folder.
  flows: []
  scope: mediadb.folder.create
- description: Endpoint permission (mediadb) enabling GET /v2/folder.
  flows: []
  scope: mediadb.folder.list
- description: Endpoint permission (program / programresource) enabling POST /v2/ac/programs/{programId}/abort.
  flows: []
  scope: program.abort
- description: Endpoint permission (program / programresource) enabling POST /v2/ac/programs/{programId}/delete.
  flows: []
  scope: program.delete
- description: Endpoint permission (program / programresource) enabling GET /v2/ac/programs.
  flows: []
  scope: program.get
- description: Endpoint permission (program / programresource) enabling POST /v2/ac/programs/entrypoints/{nodeType}/resources/{resourceId}/runs.
  flows: []
  scope: program.start
- description: Endpoint permission (program / programresource) enabling GET /v2/programresource.
  flows: []
  scope: programresource.list
- description: Endpoint permission (segment) enabling GET /v2/filter/{segmentId}/contacts/count.
  flows: []
  scope: segment.contact.count
- description: Endpoint permission (segment) enabling GET /v2/filter/{segmentId}/contacts.
  flows: []
  scope: segment.contact.list
- description: Endpoint permission (segment) enabling GET /v2/filter/{segmentId}/contacts/{contactId}.
  flows: []
  scope: segment.contact.lookup
- description: Endpoint permission (segment) enabling POST /v2/filter/{segmentId}/single_runs.
  flows: []
  scope: segment.contact.run
- description: Endpoint permission (segment) enabling GET /v2/filter/single_runs/{runId}.
  flows: []
  scope: segment.contact.run.status
- description: Endpoint permission (segment) enabling POST /v2/filter/{segmentId}/runs.
  flows: []
  scope: segment.contacts.run
- description: Endpoint permission (segment) enabling GET /v2/filter/runs/{runId}.
  flows: []
  scope: segment.contacts.run.status
- description: Endpoint permission (segment) enabling GET /v2/filter/{segmentId}/runs/{runId}.
  flows: []
  scope: segment.contacts.run.status.deprecated
- description: Endpoint permission (segment) enabling PUT /v2/filter.
  flows: []
  scope: segment.create
- description: Endpoint permission (segment) enabling GET /v2/filter/{segmentId}/contact_criteria.
  flows: []
  scope: segment.criteria.get
- description: Endpoint permission (segment) enabling PUT /v2/filter/{segmentId}/contact_criteria.
  flows: []
  scope: segment.criteria.update
- description: Endpoint permission (segment) enabling GET /v2/filter/{segmentId}/delete.
  flows: []
  scope: segment.delete
- description: Endpoint permission (segment) enabling GET /v2/filter.
  flows: []
  scope: segment.get
- description: Endpoint permission (segment) enabling GET /v2/filter/{segmentId}.
  flows: []
  scope: segment.list
- description: Endpoint permission (source) enabling POST /v2/source/create.
  flows: []
  scope: source.create
- description: Endpoint permission (source) enabling DELETE /v2/source/{sourceId}.
  flows: []
  scope: source.delete
- description: Endpoint permission (source) enabling GET /v2/source.
  flows: []
  scope: source.get
- description: Endpoint permission (trendreporting) enabling GET /v2/trendreporting/launches.
  flows: []
  scope: trendreporting.launches.get
- description: Endpoint permission (wishlist) enabling POST /v2/wishlist/update.
  flows: []
  scope: wishlist.update
slug: emarsys-scopes
source_filename: emarsys-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/emarsys-openapi.yml\ndocs: https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\nnote: Emarsys v3 API uses OAuth 2.0 client credentials (OpenID Connect/JWT) without a scope parameter; access is governed by named endpoint permissions enabled per API user in Security Settings, documented at https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings.\nschemes:\n- name: OAuth2\n  source: openapi/emarsys-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.emarsys.net/api/v3/auth/token\nscopes:\n- scope: administrator.list\n  description: Endpoint permission (administrator) enabling GET /v2/administrator.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: administrator.update\n  description: Endpoint permission (administrator) enabling POST /v2/administrator/{administratorId}/patch.\n\
  \  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: administrator.delete\n  description: Endpoint permission (administrator) enabling POST /v2/administrator/{administratorId}/delete.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: administrator.get\n  description: Endpoint permission (administrator) enabling GET /v2/administrator/query/{administratorId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: administrator.accesslevel.list\n  description: Endpoint permission (administrator) enabling GET /v2/administrator/getaccesslevels.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: administrator.session.create\n  description: Endpoint permission (administrator) enabling POST /v2/administrator/{administratorId}/session.\n\
  \  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: administrator.interfacelanguage.list\n  description: Endpoint permission (administrator) enabling GET /v2/administrator/getinterfacelanguages.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: administrator.startpage.list\n  description: Endpoint permission (administrator) enabling GET /v2/administrator/getstartpages.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: administrator.fetch\n  description: Endpoint permission (administrator) enabling GET /v2/administrator/{administratorId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: administrator.create\n  description: Endpoint permission (administrator) enabling POST /v2/administrator.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n\
  - scope: autoimport.list\n  description: Endpoint permission (autoimport) enabling GET /v2/settings/autoimports.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: autoimport.get\n  description: Endpoint permission (autoimport) enabling GET /v2/settings/autoimports/{profileId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: autoimport.delete\n  description: Endpoint permission (autoimport) enabling POST /v2/settings/autoimports/{profileId}/delete.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: autoimport.create\n  description: Endpoint permission (autoimport) enabling POST /v2/settings/autoimports.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: blacklist.get\n  description: Endpoint permission (blocklist) enabling\
  \ POST /v2/blacklist.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: blocklist.get\n  description: Endpoint permission (blocklist) enabling POST /v2/blocklist.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.create\n  description: Endpoint permission (campaign) enabling POST /v2/email.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.list\n  description: Endpoint permission (campaign) enabling GET /v2/email.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.get\n  description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.source.update\n  description:\
  \ Endpoint permission (campaign) enabling POST /v2/email/{emailId}/updatesource.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.update\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/patch.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.delete\n  description: Endpoint permission (campaign) enabling POST /v2/email/delete.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.version.create\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/version.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.finalize\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/finalize.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n\
  - scope: campaign.copy\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/copy.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.preview\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/preview.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.sendtestmail\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/sendtestmail.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.launch\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/launch.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.broadcast\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/broadcast.\n\
  \  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.stop\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/stop.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.getdeliverystatus\n  description: Endpoint permission (campaign) enabling POST /v2/email/getdeliverystatus.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.responses\n  description: Endpoint permission (campaign) enabling POST /v2/email/responses.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.responses.get\n  description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/responses.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n\
  - scope: campaign.responsesummary\n  description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/responsesummary.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.getlaunchesofemail\n  description: Endpoint permission (campaign) enabling POST /v2/email/getlaunchesofemail.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.personalization\n  description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/personalization.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.url\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/url.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.unsubscribe\n  description: Endpoint permission\
  \ (campaign) enabling POST /v2/email/unsubscribe.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.trackedlink.create\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/trackedlinks.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.trackedlink.get\n  description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/trackedlinks/{linkId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.linkcategory.list\n  description: Endpoint permission (campaign) enabling GET /v2/settings/linkcategories.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.trackedlink.update\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/trackedlinks/{linkId}.\n\
  \  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.trackedlink.delete\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/deletetrackedlinks/{linkId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.section.create\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/sections.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.section.list\n  description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/sections.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.section.get\n  description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/sections/{sectionId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n\
  - scope: campaign.section.update\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/sections/{sectionId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.section.delete\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/sections/{sectionId}/delete.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.language.list\n  description: Endpoint permission (campaign) enabling GET /v2/language.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.category.list\n  description: Endpoint permission (campaign) enabling GET /v2/emailcategory.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.condition.list\n  description: Endpoint permission\
  \ (campaign) enabling GET /v2/condition.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.template.list\n  description: Endpoint permission (campaign) enabling GET /v2/email/templates.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.template.get\n  description: Endpoint permission (campaign) enabling GET /v2/email/templates/{templateId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.delete.alias\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/delete.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.program.list\n  description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/programs.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n\
  - scope: campaign.response.get\n  description: Endpoint permission (campaign) enabling GET /v2/email/responses/{responseId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.responsesummary.filter\n  description: Endpoint permission (campaign) enabling POST /v2/email/{emailId}/responsesummary.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.version.list\n  description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/versions.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaign.trackedlink.list\n  description: Endpoint permission (campaign) enabling GET /v2/email/{emailId}/trackedlinks.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: campaigns.get\n  description: Endpoint permission\
  \ (campaign) enabling GET /v2/campaigns.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: combinedsegment.list\n  description: Endpoint permission (combinedsegment) enabling GET /v2/combinedsegments.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: combinedsegment.get\n  description: Endpoint permission (combinedsegment) enabling GET /v2/combinedsegments/{combinedSegmentId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: combinedsegment.create\n  description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: combinedsegment.update\n  description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments/{combinedSegmentId}.\n\
  \  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: combinedsegment.universal.list\n  description: Endpoint permission (combinedsegment) enabling GET /v2/combinedsegments/universal.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: combinedsegment.universal.get\n  description: Endpoint permission (combinedsegment) enabling GET /v2/combinedsegments/universal/{combinedSegmentId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: combinedsegment.universal.create\n  description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments/universal.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: combinedsegment.universal.update\n  description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments/universal/{combinedSegmentId}.\n\
  \  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: combinedsegment.test.get\n  description: Endpoint permission (combinedsegment) enabling GET /v2/combinedsegments/test/{combinedSegmentId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: combinedsegment.test.create\n  description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments/test.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: combinedsegment.test.update\n  description: Endpoint permission (combinedsegment) enabling POST /v2/combinedsegments/test/{combinedSegmentId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.batchUpdate\n  description: Endpoint permission (contact / contactlist) enabling PUT /v2/contact/update.\n  sources:\n\
  \  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.changes.get\n  description: Endpoint permission (contact / contactlist) enabling GET /v2/contact/last_change.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.changes.list\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/last_change.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.contactid.verify\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/checkids.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.create\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contact.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n\
  - scope: contact.delete\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/delete.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.get\n  description: Endpoint permission (contact / contactlist) enabling GET /v2/contact.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.getdata\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/getdata.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.history.filter\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/getcontacthistory.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.history.list\n  description: Endpoint permission (contact / contactlist)\
  \ enabling GET /v2/contact/getcontacthistory.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.list\n  description: Endpoint permission (contact / contactlist) enabling GET /v2/contact/query.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.lookup\n  description: Endpoint permission (contact / contactlist) enabling GET /v2/contact/getdata.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.merge\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contact/merge.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contact.singleUpdate\n  description: Endpoint permission (contact / contactlist) enabling PUT /v2/contact/{contactId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n\
  - scope: contact.update\n  description: Endpoint permission (contact / contactlist) enabling PUT /v2/contact.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contactlist.contact.add\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contactlist/{listId}/add.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contactlist.contact.count\n  description: Endpoint permission (contact / contactlist) enabling GET /v2/contactlist/{listId}/count.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contactlist.contact.delete\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contactlist/{listId}/delete.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contactlist.contact.ids\n\
  \  description: Endpoint permission (contact / contactlist) enabling GET /v2/contactlist/{contactlistId}/contactIds.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contactlist.create\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contactlist.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contactlist.delete\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contactlist/{listId}/deletelist.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contactlist.list\n  description: Endpoint permission (contact / contactlist) enabling GET /v2/contactlist.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contactlist.rename\n  description: Endpoint permission (contact\
  \ / contactlist) enabling POST /v2/contactlist/{listId}/rename.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: contactlist.replace\n  description: Endpoint permission (contact / contactlist) enabling POST /v2/contactlist/{listId}/replace.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: customer.settings\n  description: Endpoint permission (customer) enabling GET /v2/settings.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: customer.settings.corporatedomain\n  description: Endpoint permission (customer) enabling GET /v2/settings/corporatedomain.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: customer.settings.deliverability\n  description: Endpoint permission (customer) enabling GET /v2/settings/deliverability.\n\
  \  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: customer.settings.iprestrictions\n  description: Endpoint permission (customer) enabling GET /v2/settings/iprestrictions.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: customer.settings.languages\n  description: Endpoint permission (customer) enabling GET /v2/settings/languages/translation/en.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: export.contact.changed\n  description: Endpoint permission (export) enabling POST /v2/contact/getchanges.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: export.contact.registrations\n  description: Endpoint permission (export) enabling POST /v2/contact/getregistrations.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n\
  - scope: export.contactlist\n  description: Endpoint permission (export) enabling POST /v2/email/getcontacts.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: export.download\n  description: Endpoint permission (export) enabling GET /v2/export/{exportId}/data.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: export.responses\n  description: Endpoint permission (export) enabling POST /v2/email/getresponses.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: export.segment\n  description: Endpoint permission (export) enabling POST /v2/export/filter.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: export.status\n  description: Endpoint permission (export) enabling GET /v2/export/{exportId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n\
  - scope: externalevent.create\n  description: Endpoint permission (externalevent) enabling POST /v2/event.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: externalevent.delete\n  description: Endpoint permission (externalevent) enabling POST /v2/event/{eventId}/delete.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: externalevent.get\n  description: Endpoint permission (externalevent) enabling GET /v2/event/{eventId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: externalevent.list\n  description: Endpoint permission (externalevent) enabling GET /v2/event.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: externalevent.trigger\n  description: Endpoint permission (externalevent) enabling POST /v2/event/{eventId}/trigger.\n\
  \  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: externalevent.update\n  description: Endpoint permission (externalevent) enabling POST /v2/event/{eventId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: externalevent.usages\n  description: Endpoint permission (externalevent) enabling GET /v2/event/{eventId}/usages.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: field.create\n  description: Endpoint permission (field) enabling POST /v2/field.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: field.delete\n  description: Endpoint permission (field) enabling DELETE /v2/field/{fieldId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: field.get\n\
  \  description: Endpoint permission (field) enabling GET /v2/field.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: field.list\n  description: Endpoint permission (field) enabling GET /v2/field/translate/{languageId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: field.multichoice.list\n  description: Endpoint permission (field) enabling GET /v2/field/choices.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: field.singlechoice.get\n  description: Endpoint permission (field) enabling GET /v2/field/{fieldId}/choice.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: field.singlechoice.lang.list\n  description: Endpoint permission (field) enabling GET /v2/field/{fieldId}/choice/lang/{languageId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n\
  - scope: field.singlechoice.trans.list\n  description: Endpoint permission (field) enabling GET /v2/field/{fieldId}/choice/translate/{languageId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: form.list\n  description: Endpoint permission (form) enabling GET /v2/form.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: form.trigger\n  description: Endpoint permission (form) enabling POST /v2/form/{formId}/trigger.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: keyring.key.delete\n  description: Endpoint permission (keyring) enabling POST /v2/keyring/keys/{keyId}/delete.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: keyring.key.list\n  description: Endpoint permission (keyring) enabling POST /v2/keyring/keys.\n\
  \  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: mediadb.file.create\n  description: Endpoint permission (mediadb) enabling POST /v2/file.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: mediadb.file.delete\n  description: Endpoint permission (mediadb) enabling POST /v2/file/{fileId}/delete.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: mediadb.file.get\n  description: Endpoint permission (mediadb) enabling GET /v2/file/{fileId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: mediadb.file.list\n  description: Endpoint permission (mediadb) enabling GET /v2/file.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: mediadb.folder.create\n  description:\
  \ Endpoint permission (mediadb) enabling POST /v2/folder.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: mediadb.folder.list\n  description: Endpoint permission (mediadb) enabling GET /v2/folder.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: program.abort\n  description: Endpoint permission (program / programresource) enabling POST /v2/ac/programs/{programId}/abort.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: program.delete\n  description: Endpoint permission (program / programresource) enabling POST /v2/ac/programs/{programId}/delete.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: program.get\n  description: Endpoint permission (program / programresource) enabling GET /v2/ac/programs.\n  sources:\n  -\
  \ https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: program.start\n  description: Endpoint permission (program / programresource) enabling POST /v2/ac/programs/entrypoints/{nodeType}/resources/{resourceId}/runs.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: programresource.list\n  description: Endpoint permission (program / programresource) enabling GET /v2/programresource.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: segment.contact.count\n  description: Endpoint permission (segment) enabling GET /v2/filter/{segmentId}/contacts/count.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: segment.contact.list\n  description: Endpoint permission (segment) enabling GET /v2/filter/{segmentId}/contacts.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n\
  - scope: segment.contact.lookup\n  description: Endpoint permission (segment) enabling GET /v2/filter/{segmentId}/contacts/{contactId}.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: segment.contact.run\n  description: Endpoint permission (segment) enabling POST /v2/filter/{segmentId}/single_runs.\n  sources:\n  - https://dev.emarsys.com/docs/core-api-reference/ef41493bd7812-endpoint-permission-settings\n- scope: segment.contact.run.status\n \n\n# --- truncated at 32 KB (35 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/emarsys/refs/heads/main/scopes/emarsys-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emarsys/refs/heads/main/scopes/emarsys-scopes.yml
summary_line: 156 scopes · clientCredentials
tags:
- Marketing Automation
- Customer Engagement
- Email Marketing
- Omnichannel
- Customer Data Platform
- SAP
token_urls:
- https://api.emarsys.net/api/v3/auth/token
---
