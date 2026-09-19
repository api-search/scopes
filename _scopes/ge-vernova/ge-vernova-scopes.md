---
authorization_urls: []
description: ''
docs: https://www.gevernova.com/software/documentation/uaa/version2025/r_proficyauth_historian_groups_in_uaa.html
flows:
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Ge Vernova Scopes
name_suffix: OAuth Scopes
note: Proficy Authentication (Cloud Foundry UAA) is the OAuth2 authorization server for the on-premises Proficy products. GE Vernova publishes the assignable scope list per product as reference tables in the Proficy Authentication documentation; the scopes below are transcribed verbatim from those tables. There is no OpenAPI document to derive these from — no GE Vernova Electrification Software product publishes a machine-readable contract — so this file is searched, not derived.
overview: 'GE Vernova publishes 27 OAuth 2.0 scopes via the password and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the GE Vernova API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GE Vernova
provider_slug: ge-vernova
schemes:
- flows:
  - flow: password
  - flow: clientCredentials
  name: ProficyAuthentication
  source: https://www.gevernova.com/software/documentation/uaa/version2025/index.html
  type: oauth2
scope_count: 27
scope_names:
- historian_rest_api.read
- historian_rest_api.write
- historian_rest_api.admin
- historian_enterprise.admin
- historian_enterprise.user
- historian_visualization.admin
- historian_visualization.user
- ih_archive_admins
- ih_audited_writers
- ih_collector_admins
- ih_readers
- ih_security_admins
- ih_tag_admins
- ih_unaudited_logins
- ih_unaudited_writers
- iqp.clouduser
- iqp.developer
- iqp.user
- iqp.nodered
- iqp.studioAdmin
- iqp.tenantAdmin
- proficy_client.manage
- scada.fix_shared_IFIX_PROFICY_AUTH_ADMIN
- scada.fix.shared.APPLICATION_DESIGNER
- scada.fix.shared.OPERATORS
- scada.fix.shared.SUPERVISORS
- scada.proficy.admin
scopes:
- description: Provides read access to the Historian public REST API.
  flows: []
  scope: historian_rest_api.read
- description: Provides write access to the Historian public REST API.
  flows: []
  scope: historian_rest_api.write
- description: Provides read/write access to the Historian public REST API.
  flows: []
  scope: historian_rest_api.admin
- description: Provides read/write access to Configuration Hub APIs.
  flows: []
  scope: historian_enterprise.admin
- description: Allows access to Configuration Hub APIs.
  flows: []
  scope: historian_enterprise.user
- description: Provides access to Trend Client and the Web Admin console.
  flows: []
  scope: historian_visualization.admin
- description: Allows access to Trend Client.
  flows: []
  scope: historian_visualization.user
- description: Provides the ability to create, modify, and remove archives.
  flows: []
  scope: ih_archive_admins
- description: Allows data writes and produces a message each time a data value is added or changed.
  flows: []
  scope: ih_audited_writers
- description: Allows the ability to add collector instances and change their destination.
  flows: []
  scope: ih_collector_admins
- description: Provides the ability to read data and system statistics, and access to Historian Administrator.
  flows: []
  scope: ih_readers
- description: Historian power security users; rights to all Historian functions.
  flows: []
  scope: ih_security_admins
- description: Ability to create, modify, and remove tags; tag-level security can override other groups.
  flows: []
  scope: ih_tag_admins
- description: Allow connections to the Data Archiver without creating login-successful audit messages.
  flows: []
  scope: ih_unaudited_logins
- description: Ability to write data without creating any messages.
  flows: []
  scope: ih_unaudited_writers
- description: Assigned to users who want to use the REST API, mainly the M2M Device RESTful APIs.
  flows: []
  scope: iqp.clouduser
- description: Assigned to developer users; an associated application user account is generated automatically.
  flows: []
  scope: iqp.developer
- description: Assigned to application users; access only to the applications they are granted.
  flows: []
  scope: iqp.user
- description: Assigned to users who need access to the Dataflow Editor.
  flows: []
  scope: iqp.nodered
- description: Access to the Administrator Console to configure global settings for an Operations Hub instance.
  flows: []
  scope: iqp.studioAdmin
- description: Administrative authority at the tenant or system level.
  flows: []
  scope: iqp.tenantAdmin
- description: Controls who can delete clients within Proficy Authentication.
  flows: []
  scope: proficy_client.manage
- description: Allows access to all iFIX application features.
  flows: []
  scope: scada.fix_shared_IFIX_PROFICY_AUTH_ADMIN
- description: Access to Configuration Hub and iFIX connection, database and model features.
  flows: []
  scope: scada.fix.shared.APPLICATION_DESIGNER
- description: Run-mode-only access for a user in iFIX.
  flows: []
  scope: scada.fix.shared.OPERATORS
- description: WorkSpace run and configure mode, background task exit, and iFIX system shutdown.
  flows: []
  scope: scada.fix.shared.SUPERVISORS
- description: Access to the iFIX Projects panel and Deploy operations from Configuration Hub.
  flows: []
  scope: scada.proficy.admin
slug: ge-vernova-scopes
source_filename: ge-vernova-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://www.gevernova.com/software/documentation/uaa/version2025/index.html\ndocs: https://www.gevernova.com/software/documentation/uaa/version2025/r_proficyauth_historian_groups_in_uaa.html\nnote: >-\n  Proficy Authentication (Cloud Foundry UAA) is the OAuth2 authorization server for the on-premises\n  Proficy products. GE Vernova publishes the assignable scope list per product as reference tables\n  in the Proficy Authentication documentation; the scopes below are transcribed verbatim from those\n  tables. There is no OpenAPI document to derive these from — no GE Vernova Electrification\n  Software product publishes a machine-readable contract — so this file is searched, not derived.\nschemes:\n  - name: ProficyAuthentication\n    type: oauth2\n    source: https://www.gevernova.com/software/documentation/uaa/version2025/index.html\n    flows:\n      - flow: password\n      - flow: clientCredentials\nscopes:\n  - scope: historian_rest_api.read\n\
  \    description: Provides read access to the Historian public REST API.\n    product: Proficy Historian\n    sources: [https://www.gevernova.com/software/documentation/uaa/version2025/r_proficyauth_historian_groups_in_uaa.html]\n  - scope: historian_rest_api.write\n    description: Provides write access to the Historian public REST API.\n    product: Proficy Historian\n  - scope: historian_rest_api.admin\n    description: Provides read/write access to the Historian public REST API.\n    product: Proficy Historian\n  - scope: historian_enterprise.admin\n    description: Provides read/write access to Configuration Hub APIs.\n    product: Proficy Historian\n  - scope: historian_enterprise.user\n    description: Allows access to Configuration Hub APIs.\n    product: Proficy Historian\n  - scope: historian_visualization.admin\n    description: Provides access to Trend Client and the Web Admin console.\n    product: Proficy Historian\n  - scope: historian_visualization.user\n    description:\
  \ Allows access to Trend Client.\n    product: Proficy Historian\n  - scope: ih_archive_admins\n    description: Provides the ability to create, modify, and remove archives.\n    product: Proficy Historian\n  - scope: ih_audited_writers\n    description: Allows data writes and produces a message each time a data value is added or changed.\n    product: Proficy Historian\n  - scope: ih_collector_admins\n    description: Allows the ability to add collector instances and change their destination.\n    product: Proficy Historian\n  - scope: ih_readers\n    description: Provides the ability to read data and system statistics, and access to Historian Administrator.\n    product: Proficy Historian\n  - scope: ih_security_admins\n    description: Historian power security users; rights to all Historian functions.\n    product: Proficy Historian\n  - scope: ih_tag_admins\n    description: Ability to create, modify, and remove tags; tag-level security can override other groups.\n    product: Proficy\
  \ Historian\n  - scope: ih_unaudited_logins\n    description: Allow connections to the Data Archiver without creating login-successful audit messages.\n    product: Proficy Historian\n  - scope: ih_unaudited_writers\n    description: Ability to write data without creating any messages.\n    product: Proficy Historian\n  - scope: iqp.clouduser\n    description: Assigned to users who want to use the REST API, mainly the M2M Device RESTful APIs.\n    product: Proficy Operations Hub\n    sources: [https://www.gevernova.com/software/documentation/uaa/version2025/r_proficyauth_opshub_groups_in_uaa.html]\n  - scope: iqp.developer\n    description: Assigned to developer users; an associated application user account is generated automatically.\n    product: Proficy Operations Hub\n  - scope: iqp.user\n    description: Assigned to application users; access only to the applications they are granted.\n    product: Proficy Operations Hub\n  - scope: iqp.nodered\n    description: Assigned to users who\
  \ need access to the Dataflow Editor.\n    product: Proficy Operations Hub\n  - scope: iqp.studioAdmin\n    description: Access to the Administrator Console to configure global settings for an Operations Hub instance.\n    product: Proficy Operations Hub\n  - scope: iqp.tenantAdmin\n    description: Administrative authority at the tenant or system level.\n    product: Proficy Operations Hub\n  - scope: proficy_client.manage\n    description: Controls who can delete clients within Proficy Authentication.\n    product: Proficy Authentication\n    sources: [https://www.gevernova.com/software/documentation/uaa/version2025/r_proficyauth_uaa_groups_in_uaa.html]\n  - scope: scada.fix_shared_IFIX_PROFICY_AUTH_ADMIN\n    description: Allows access to all iFIX application features.\n    product: Proficy iFIX\n    sources: [https://www.gevernova.com/software/documentation/uaa/version2025/r_proficyauth_ifix_groups_in_uaa.html]\n  - scope: scada.fix.shared.APPLICATION_DESIGNER\n    description: Access\
  \ to Configuration Hub and iFIX connection, database and model features.\n    product: Proficy iFIX\n  - scope: scada.fix.shared.OPERATORS\n    description: Run-mode-only access for a user in iFIX.\n    product: Proficy iFIX\n  - scope: scada.fix.shared.SUPERVISORS\n    description: WorkSpace run and configure mode, background task exit, and iFIX system shutdown.\n    product: Proficy iFIX\n  - scope: scada.proficy.admin\n    description: Access to the iFIX Projects panel and Deploy operations from Configuration Hub.\n    product: Proficy iFIX\nplant_applications_scopes:\n  note: >-\n    Plant Applications publishes a scope-per-application table (mes.<application>.user). Transcribed\n    verbatim; the \"applies to\" column names the Web Client application each scope unlocks.\n  source: https://www.gevernova.com/software/documentation/uaa/version2025/r_proficyauth_plantapps_groups_in_uaa.html\n  scopes:\n    - {scope: mes.activities.user, applies_to: Activities}\n    - {scope: mes.alarms.user,\
  \ applies_to: Alarms / Alarm Notifications}\n    - {scope: mes.analysis.user, applies_to: Analysis}\n    - {scope: mes.approval_cockpit.user, applies_to: Approval Cockpit}\n    - {scope: mes.autolog.user, applies_to: Autolog}\n    - {scope: mes.bom_editor.user, applies_to: BOM Editor}\n    - {scope: mes.configuration_management.user, applies_to: Configuration}\n    - {scope: mes.downtime.user, applies_to: Downtime}\n    - {scope: mes.engineeringChangeOrder.user, applies_to: Engineering Change Orders}\n    - {scope: mes.equipment.user, applies_to: OEE Dashboard}\n    - {scope: mes.genealogy.user, applies_to: Genealogy}\n    - {scope: mes.lineoverview.user, applies_to: Line Overview}\n    - {scope: mes.my_machines.user, applies_to: My Machines}\n    - {scope: mes.ncm_management.user, applies_to: Non Conformance}\n    - {scope: mes.operations.user, applies_to: Unit Operations}\n    - {scope: mes.operatorlog.user, applies_to: Operator Log}\n    - {scope: mes.order_management.user, applies_to:\
  \ Work Order Manager}\n    - {scope: mes.process_orders.user, applies_to: Process Orders}\n    - {scope: mes.property_definition.user, applies_to: Property Definition}\n    - {scope: mes.receiving_inspection.user, applies_to: Receiving Inspection}\n    - {scope: mes.reports.user, applies_to: Reports}\n    - {scope: mes.route_management.user, applies_to: Route Editor}\n    - {scope: mes.security_management.user, applies_to: Security}\n    - {scope: mes.time_booking.user, applies_to: Time Booking}\n    - {scope: mes.waste.user, applies_to: Waste}\n    - {scope: mes.work_queue.user, applies_to: Work Queue}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ge-vernova/refs/heads/main/scopes/ge-vernova-scopes.yml
summary_line: 27 scopes · password/clientCredentials
tags:
- Decarbonization
- Electrification
- Energy
- Fortune 500
- Power
- Renewable Energy
- Sustainability
- Industrial
- Asset Performance Management
- Manufacturing Execution Systems
- Historian
- Grid
token_urls: []
---
