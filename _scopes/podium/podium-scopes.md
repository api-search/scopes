---
api_specs:
- filename: podium-accounts-openapi.yml
  format: yaml
  label: Podium API
  slug: podium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podium/refs/heads/main/openapi/podium-accounts-openapi.yml
authorization_urls:
- https://api.podium.com/oauth/authorize
description: ''
docs: https://docs.podium.com/docs/oauth-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Podium Scopes
name_suffix: OAuth Scopes
note: Union of the 17 scopes published on Podium's OAuth scopes reference page and the 24 scopes named in `Required scope:` lines inside the 12 harvested OpenAPI definitions. Eight scopes are enforced by operations but absent from the published reference page (read_phones, read_products, read_templates, write_campaigns, write_feedback, write_products, write_templates, write_writebacks); one scope (write_data_feed_event) is published but has no operation in the harvested specs.
overview: 'Podium publishes 25 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Podium API on a user''s behalf.


  Tokens are issued from https://api.podium.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Podium
provider_slug: podium
schemes:
- flows:
  - authorizationUrl: https://api.podium.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.podium.com/oauth/token
    tokenUrl: https://api.podium.com/oauth/token
  name: OAuth2
  source: https://docs.podium.com/docs/oauth
  type: oauth2
scope_count: 25
scope_names:
- read_campaigns
- read_contacts
- read_feedback
- read_locations
- read_messages
- read_organizations
- read_payments
- read_phones
- read_products
- read_reviews
- read_templates
- read_users
- write_appointments
- write_campaign_messages
- write_campaigns
- write_contacts
- write_data_feed_event
- write_feedback
- write_locations
- write_messages
- write_payments
- write_products
- write_reviews
- write_templates
- write_writebacks
scopes:
- description: Grant access to read campaign data for the user's locations.
  flows:
  - authorizationCode
  scope: read_campaigns
- description: Grant access to all contact data for the user's locations.
  flows:
  - authorizationCode
  scope: read_contacts
- description: Grant access to all feedback data for the user's locations.
  flows:
  - authorizationCode
  scope: read_feedback
- description: Grant access to the user's locations.
  flows:
  - authorizationCode
  scope: read_locations
- description: Grant access to all messages for the user's locations.
  flows:
  - authorizationCode
  scope: read_messages
- description: Grant access to the user's organization.
  flows:
  - authorizationCode
  scope: read_organizations
- description: Grant access to all payment data for to the user's locations.
  flows:
  - authorizationCode
  scope: read_payments
- description: Scope required by the operations listed below; not present on the published scopes reference page.
  flows:
  - authorizationCode
  scope: read_phones
- description: Scope required by the operations listed below; not present on the published scopes reference page.
  flows:
  - authorizationCode
  scope: read_products
- description: Grant access to all review data for the user's locations.
  flows:
  - authorizationCode
  scope: read_reviews
- description: Scope required by the operations listed below; not present on the published scopes reference page.
  flows:
  - authorizationCode
  scope: read_templates
- description: Grant access to all user data for the user's locations.
  flows:
  - authorizationCode
  scope: read_users
- description: Grant access to create appointments in the user's locations.
  flows:
  - authorizationCode
  scope: write_appointments
- description: Grant access to write campaign messages for the user's locations.
  flows:
  - authorizationCode
  scope: write_campaign_messages
- description: Scope required by the operations listed below; not present on the published scopes reference page.
  flows:
  - authorizationCode
  scope: write_campaigns
- description: Grant access to create, update, and delete contact data for the user's locations.
  flows:
  - authorizationCode
  scope: write_contacts
- description: Grant access to trigger data feed events for the user's locations.
  flows:
  - authorizationCode
  scope: write_data_feed_event
- description: Scope required by the operations listed below; not present on the published scopes reference page.
  flows:
  - authorizationCode
  scope: write_feedback
- description: Grant access to write locations.
  flows:
  - authorizationCode
  scope: write_locations
- description: Grant access to write messages in the user's locations.
  flows:
  - authorizationCode
  scope: write_messages
- description: Grant access to create payments for all the user's locations.
  flows:
  - authorizationCode
  scope: write_payments
- description: Scope required by the operations listed below; not present on the published scopes reference page.
  flows:
  - authorizationCode
  scope: write_products
- description: Grant access to create reviews data for all the user's locations.
  flows:
  - authorizationCode
  scope: write_reviews
- description: Scope required by the operations listed below; not present on the published scopes reference page.
  flows:
  - authorizationCode
  scope: write_templates
- description: Scope required by the operations listed below; not present on the published scopes reference page.
  flows:
  - authorizationCode
  scope: write_writebacks
slug: podium-scopes
source_filename: podium-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.podium.com/docs/oauth-scopes\ndocs: https://docs.podium.com/docs/oauth-scopes\nnote: Union of the 17 scopes published on Podium's OAuth scopes reference page and the 24 scopes named\n  in `Required scope:` lines inside the 12 harvested OpenAPI definitions. Eight scopes are enforced by\n  operations but absent from the published reference page (read_phones, read_products, read_templates,\n  write_campaigns, write_feedback, write_products, write_templates, write_writebacks); one scope (write_data_feed_event)\n  is published but has no operation in the harvested specs.\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://docs.podium.com/docs/oauth\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.podium.com/oauth/authorize\n    tokenUrl: https://api.podium.com/oauth/token\n    refreshUrl: https://api.podium.com/oauth/token\nscope_count: 25\nundocumented_scope_count: 8\nscopes:\n- scope:\
  \ read_campaigns\n  description: Grant access to read campaign data for the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - campaign.get\n  - campaign.index\n  - campaign_interaction.index\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-campaigns-openapi.yml\n- scope: read_contacts\n  description: Grant access to all contact data for the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - contact.get\n  - contact.index\n  - contact_entity_attribute.get\n  - contact_entity_attribute.index\n  - contact_entity_tag.get\n  - contact_entity_tag.list\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-contacts-openapi.yml\n- scope: read_feedback\n  description: Grant access to all feedback data for the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - feedback.index\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n\
  \  - openapi/podium-feedback-surveys-openapi.yml\n- scope: read_locations\n  description: Grant access to the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - location.get\n  - location.index\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-accounts-openapi.yml\n- scope: read_messages\n  description: Grant access to all messages for the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - conversation.get\n  - conversation.index\n  - conversation_assignee.get\n  - message.get\n  - message.index\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-conversations-openapi.yml\n  - openapi/podium-messenger-openapi.yml\n- scope: read_organizations\n  description: Grant access to the user's organization.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - organization.get\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-accounts-openapi.yml\n\
  - scope: read_payments\n  description: Grant access to all payment data for to the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - Refund.get\n  - invoice.get\n  - invoice.index\n  - payment.get\n  - reader.get\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-payments-openapi.yml\n- scope: read_phones\n  description: Scope required by the operations listed below; not present on the published scopes reference\n    page.\n  documented: false\n  flows:\n  - authorizationCode\n  operations:\n  - call.get\n  sources:\n  - openapi/podium-phones-openapi.yml\n- scope: read_products\n  description: Scope required by the operations listed below; not present on the published scopes reference\n    page.\n  documented: false\n  flows:\n  - authorizationCode\n  operations:\n  - Product.get\n  - Product.index\n  sources:\n  - openapi/podium-products-openapi.yml\n- scope: read_reviews\n  description: Grant access to all review data\
  \ for the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - review.get\n  - review.index\n  - review_invite.get\n  - review_invite.index\n  - review_response.index\n  - review_sites_summary.index\n  - review_summary.index\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-reviews-openapi.yml\n- scope: read_templates\n  description: Scope required by the operations listed below; not present on the published scopes reference\n    page.\n  documented: false\n  flows:\n  - authorizationCode\n  operations:\n  - Template.index\n  sources:\n  - openapi/podium-messenger-openapi.yml\n- scope: read_users\n  description: Grant access to all user data for the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - user.get\n  - user.index\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-accounts-openapi.yml\n- scope: write_appointments\n  description: Grant access to\
  \ create appointments in the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - appointment.create\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-appointments-openapi.yml\n- scope: write_campaign_messages\n  description: Grant access to write campaign messages for the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - message.create_campaign_message\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-campaigns-openapi.yml\n- scope: write_campaigns\n  description: Scope required by the operations listed below; not present on the published scopes reference\n    page.\n  documented: false\n  flows:\n  - authorizationCode\n  operations:\n  - campaign.create\n  - campaign.delete\n  - campaign.update\n  sources:\n  - openapi/podium-campaigns-openapi.yml\n- scope: write_contacts\n  description: Grant access to create, update, and delete contact data for the\
  \ user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - contact.create\n  - contact.delete\n  - contact.update\n  - contact_attribute.create\n  - contact_attribute.delete\n  - contact_attribute.update\n  - contact_entity_attribute.create\n  - contact_entity_attribute.delete\n  - contact_entity_attribute.update\n  - contact_entity_tag.create\n  - contact_entity_tag.update\n  - contact_tag.create\n  - contact_tag.create (2)\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-contacts-openapi.yml\n- scope: write_data_feed_event\n  description: Grant access to trigger data feed events for the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations: []\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n- scope: write_feedback\n  description: Scope required by the operations listed below; not present on the published scopes reference\n    page.\n  documented: false\n  flows:\n  - authorizationCode\n\
  \  operations:\n  - feedback_creation.create\n  sources:\n  - openapi/podium-feedback-surveys-openapi.yml\n- scope: write_locations\n  description: Grant access to write locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - location.update\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-accounts-openapi.yml\n- scope: write_messages\n  description: Grant access to write messages in the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - conversation.update\n  - conversation_assignee.update\n  - conversation_note.create_conversation_note\n  - message.import\n  - message.send\n  - message.send_with_attachment\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-conversations-openapi.yml\n  - openapi/podium-messenger-openapi.yml\n- scope: write_payments\n  description: Grant access to create payments for all the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n\
  \  operations:\n  - Refund.create\n  - invoice.cancel\n  - invoice.charge\n  - invoice.create\n  - invoice.refund\n  - invoice.setup\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-payments-openapi.yml\n- scope: write_products\n  description: Scope required by the operations listed below; not present on the published scopes reference\n    page.\n  documented: false\n  flows:\n  - authorizationCode\n  operations:\n  - Product.upload_images\n  - product_image.delete\n  sources:\n  - openapi/podium-products-openapi.yml\n- scope: write_reviews\n  description: Grant access to create reviews data for all the user's locations.\n  documented: true\n  flows:\n  - authorizationCode\n  operations:\n  - review_attribution.create\n  - review_attribution.delete\n  - review_invite.create\n  - review_response.create\n  - review_response.update\n  sources:\n  - https://docs.podium.com/docs/oauth-scopes\n  - openapi/podium-reviews-openapi.yml\n- scope: write_templates\n  description:\
  \ Scope required by the operations listed below; not present on the published scopes reference\n    page.\n  documented: false\n  flows:\n  - authorizationCode\n  operations:\n  - Template.create\n  - Template.delete\n  - Template.update\n  sources:\n  - openapi/podium-messenger-openapi.yml\n- scope: write_writebacks\n  description: Scope required by the operations listed below; not present on the published scopes reference\n    page.\n  documented: false\n  flows:\n  - authorizationCode\n  operations:\n  - lead_writeback.get\n  sources:\n  - openapi/podium-conversations-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podium/refs/heads/main/scopes/podium-scopes.yml
summary_line: 25 scopes · authorizationCode
tags:
- Customer Communication
- Reviews
- Messaging
- Payments
- Web Chat
- Local Business
- SMS
- Lead Generation
token_urls:
- https://api.podium.com/oauth/token
---
