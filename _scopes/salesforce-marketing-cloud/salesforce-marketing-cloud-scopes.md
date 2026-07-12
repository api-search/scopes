---
authorization_urls: []
description: ''
docs: https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Salesforce Marketing Cloud Scopes
name_suffix: OAuth Scopes
note: Marketing Cloud Engagement scopes are assigned to an installed package's API integration in Setup (not requested freely at authorization time); the token is limited to the scopes selected for that integration. Categories and access levels are described at https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html.
overview: 'Salesforce Marketing Cloud publishes 42 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Marketing Cloud API on a user''s behalf.


  Tokens are issued from https://YOUR_SUBDOMAIN.auth.marketingcloudapis.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schemes:
- description: Marketing Cloud uses OAuth 2.0 client credentials flow for authentication. Obtain a client ID and secret from an installed package in Marketing Cloud Setup, then exchange them for an access token at the authentication endpoint.
  flows:
  - flow: clientCredentials
    tokenUrl: https://YOUR_SUBDOMAIN.auth.marketingcloudapis.com/v2/token
  name: OAuth2
  source: openapi/salesforce-marketing-cloud-openapi.yml
scope_count: 42
scope_names:
- email_read
- email_write
- email_send
- push_read
- push_write
- push_send
- sms_read
- sms_write
- sms_send
- documents_and_images_read
- documents_and_images_write
- saved_content_read
- saved_content_write
- automations_read
- journeys_read
- audiences_read
- list_and_subscribers_read
- list_and_subscribers_write
- Contacts_access
- data_extensions_read
- data_extensions_write
- file_location_create
- file_location_view
- file_location_delete
- tracking_events_read
- approvals_read
- approvals_write
- campaign_read
- campaign_write
- tags_read
- tags_write
- tags_create
- tags_edit
- tags_delete
- event_notification_callback_create
- event_notification_callback_read
- event_notification_callback_update
- event_notification_callback_delete
- event_notification_subscription_create
- event_notification_subscription_read
- event_notification_subscription_update
- event_notification_subscription_delete
scopes:
- description: Enables email message management and sending (read access).
  flows: []
  scope: email_read
- description: Enables email message management and sending (write access).
  flows: []
  scope: email_write
- description: Enables email message management and sending (send access).
  flows: []
  scope: email_send
- description: Enables Push message management and sending (read access).
  flows: []
  scope: push_read
- description: Enables Push message management and sending (write access).
  flows: []
  scope: push_write
- description: Enables Push message management and sending (send access).
  flows: []
  scope: push_send
- description: Enables SMS message management and sending (read access).
  flows: []
  scope: sms_read
- description: Enables SMS message management and sending (write access).
  flows: []
  scope: sms_write
- description: Enables SMS message management and sending (send access).
  flows: []
  scope: sms_send
- description: Enables management of documents and images in the portfolio or image library (read access).
  flows: []
  scope: documents_and_images_read
- description: Enables management of documents and images in the portfolio or image library (write access).
  flows: []
  scope: documents_and_images_write
- description: Enables management of content saved in content areas, surveys, and coupons (read access).
  flows: []
  scope: saved_content_read
- description: Enables management of content saved in content areas, surveys, and coupons (write access).
  flows: []
  scope: saved_content_write
- description: Enables management of Automation Studio programs and activities (read access).
  flows: []
  scope: automations_read
- description: Enables management of Journeys (read access).
  flows: []
  scope: journeys_read
- description: Read access to audience data.
  flows: []
  scope: audiences_read
- description: Enables management of subscribers, lists, groups, filters, measures, and preference management (read access).
  flows: []
  scope: list_and_subscribers_read
- description: Enables management of subscribers, lists, groups, filters, measures, and preference management (write access).
  flows: []
  scope: list_and_subscribers_write
- description: Grants access to Contacts REST API resources.
  flows: []
  scope: Contacts_access
- description: Enables management of data extensions and relationships (read access).
  flows: []
  scope: data_extensions_read
- description: Enables management of data extensions and relationships (write access).
  flows: []
  scope: data_extensions_write
- description: Create access to file locations used for file transfer and import operations.
  flows: []
  scope: file_location_create
- description: View access to file locations used for file transfer and import operations.
  flows: []
  scope: file_location_view
- description: Delete access to file locations used for file transfer and import operations.
  flows: []
  scope: file_location_delete
- description: Enables management of tracking event data associated with channels (read access).
  flows: []
  scope: tracking_events_read
- description: Enables management of approval items (read access).
  flows: []
  scope: approvals_read
- description: Enables management of approval items; can edit and delete approval comments (write access).
  flows: []
  scope: approvals_write
- description: Enables management of campaigns (read access).
  flows: []
  scope: campaign_read
- description: Enables management of campaigns (write access).
  flows: []
  scope: campaign_write
- description: Read access to tags.
  flows: []
  scope: tags_read
- description: Write access to tags.
  flows: []
  scope: tags_write
- description: Create access to tags.
  flows: []
  scope: tags_create
- description: Edit access to tags.
  flows: []
  scope: tags_edit
- description: Delete access to tags.
  flows: []
  scope: tags_delete
- description: Create Event Notification Service callbacks.
  flows: []
  scope: event_notification_callback_create
- description: Read Event Notification Service callbacks.
  flows: []
  scope: event_notification_callback_read
- description: Update Event Notification Service callbacks.
  flows: []
  scope: event_notification_callback_update
- description: Delete Event Notification Service callbacks.
  flows: []
  scope: event_notification_callback_delete
- description: Create Event Notification Service subscriptions.
  flows: []
  scope: event_notification_subscription_create
- description: Read Event Notification Service subscriptions.
  flows: []
  scope: event_notification_subscription_read
- description: Update Event Notification Service subscriptions.
  flows: []
  scope: event_notification_subscription_update
- description: Delete Event Notification Service subscriptions.
  flows: []
  scope: event_notification_subscription_delete
slug: salesforce-marketing-cloud-scopes
source_filename: salesforce-marketing-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/salesforce-marketing-cloud-openapi.yml\ndocs: https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\nnote: Marketing Cloud Engagement scopes are assigned to an installed package's API\n  integration in Setup (not requested freely at authorization time); the token is\n  limited to the scopes selected for that integration. Categories and access levels\n  are described at https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html.\nschemes:\n- name: OAuth2\n  source: openapi/salesforce-marketing-cloud-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://YOUR_SUBDOMAIN.auth.marketingcloudapis.com/v2/token\n  description: Marketing Cloud uses OAuth 2.0 client credentials flow for authentication. Obtain\n    a client ID and secret from an installed package in Marketing Cloud Setup,\
  \ then exchange\n    them for an access token at the authentication endpoint.\nscopes:\n- scope: email_read\n  description: Enables email message management and sending (read access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: email_write\n  description: Enables email message management and sending (write access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: email_send\n  description: Enables email message management and sending (send access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n\
  \  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: push_read\n  description: Enables Push message management and sending (read access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: push_write\n  description: Enables Push message management and sending (write access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: push_send\n  description: Enables Push message management and sending (send access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n\
  \  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: sms_read\n  description: Enables SMS message management and sending (read access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: sms_write\n  description: Enables SMS message management and sending (write access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: sms_send\n  description: Enables SMS message management and sending (send access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n\
  \  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: documents_and_images_read\n  description: Enables management of documents and images in the portfolio or image\n    library (read access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: documents_and_images_write\n  description: Enables management of documents and images in the portfolio or image\n    library (write access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: saved_content_read\n  description: Enables management of content saved\
  \ in content areas, surveys, and\n    coupons (read access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: saved_content_write\n  description: Enables management of content saved in content areas, surveys, and\n    coupons (write access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: automations_read\n  description: Enables management of Automation Studio programs and activities (read\n    access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n\
  \  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: journeys_read\n  description: Enables management of Journeys (read access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: audiences_read\n  description: Read access to audience data.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: list_and_subscribers_read\n  description: Enables management of subscribers, lists, groups, filters, measures,\n    and preference management (read access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n\
  \  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: list_and_subscribers_write\n  description: Enables management of subscribers, lists, groups, filters, measures,\n    and preference management (write access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: Contacts_access\n  description: Grants access to Contacts REST API resources.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: data_extensions_read\n  description: Enables management of data extensions and relationships (read access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n\
  \  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: data_extensions_write\n  description: Enables management of data extensions and relationships (write access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: file_location_create\n  description: Create access to file locations used for file transfer and import\n    operations.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: file_location_view\n  description: View access to file locations used for file transfer and import operations.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n\
  - scope: file_location_delete\n  description: Delete access to file locations used for file transfer and import\n    operations.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: tracking_events_read\n  description: Enables management of tracking event data associated with channels\n    (read access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: approvals_read\n  description: Enables management of approval items (read access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n\
  - scope: approvals_write\n  description: Enables management of approval items; can edit and delete approval\n    comments (write access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: campaign_read\n  description: Enables management of campaigns (read access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: campaign_write\n  description: Enables management of campaigns (write access).\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n\
  - scope: tags_read\n  description: Read access to tags.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: tags_write\n  description: Write access to tags.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/guide/data-access-permissions.html\n- scope: tags_create\n  description: Create access to tags.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: tags_edit\n  description: Edit access to tags.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: tags_delete\n  description: Delete\
  \ access to tags.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: event_notification_callback_create\n  description: Create Event Notification Service callbacks.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: event_notification_callback_read\n  description: Read Event Notification Service callbacks.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: event_notification_callback_update\n  description: Update Event Notification Service callbacks.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: event_notification_callback_delete\n\
  \  description: Delete Event Notification Service callbacks.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: event_notification_subscription_create\n  description: Create Event Notification Service subscriptions.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: event_notification_subscription_read\n  description: Read Event Notification Service subscriptions.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n- scope: event_notification_subscription_update\n  description: Update Event Notification Service subscriptions.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n\
  - scope: event_notification_subscription_delete\n  description: Delete Event Notification Service subscriptions.\n  sources:\n  - https://developer.salesforce.com/docs/marketing/marketing-cloud/references/mc_rest_rest_permission_scopes/rest-permissions-and-scopes.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/scopes/salesforce-marketing-cloud-scopes.yml
summary_line: 42 scopes · clientCredentials
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
token_urls:
- https://YOUR_SUBDOMAIN.auth.marketingcloudapis.com/v2/token
---
