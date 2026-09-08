---
api_specs:
- filename: cvent-hospitality-cloud-housing-openapi.yml
  format: yaml
  label: Cvent Passkey RegLink API
  slug: passkey-reglink
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-housing-openapi.yml
- filename: cvent-hospitality-cloud-authentication-openapi.yml
  format: yaml
  label: Cvent Platform REST API (Hospitality)
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-authentication-openapi.yml
- filename: cvent-hospitality-cloud-rfp-management-openapi.yml
  format: yaml
  label: Cvent RFP Management API
  slug: rfp-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-management-openapi.yml
- filename: cvent-hospitality-cloud-rfp-requirements-openapi.yml
  format: yaml
  label: Cvent RFP Requirements API
  slug: rfp-requirements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml
- filename: cvent-hospitality-cloud-rfp-suppliers-openapi.yml
  format: yaml
  label: Cvent RFP Suppliers API
  slug: rfp-suppliers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml
- filename: cvent-hospitality-cloud-rfp-additional-details-openapi.yml
  format: yaml
  label: Cvent RFP Additional Details API
  slug: rfp-additional-details
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml
- filename: cvent-hospitality-cloud-proposal-drafts-openapi.yml
  format: yaml
  label: Cvent Proposal Draft API
  slug: proposal-drafts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml
- filename: cvent-hospitality-cloud-venue-profiles-openapi.yml
  format: yaml
  label: Cvent Venue Profiles API
  slug: venue-profiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml
- filename: cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml
  format: yaml
  label: Cvent Venue Meeting Rooms API
  slug: venue-meeting-rooms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml
- filename: cvent-hospitality-cloud-meeting-requests-openapi.yml
  format: yaml
  label: Cvent Meeting Request API
  slug: meeting-requests
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml
- filename: cvent-hospitality-cloud-travel-rfps-openapi.yml
  format: yaml
  label: Cvent Travel RFPs API
  slug: travel-rfps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml
- filename: cvent-hospitality-cloud-travel-suppliers-openapi.yml
  format: yaml
  label: Cvent Travel Suppliers API
  slug: travel-suppliers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml
- filename: cvent-hospitality-cloud-travel-accounts-openapi.yml
  format: yaml
  label: Cvent Travel Accounts API
  slug: travel-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml
- filename: cvent-hospitality-cloud-event-travel-openapi.yml
  format: yaml
  label: Cvent Event Travel API
  slug: event-travel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-event-travel-openapi.yml
- filename: cvent-hospitality-cloud-signatures-openapi.yml
  format: yaml
  label: Cvent Signatures API
  slug: signatures
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/openapi/cvent-hospitality-cloud-signatures-openapi.yml
authorization_urls:
- https://api-platform.cvent.com/ea/oauth2/authorize
description: ''
docs: https://developers.cvent.com/docs/rest-api/explanation/concepts
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cvent Hospitality Cloud Scopes
name_suffix: OAuth Scopes
note: 238 OAuth 2.0 scopes read straight out of the securitySchemes block of the OpenAPI document Cvent publishes at https://developers.cvent.com/documentation, each with Cvent's own description. The shape is <domain>/<resource>:<read|write|delete>. The hospitality domains are housing/* (15 scopes), rfp/* (11), venue/* (8), business-travel/* + business-transient/* (15) and proposal/*. Cvent's Concepts page documents how scopes are attached to an application inside a workspace, and warns that a token carrying roughly 50 or more scopes trips HTTP 431 — mint runtime tokens with only the scopes a call needs.
overview: 'Cvent Hospitality Cloud publishes 238 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cvent Hospitality Cloud API on a user''s behalf.


  Tokens are issued from https://api-platform.cvent.com/ea/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cvent Hospitality Cloud
provider_slug: cvent-hospitality-cloud
schemes:
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-authentication-openapi.yml
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  source: openapi/cvent-hospitality-cloud-authentication-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-event-travel-openapi.yml
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  source: openapi/cvent-hospitality-cloud-event-travel-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-housing-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  source: openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  source: openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-rfp-management-openapi.yml
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  source: openapi/cvent-hospitality-cloud-rfp-management-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  source: openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  source: openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-signatures-openapi.yml
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  source: openapi/cvent-hospitality-cloud-signatures-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  source: openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  source: openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  source: openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  source: openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml
scope_count: 238
scope_names:
- account/hooks:delete
- account/hooks:read
- account/hooks:write
- account/user-groups:delete
- account/user-groups:read
- account/user-groups:write
- account/users:delete
- account/users:read
- account/users:write
- appointments/appointment-attendees:read
- appointments/appointment-events:read
- appointments/appointment-types:read
- appointments/appointments:read
- appointments/appointments:write
- appointments/available-times:read
- appointments/locations:read
- attendee-insights/attendee-insights:read
- attendee-insights/scores:read
- attendee-insights/stats:read
- budget/budget-items:delete
- budget/budget-items:read
- budget/budget-items:write
- budget/budget-totals:read
- budget/budget-vendors:read
- budget/cards:read
- budget/currency-conversion-rate:delete
- budget/currency-conversion-rate:read
- budget/currency-conversion-rate:write
- budget/payments:delete
- budget/payments:read
- budget/payments:write
- budget/transactions:delete
- budget/transactions:read
- budget/transactions:write
- bulk/bulk-jobs:read
- bulk/bulk-jobs:write
- business-transient/bids:read
- business-transient/proposals:read
- business-transient/supplier-brands:read
- business-transient/supplier-chains:read
- business-transient/supplier-properties:read
- business-transient/supplier-property-rooms:read
- business-transient/travel-accounts:read
- business-transient/travel-program-questions:read
- business-transient/travel-programs:read
- business-transient/travel-supplier-accounts:read
- business-travel/bids:read
- business-travel/proposals:read
- business-travel/travel-accounts:read
- business-travel/travel-program-questions:read
- business-travel/travel-programs:read
- compliance/communications:read
- compliance/communications:write
- eMarketing/campaigns:read
- eMarketing/eMarketing-email-templates:read
- eMarketing/eMarketing-send-emails:write
- email/bounces:read
- email/email-status:read
- email/emails:read
- emarketing/emarketing-email-status:read
- event/admission-items:read
- event/air-request:read
- event/alternate-travel:read
- event/attendance-durations:read
- event/attendee-activities-metadata:delete
- event/attendee-activities-metadata:read
- event/attendee-activities-metadata:write
- event/attendee-activities:read
- event/attendee-activities:write
- event/attendee-credits:read
- event/attendee-links:delete
- event/attendee-links:read
- event/attendee-links:write
- event/attendee-messages:read
- event/attendees:read
- event/attendees:write
- event/audience-segments:read
- event/audience-segments:write
- event/contact-groups:read
- event/contact-groups:write
- event/contact-types:read
- event/contacts:delete
- event/contacts:read
- event/contacts:write
- event/contacts:write-sensitive
- event/custom-fields:read
- event/custom-fields:write
- event/discounts:write
- event/donation-items:read
- event/event-discounts:read
- event/event-discounts:write
- event/event-email-status:read
- event/event-emails:read
- event/event-emails:write
- event/event-features:read
- event/event-features:write
- event/event-user-groups:read
- event/event-user-groups:write
- event/events:read
- event/events:write
- event/fee-items:read
- event/hotel-request:read
- event/invitation-lists:read
- event/meeting-request-forms:read
- event/meeting-requests:read
- event/meeting-requests:write
- event/membership-items:read
- event/orders:read
- event/planning-documents:read
- event/players:read
- event/process-form-submissions:read
- event/program-items:delete
- event/program-items:read
- event/program-items:write
- event/quantity-items:read
- event/quantity-items:write
- event/registration-paths:read
- event/registration-types:read
- event/registration-types:write
- event/role-assignments:read
- event/session-attendance:read
- event/session-attendance:write
- event/session-categories:read
- event/session-categories:write
- event/session-enrollment:delete
- event/session-enrollment:read
- event/session-enrollment:write
- event/session-segments:read
- event/sessions:delete
- event/sessions:read
- event/sessions:write
- event/speaker-categories:read
- event/speaker-categories:write
- event/speakers:delete
- event/speakers:read
- event/speakers:write
- event/taxes:read
- event/transactions:read
- event/transactions:write
- event/video-views:read
- event/videos:read
- event/videos:write
- event/vouchers:read
- event/webcasts:delete
- event/webcasts:read
- event/webcasts:write
- event/weblinks:read
- events-plus/hubs:read
- exhibitor/badges:read
- exhibitor/badges:write
- exhibitor/booth-staff:delete
- exhibitor/booth-staff:read
- exhibitor/booth-staff:write
- exhibitor/eliterature-requests:read
- exhibitor/exhibitor-admins:read
- exhibitor/exhibitor-admins:write
- exhibitor/exhibitor-answers:read
- exhibitor/exhibitor-answers:write
- exhibitor/exhibitor-categories:delete
- exhibitor/exhibitor-categories:read
- exhibitor/exhibitor-categories:write
- exhibitor/exhibitor-contents:delete
- exhibitor/exhibitor-contents:read
- exhibitor/exhibitor-contents:write
- exhibitor/exhibitor-questions:read
- exhibitor/exhibitors:delete
- exhibitor/exhibitors:read
- exhibitor/exhibitors:write
- exhibitor/lead-qualification-answers:read
- exhibitor/lead-qualification-questions:read
- exhibitor/leads:read
- exhibitor/registration-packs:delete
- exhibitor/registration-packs:read
- exhibitor/registration-packs:write
- exhibitor/sponsorship-levels:read
- file/file:read
- file/file:write
- housing/connections:write
- housing/hotel-room-rates:write
- housing/housing-event-available-nights:read
- housing/housing-event-hotels:read
- housing/housing-event-inventory:read
- housing/housing-event-room-types:read
- housing/housing-events:read
- housing/reservation-requests:delete
- housing/reservation-requests:read
- housing/reservation-requests:write
- housing/reservations-link:delete
- housing/reservations-link:write
- housing/reservations:delete
- housing/reservations:read
- housing/reservations:write
- onsite/signatures:read
- proposal/proposals:write
- remote-printing/badge-print-jobs:read
- remote-printing/badge-print-jobs:write
- remote-printing/badge-printer-pools:read
- rfp/rfp-agenda-items:read
- rfp/rfp-attachments:read
- rfp/rfp-custom-fields:read
- rfp/rfp-guest-rooms:read
- rfp/rfp-internal-documents:read
- rfp/rfp-lead-sources:read
- rfp/rfp-past-events:read
- rfp/rfp-questions:read
- rfp/rfp-recipients-history:read
- rfp/rfp-suppliers:read
- rfp/rfps:read
- seating/assignments:read
- seating/event-seatings:read
- seating/seats:read
- seating/tables:read
- secure-ecommerce/card-tokens:write
- survey/questions:read
- survey/respondents:read
- survey/responses:read
- survey/standard-survey-email-templates:read
- survey/standard-survey-email:write
- survey/standard-survey-questions:read
- survey/standard-survey-respondents:read
- survey/standard-survey-respondents:write
- survey/standard-survey-responses:read
- survey/standard-survey-responses:write
- survey/standard-surveys:read
- survey/survey-questions:read
- survey/survey-respondents:read
- survey/survey-respondents:write
- survey/survey-responses:read
- survey/survey-responses:write
- survey/surveys:read
- venue/meeting-room-images:delete
- venue/meeting-room-images:read
- venue/meeting-room-images:write
- venue/meeting-room-overviews:read
- venue/meeting-rooms:write
- venue/venue-details-overview:read
- venue/venue-details:write
- venue/venue-facility:write
scopes:
- description: Allows the deletion of hooks.
  flows:
  - authorizationCode
  - clientCredentials
  scope: account/hooks:delete
- description: Allows the reading of hooks.
  flows:
  - authorizationCode
  - clientCredentials
  scope: account/hooks:read
- description: Allows the creation/updation of hooks.
  flows:
  - authorizationCode
  - clientCredentials
  scope: account/hooks:write
- description: Allows deletion for user groups
  flows:
  - authorizationCode
  - clientCredentials
  scope: account/user-groups:delete
- description: Allows the reading of user groups
  flows:
  - authorizationCode
  - clientCredentials
  scope: account/user-groups:read
- description: Allows the writing of user groups
  flows:
  - authorizationCode
  - clientCredentials
  scope: account/user-groups:write
- description: Allows the deletion of User
  flows:
  - authorizationCode
  - clientCredentials
  scope: account/users:delete
- description: Allows the reading of User, User Group
  flows:
  - authorizationCode
  - clientCredentials
  scope: account/users:read
- description: Allows the creation/updating of User
  flows:
  - authorizationCode
  - clientCredentials
  scope: account/users:write
- description: Allows the reading of appointment attendees and their related entities.
  flows:
  - authorizationCode
  - clientCredentials
  scope: appointments/appointment-attendees:read
- description: Allows the reading of appointment events and their related entities.
  flows:
  - authorizationCode
  - clientCredentials
  scope: appointments/appointment-events:read
- description: Allows the reading of appointment types and their related entities.
  flows:
  - authorizationCode
  - clientCredentials
  scope: appointments/appointment-types:read
- description: Allows the reading of appointment and their related entities.
  flows:
  - authorizationCode
  - clientCredentials
  scope: appointments/appointments:read
- description: Allows the writing of appointments and their related entities.
  flows:
  - authorizationCode
  - clientCredentials
  scope: appointments/appointments:write
- description: Allows the reading of availability times.
  flows:
  - authorizationCode
  - clientCredentials
  scope: appointments/available-times:read
- description: Allows the reading of appointment locations and their related entities.
  flows:
  - authorizationCode
  - clientCredentials
  scope: appointments/locations:read
- description: Allows the reading of engagement scores (attendee insights).
  flows:
  - authorizationCode
  - clientCredentials
  scope: attendee-insights/attendee-insights:read
- description: Allows the reading of scores.
  flows:
  - authorizationCode
  - clientCredentials
  scope: attendee-insights/scores:read
- description: Allows the reading of engagement score (attendee insight) stats.
  flows:
  - authorizationCode
  - clientCredentials
  scope: attendee-insights/stats:read
- description: Allows the deletion of budget items
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/budget-items:delete
- description: Allows the reading of all budget items
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/budget-items:read
- description: Allows creation/updation of budget item
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/budget-items:write
- description: Allows the reading of all event budget totals
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/budget-totals:read
- description: Allows reading of account-level budget vendors.
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/budget-vendors:read
- description: Allows the reading of cards
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/cards:read
- description: Allows deletion of currency conversion rate for currency.
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/currency-conversion-rate:delete
- description: Allows reading of currency conversion rate for currency.
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/currency-conversion-rate:read
- description: Allows creation/update of currency conversion rate for currency.
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/currency-conversion-rate:write
- description: Allows deletion of payments.
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/payments:delete
- description: Allows reading of payment for budget item.
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/payments:read
- description: Allows creation of payment in a budget item.
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/payments:write
- description: Allows delete card transactions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/transactions:delete
- description: Allows the reading of all card's transactions
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/transactions:read
- description: Allows creation of card transactions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: budget/transactions:write
- description: Allows the reading of bulk job related entities
  flows:
  - clientCredentials
  scope: bulk/bulk-jobs:read
- description: Allows the creation, update and deletion of bulk job related entities
  flows:
  - clientCredentials
  scope: bulk/bulk-jobs:write
- description: Allows the reading of Business Transient Bid data
  flows:
  - authorizationCode
  - clientCredentials
  scope: business-transient/bids:read
- description: Allows the reading of Business Transient Proposal data
  flows:
  - authorizationCode
  - clientCredentials
  scope: business-transient/proposals:read
- description: Allows the reading of a supplier brand or a list of travel supplier brands.
  flows:
  - clientCredentials
  scope: business-transient/supplier-brands:read
- description: Allows the reading of a travel supplier chain or a list of travel supplier chains.
  flows:
  - clientCredentials
  scope: business-transient/supplier-chains:read
- description: Allows the reading of a travel supplier property or a list of travel supplier properties.
  flows:
  - clientCredentials
  scope: business-transient/supplier-properties:read
- description: Allows the reading of a list of travel supplier property rooms.
  flows:
  - clientCredentials
  scope: business-transient/supplier-property-rooms:read
- description: Allows the reading of business transient travel account data.
  flows:
  - clientCredentials
  scope: business-transient/travel-accounts:read
- description: Allows the reading of business transient travel program question data.
  flows:
  - clientCredentials
  scope: business-transient/travel-program-questions:read
- description: Allows the reading of business transient travel program data.
  flows:
  - clientCredentials
  scope: business-transient/travel-programs:read
- description: Allows the reading of business transient travel supplier account data.
  flows:
  - clientCredentials
  scope: business-transient/travel-supplier-accounts:read
- description: Allows the reading of Business Travel Bid data
  flows:
  - authorizationCode
  - clientCredentials
  scope: business-travel/bids:read
- description: Allows the reading of Business Travel Proposal data
  flows:
  - authorizationCode
  - clientCredentials
  scope: business-travel/proposals:read
- description: Allows the reading of business travel account data.
  flows:
  - clientCredentials
  scope: business-travel/travel-accounts:read
- description: Allows the reading of business travel program question data.
  flows:
  - clientCredentials
  scope: business-travel/travel-program-questions:read
- description: Allows the reading of business travel program data.
  flows:
  - clientCredentials
  scope: business-travel/travel-programs:read
- description: Allows the reading of communication compliance
  flows:
  - authorizationCode
  - clientCredentials
  scope: compliance/communications:read
- description: Allows the writing of communication compliance
  flows:
  - authorizationCode
  - clientCredentials
  scope: compliance/communications:write
- description: Allows the reading of campaigns.
  flows:
  - authorizationCode
  - clientCredentials
  scope: eMarketing/campaigns:read
- description: Allows the reading of email-templates.
  flows:
  - authorizationCode
  - clientCredentials
  scope: eMarketing/eMarketing-email-templates:read
- description: Allows the writing of eMarketing emails.
  flows:
  - authorizationCode
  - clientCredentials
  scope: eMarketing/eMarketing-send-emails:write
- description: Allow the reading of email bounces.
  flows:
  - authorizationCode
  - clientCredentials
  scope: email/bounces:read
- description: Allows the reading of email statuses.
  flows:
  - authorizationCode
  - clientCredentials
  scope: email/email-status:read
- description: Allows the reading of emails.
  flows:
  - authorizationCode
  - clientCredentials
  scope: email/emails:read
- description: Allows the reading of eMarketing email statuses.
  flows:
  - authorizationCode
  - clientCredentials
  scope: emarketing/emarketing-email-status:read
- description: Allows the reading of admission items
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/admission-items:read
- description: Allow reading the air request or air actual detail for attendees.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/air-request:read
- description: Allow reading the alternate travel answers for attendees.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/alternate-travel:read
- description: Allows the read of Duration records
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendance-durations:read
- description: Allows the deletion of attendees activities metadata.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendee-activities-metadata:delete
- description: Allows the reading of attendee activities metadata.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendee-activities-metadata:read
- description: Allows the creation/updating of attendees activities metadata.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendee-activities-metadata:write
- description: Allows the reading of attendee activities.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendee-activities:read
- description: Allows the writing of external attendee activities.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendee-activities:write
- description: Allows the reading of attendee credits.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendee-credits:read
- description: Allows the deletion of attendee links
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendee-links:delete
- description: Allows the reading of attendee links
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendee-links:read
- description: Allows the creation of attendee links
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendee-links:write
- description: Allows the reading of attendee messages
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendee-messages:read
- description: Allows the reading of attendees.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendees:read
- description: Allows the creation of an attendee in an event.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/attendees:write
- description: Allows the reading of audience segments.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/audience-segments:read
- description: Allows the creation/updating/deletion of audience segments.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/audience-segments:write
- description: Allows the reading of contact groups.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/contact-groups:read
- description: Allows the creation/updating of contact groups.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/contact-groups:write
- description: Allows the reading of contact types.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/contact-types:read
- description: Allows the deletion of contacts.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/contacts:delete
- description: Allows the reading of contacts.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/contacts:read
- description: Allows the creation/updating of contacts.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/contacts:write
- description: Allows the creation/updating of sensitive data related to contacts.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/contacts:write-sensitive
- description: Allows the reading of custom fields
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/custom-fields:read
- description: Allows the writing of custom fields
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/custom-fields:write
- description: Allows the writing of discounts
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/discounts:write
- description: Allows the reading of donation items.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/donation-items:read
- description: Allows the reading of event discounts.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/event-discounts:read
- description: Allows the writing of event discounts.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/event-discounts:write
- description: Allows the reading of event email statuses.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/event-email-status:read
- description: Allows the reading of event emails
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/event-emails:read
- description: Allows to send event emails.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/event-emails:write
- description: Allows the reading of events-features
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/event-features:read
- description: Allows updating the event-features
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/event-features:write
- description: Allows the reading of user groups
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/event-user-groups:read
- description: Allows associating/disassociating user groups to event
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/event-user-groups:write
- description: Allows the reading of events
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/events:read
- description: Allows the creation/updating of events
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/events:write
- description: Allows the reading of fee items.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/fee-items:read
- description: Allow reading the hotel request or housing reservation request detail for attendees.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/hotel-request:read
- description: Allows the reading of the invitation lists for an event
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/invitation-lists:read
- description: Allows the reading of meeting request forms.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/meeting-request-forms:read
- description: Allows the reading of meeting requests.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/meeting-requests:read
- description: Allows the creation/updating of meeting requests.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/meeting-requests:write
- description: Allows reading of membership items.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/membership-items:read
- description: Allows the reading of orders
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/orders:read
- description: Allows the reading of event planning documents
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/planning-documents:read
- description: Allows the reading of players
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/players:read
- description: Allows the reading of process form submissions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/process-form-submissions:read
- description: Allows deletion of session program items
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/program-items:delete
- description: Allows reading of session program items
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/program-items:read
- description: Allows writing of session program items
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/program-items:write
- description: Allows the reading of quantity items.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/quantity-items:read
- description: Allows the writing of quantity items
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/quantity-items:write
- description: Allows the reading of registration paths
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/registration-paths:read
- description: Allows the reading of registration types
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/registration-types:read
- description: Allows the writing of registration types
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/registration-types:write
- description: Allows the reading of event role assignment.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/role-assignments:read
- description: Allows the reading of sessions attendance
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/session-attendance:read
- description: Allows the creation/updating of sessions attendance
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/session-attendance:write
- description: Allows reading of session categories
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/session-categories:read
- description: Allows writing of session categories
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/session-categories:write
- description: Allows the deletion of session registrations
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/session-enrollment:delete
- description: Allows the reading of sessions registrations
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/session-enrollment:read
- description: Allows the writing of sessions registrations
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/session-enrollment:write
- description: Allows reading of session segments
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/session-segments:read
- description: Allows the deletion of a session in an event
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/sessions:delete
- description: Allows the reading of sessions
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/sessions:read
- description: Allows the creation of a session in an event
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/sessions:write
- description: Allows reading of speaker categories
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/speaker-categories:read
- description: Allows writing of speaker categories
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/speaker-categories:write
- description: Allows the deletion of a speaker in an event
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/speakers:delete
- description: Allows the reading of speakers
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/speakers:read
- description: Allows the creation of a speaker in an event
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/speakers:write
- description: Allows the reading of taxes.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/taxes:read
- description: Allows the reading of transactions
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/transactions:read
- description: Allows the writing of transactions
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/transactions:write
- description: Allows reading of video views.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/video-views:read
- description: Allows the reading of video data.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/videos:read
- description: Allows the creation/updating of video data.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/videos:write
- description: Allows reading of event vouchers.
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/vouchers:read
- description: Allows the deletion of webcast
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/webcasts:delete
- description: Allows the reading of webcasts
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/webcasts:read
- description: Allows the creation of webcast
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/webcasts:write
- description: Allows the reading of event weblinks
  flows:
  - authorizationCode
  - clientCredentials
  scope: event/weblinks:read
- description: Allows the reading of Events+ hub data.
  flows:
  - authorizationCode
  - clientCredentials
  scope: events-plus/hubs:read
- description: Allows reading badges
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/badges:read
- description: Allows creating/updating badges
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/badges:write
- description: Allows deleting booth staff
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/booth-staff:delete
- description: Allows reading booth staff
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/booth-staff:read
- description: Allows creating booth staff
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/booth-staff:write
- description: Allows reading eliterature document request data
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/eliterature-requests:read
- description: Allows reading exhibitor admins
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitor-admins:read
- description: Allows creating/updating exhibitor admins
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitor-admins:write
- description: Allows reading exhibitor answers
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitor-answers:read
- description: Allows updating exhibitor answers
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitor-answers:write
- description: Allows deleting exhibitor categories
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitor-categories:delete
- description: Allows reading exhibitor categories
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitor-categories:read
- description: Allows creating/updating exhibitor categories
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitor-categories:write
- description: Allows deleting exhibitor content
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitor-contents:delete
- description: Allows reading exhibitor content
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitor-contents:read
- description: Allows creating/updating exhibitor content
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitor-contents:write
- description: Allows reading exhibitor questions
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitor-questions:read
- description: Allows deleting exhibitors
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitors:delete
- description: Allows reading exhibitors
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitors:read
- description: Allows creating/updating exhibitors
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/exhibitors:write
- description: Allows reading Lead Qualification Answers
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/lead-qualification-answers:read
- description: Allows reading Lead Qualification Questions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/lead-qualification-questions:read
- description: Allows reading leads.
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/leads:read
- description: Allows deleting registration pack
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/registration-packs:delete
- description: Allows reading registration pack
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/registration-packs:read
- description: Allows creating/updating registration pack
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/registration-packs:write
- description: Allows reading sponsorship level
  flows:
  - authorizationCode
  - clientCredentials
  scope: exhibitor/sponsorship-levels:read
- description: Allows the reading of file
  flows:
  - authorizationCode
  - clientCredentials
  scope: file/file:read
- description: Allows the uploading of file
  flows:
  - authorizationCode
  - clientCredentials
  scope: file/file:write
- description: Allows the user to connect to the Reglink APIs.
  flows:
  - clientCredentials
  scope: housing/connections:write
- description: Allows the user to create/update hotel room rates.
  flows:
  - clientCredentials
  scope: housing/hotel-room-rates:write
- description: Allows the user to read availability information for given event.
  flows:
  - clientCredentials
  scope: housing/housing-event-available-nights:read
- description: Allows the user to read information about event hotels.
  flows:
  - clientCredentials
  scope: housing/housing-event-hotels:read
- description: Allows the user to get information about housing event inventory.
  flows:
  - clientCredentials
  scope: housing/housing-event-inventory:read
- description: Allows the user to read information about event room types.
  flows:
  - clientCredentials
  scope: housing/housing-event-room-types:read
- description: Allows the user to read information about events.
  flows:
  - clientCredentials
  scope: housing/housing-events:read
- description: Allows the user to cancel reservation request.
  flows:
  - clientCredentials
  scope: housing/reservation-requests:delete
- description: Allows the user to read reservation request information.
  flows:
  - clientCredentials
  scope: housing/reservation-requests:read
- description: Allows the user to create/update reservation request.
  flows:
  - clientCredentials
  scope: housing/reservation-requests:write
- description: Allows the user to remove association from reservation.
  flows:
  - clientCredentials
  scope: housing/reservations-link:delete
- description: Allows the user to associate reservation to reservation request.
  flows:
  - clientCredentials
  scope: housing/reservations-link:write
- description: Allows the user to cancel reservation.
  flows:
  - clientCredentials
  scope: housing/reservations:delete
- description: Allows the user to read reservation details information.
  flows:
  - clientCredentials
  scope: housing/reservations:read
- description: Allows the user to create/update reservation.
  flows:
  - clientCredentials
  scope: housing/reservations:write
- description: Allows reading signatures.
  flows:
  - authorizationCode
  - clientCredentials
  scope: onsite/signatures:read
- description: Allows the creation/writing of proposal
  flows:
  - clientCredentials
  scope: proposal/proposals:write
- description: Allows reading print jobs.
  flows:
  - authorizationCode
  - clientCredentials
  scope: remote-printing/badge-print-jobs:read
- description: Allows creating print jobs.
  flows:
  - authorizationCode
  - clientCredentials
  scope: remote-printing/badge-print-jobs:write
- description: Allows reading pools.
  flows:
  - authorizationCode
  - clientCredentials
  scope: remote-printing/badge-printer-pools:read
- description: Allows the reading of RFP agenda items.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rfp/rfp-agenda-items:read
- description: Allows the reading of RFP attachments.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rfp/rfp-attachments:read
- description: Allows the reading of RFP custom fields.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rfp/rfp-custom-fields:read
- description: Allows the reading of RFP guest rooms.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rfp/rfp-guest-rooms:read
- description: Allows the reading of RFP internal documents.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rfp/rfp-internal-documents:read
- description: Allows the reading of RFP lead sources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rfp/rfp-lead-sources:read
- description: Allows the reading of past events similar to rfp event.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rfp/rfp-past-events:read
- description: Allows the reading of RFP questions.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rfp/rfp-questions:read
- description: Allows the reading of RFP recipients history.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rfp/rfp-recipients-history:read
- description: Allows the reading of RFP suppliers.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rfp/rfp-suppliers:read
- description: Allows the reading of basic details of RFP.
  flows:
  - authorizationCode
  - clientCredentials
  scope: rfp/rfps:read
- description: Allows to read attendee seat assignment information.
  flows:
  - authorizationCode
  - clientCredentials
  scope: seating/assignments:read
- description: Allows to read event seating.
  flows:
  - authorizationCode
  - clientCredentials
  scope: seating/event-seatings:read
- description: Allows to read seat information.
  flows:
  - authorizationCode
  - clientCredentials
  scope: seating/seats:read
- description: Allows to read table information.
  flows:
  - authorizationCode
  - clientCredentials
  scope: seating/tables:read
- description: Allows creation of credit card tokens
  flows:
  - clientCredentials
  scope: secure-ecommerce/card-tokens:write
- description: Allows the reading of survey questions
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/questions:read
- description: Allows reading the survey respondents
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/respondents:read
- description: Allows reading the survey responses
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/responses:read
- description: Allows reading the standalone survey email templates
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/standard-survey-email-templates:read
- description: Allows writing operations on standalone survey emails
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/standard-survey-email:write
- description: Allows the reading of standalone surveys questions
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/standard-survey-questions:read
- description: Allows reading the standalone survey respondents
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/standard-survey-respondents:read
- description: Allows write operations on standalone survey respondents
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/standard-survey-respondents:write
- description: Allows reading the standalone survey responses
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/standard-survey-responses:read
- description: Allows write operations on standalone surveys respondent's responses
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/standard-survey-responses:write
- description: Allows the reading of standalone surveys
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/standard-surveys:read
- description: Allows the reading of event survey questions
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/survey-questions:read
- description: Allows reading the event survey respondents
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/survey-respondents:read
- description: Allows write operations on the event survey respondents
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/survey-respondents:write
- description: Allows reading the event survey responses
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/survey-responses:read
- description: Allows write operations on the event surveys respondent's responses
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/survey-responses:write
- description: Allows the reading of event surveys
  flows:
  - authorizationCode
  - clientCredentials
  scope: survey/surveys:read
- description: Allows disassociating images from meeting rooms.
  flows:
  - authorizationCode
  - clientCredentials
  scope: venue/meeting-room-images:delete
- description: Allows retrieving meeting room images.
  flows:
  - authorizationCode
  - clientCredentials
  scope: venue/meeting-room-images:read
- description: Allows associating images with meeting rooms.
  flows:
  - authorizationCode
  - clientCredentials
  scope: venue/meeting-room-images:write
- description: Allows read access for overview of meeting room.
  flows:
  - authorizationCode
  - clientCredentials
  scope: venue/meeting-room-overviews:read
- description: Allows the creation and modification of meeting rooms.
  flows:
  - authorizationCode
  - clientCredentials
  scope: venue/meeting-rooms:write
- description: Allows read access for overview of venue details.
  flows:
  - authorizationCode
  - clientCredentials
  scope: venue/venue-details-overview:read
- description: Allows the creation and modification of venue details.
  flows:
  - authorizationCode
  - clientCredentials
  scope: venue/venue-details:write
- description: Allows the modification of venue facility information.
  flows:
  - authorizationCode
  - clientCredentials
  scope: venue/venue-facility:write
slug: cvent-hospitality-cloud-scopes
source_filename: cvent-hospitality-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\ndocs: https://developers.cvent.com/docs/rest-api/explanation/concepts\nnote: >-\n  238 OAuth 2.0 scopes read straight out of the securitySchemes block of the OpenAPI document Cvent\n  publishes at https://developers.cvent.com/documentation, each with Cvent's own description. The shape is\n  <domain>/<resource>:<read|write|delete>. The hospitality domains are housing/* (15 scopes),\n  rfp/* (11), venue/* (8), business-travel/* + business-transient/* (15) and proposal/*.\n  Cvent's Concepts page documents how scopes are attached to an application inside a workspace, and warns\n  that a token carrying roughly 50 or more scopes trips HTTP 431 — mint runtime tokens with only the\n  scopes a call needs.\nscope_domains_hospitality:\n  housing: 15\n  rfp: 11\n  venue: 8\n  business-travel: 5\n  business-transient: 10\n  proposal: 1\nsource: openapi/cvent-hospitality-cloud-authentication-openapi.yml, openapi/cvent-hospitality-cloud-event-travel-openapi.yml,\n\
  \  openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml, openapi/cvent-hospitality-cloud-housing-openapi.yml,\n  openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml, openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml,\n  openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml, openapi/cvent-hospitality-cloud-rfp-management-openapi.yml,\n  openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml, openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml,\n  openapi/cvent-hospitality-cloud-signatures-openapi.yml, openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml,\n  openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml, openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml,\n  openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml, openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\nschemes:\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.authorizationCode\n  source: openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Authorization Code Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.authorizationCode\n  source: openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description:\
  \ OAuth2 Authorization Code Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-housing-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.authorizationCode\n  source: openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n\
  \    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Authorization Code Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.authorizationCode\n  source: openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Authorization Code Flow.\n- name: OAuth2.clientCredentials\n  source:\
  \ openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.authorizationCode\n  source: openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Authorization Code Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.authorizationCode\n  source: openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n\
  \    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Authorization Code Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.authorizationCode\n  source: openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Authorization Code Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.authorizationCode\n  source: openapi/cvent-hospitality-cloud-signatures-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Authorization Code Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.authorizationCode\n  source: openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n\
  \  description: OAuth2 Authorization Code Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.authorizationCode\n  source: openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Authorization Code Flow.\n- name: OAuth2.clientCredentials\n  source: openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n \
  \ flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Client Credentials Flow.\n- name: OAuth2.authorizationCode\n  source: openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n  description: OAuth2 Authorization Code Flow.\nscopes:\n- scope: account/hooks:delete\n  description: Allows the deletion of hooks.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: account/hooks:read\n  description: Allows the reading of hooks.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: account/hooks:write\n  description: Allows the creation/updation of hooks.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: account/user-groups:delete\n\
  \  description: Allows deletion for user groups\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: account/user-groups:read\n  description: Allows the reading of user groups\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: account/user-groups:write\n  description: Allows the writing of user groups\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: account/users:delete\n  description: Allows the deletion of User\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: account/users:read\n  description: Allows the reading of User, User Group\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: account/users:write\n  description: Allows the creation/updating of User\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: appointments/appointment-attendees:read\n  description: Allows the reading of appointment attendees and their related entities.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: appointments/appointment-events:read\n\
  \  description: Allows the reading of appointment events and their related entities.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: appointments/appointment-types:read\n  description: Allows the reading of appointment types and their related entities.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: appointments/appointments:read\n  description: Allows the reading of appointment and their related entities.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: appointments/appointments:write\n  description: Allows the writing of appointments and their related entities.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: appointments/available-times:read\n  description: Allows the reading of availability times.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: appointments/locations:read\n  description: Allows the reading of appointment locations\
  \ and their related entities.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: attendee-insights/attendee-insights:read\n  description: Allows the reading of engagement scores (attendee insights).\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: attendee-insights/scores:read\n  description: Allows the reading of scores.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: attendee-insights/stats:read\n  description: Allows the reading of engagement score (attendee insight) stats.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-meeting-rooms-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-profiles-openapi.yml\n- scope: budget/budget-items:delete\n  description: Allows the deletion of budget items\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-authentication-openapi.yml\n  - openapi/cvent-hospitality-cloud-event-travel-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-hotels-openapi.yml\n  - openapi/cvent-hospitality-cloud-housing-openapi.yml\n  - openapi/cvent-hospitality-cloud-meeting-requests-openapi.yml\n\
  \  - openapi/cvent-hospitality-cloud-proposal-drafts-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-additional-details-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-management-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-requirements-openapi.yml\n  - openapi/cvent-hospitality-cloud-rfp-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-signatures-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-accounts-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-rfps-openapi.yml\n  - openapi/cvent-hospitality-cloud-travel-suppliers-openapi.yml\n  - openapi/cvent-hospitality-cloud-venue-mee\n\n# --- truncated at 32 KB (281 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/scopes/cvent-hospitality-cloud-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/scopes/cvent-hospitality-cloud-scopes.yml
summary_line: 238 scopes · clientCredentials/authorizationCode
tags:
- Catering
- Group Bookings
- Hospitality
- Hospitality Cloud
- Hotels
- Housing
- Authentication
- Passkey
- Reservations
- RFP
- Room Blocks
- Sales
- Sourcing
- Supplier Network
- Venues
token_urls:
- https://api-platform.cvent.com/ea/oauth2/token
---
