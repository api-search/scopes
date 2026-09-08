---
api_specs:
- filename: znanylekarz-integrations-api.yml
  format: yaml
  label: Docplanner Integrations API
  slug: docplanner-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-integrations-api.yml
authorization_urls: []
description: ''
docs: https://integrations.docplanner.com/guide/fundamentals/authorization.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Znanylekarz Scopes
name_suffix: OAuth Scopes
note: 'The OAuth surface is deliberately flat: ONE scope, `integration`, requested at token exchange, granting the whole API. There is no read/write split, no per-resource scope and no least-privilege story — a token that can read a doctor''s calendar can also cancel their patients'' appointments. Authorization is instead enforced out-of-band, by which facilities the API client is provisioned for (403 outside that estate). Searched the docs for a scope or permissions reference page; none exists beyond the single scope named in the token example.'
overview: 'ZnanyLekarz publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ZnanyLekarz API on a user''s behalf.


  Tokens are issued from https://www.{domain}/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ZnanyLekarz
provider_slug: znanylekarz
schemes:
- description: "The API utilizes the industry-standard [OAuth 2.0](https://tools.ietf.org/html/rfc6749) protocol.\n\nAll requests to our API must be authenticated and must include a valid access token.\n\n`NOTE! Our SSO Api version is v2 while our Integration Api version is v3`\n\nYou can get a token for testing purposes with cURL\n\n```\ncurl -u {client_id}:{client_secret} https://www.{domain}/oauth/v2/token -d 'grant_type=client_credentials&scope=integration'\n```\n\nA response example you can expect\n\n```\n{\n    \"access_token\": \"03807cb390319329bdf6c777d4dfae9c0d3b3c35\",\n    \"expires_in\": 3600,\n    \"token_type\": \"bearer\",\n    \"scope\": null\n}\n```\n\nAnd then with every request in the `request header` you should add your bearer token like so:\n\n```\nAuthorization: Bearer {access_token}\n```"
  flows:
  - flow: clientCredentials
    tokenUrl: https://www.{domain}/oauth/v2/token
  name: oauth2
  source: openapi/znanylekarz-integrations-api.yml
scope_count: 1
scope_names:
- integration
scopes:
- description: API integration
  flows:
  - clientCredentials
  scope: integration
slug: znanylekarz-scopes
source_filename: znanylekarz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://integrations.docplanner.com/guide/fundamentals/authorization.html\nschemes:\n- name: oauth2\n  source: openapi/znanylekarz-integrations-api.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.{domain}/oauth/v2/token\n  description: \"The API utilizes the industry-standard [OAuth 2.0](https://tools.ietf.org/html/rfc6749)\\\n    \\ protocol.\\n\\nAll requests to our API must be authenticated and must include a valid access token.\\n\\\n    \\n`NOTE! Our SSO Api version is v2 while our Integration Api version is v3`\\n\\nYou can get a token\\\n    \\ for testing purposes with cURL\\n\\n```\\ncurl -u {client_id}:{client_secret} https://www.{domain}/oauth/v2/token\\\n    \\ -d 'grant_type=client_credentials&scope=integration'\\n```\\n\\nA response example you can expect\\n\\\n    \\n```\\n{\\n    \\\"access_token\\\": \\\"03807cb390319329bdf6c777d4dfae9c0d3b3c35\\\",\\n    \\\"expires_in\\\"\\\n    : 3600,\\\
  n    \\\"token_type\\\": \\\"bearer\\\",\\n    \\\"scope\\\": null\\n}\\n```\\n\\nAnd then with every request\\\n    \\ in the `request header` you should add your bearer token like so:\\n\\n```\\nAuthorization: Bearer\\\n    \\ {access_token}\\n```\"\nscopes:\n- scope: integration\n  description: API integration\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/znanylekarz-integrations-api.yml\ndocs: https://integrations.docplanner.com/guide/fundamentals/authorization.html\nderived_from: openapi/znanylekarz-integrations-api.yml\nnote: 'The OAuth surface is deliberately flat: ONE scope, `integration`, requested at token exchange,\n  granting the whole API. There is no read/write split, no per-resource scope and no least-privilege story\n  — a token that can read a doctor''s calendar can also cancel their patients'' appointments. Authorization\n  is instead enforced out-of-band, by which facilities the API client is provisioned for (403 outside\n  that estate). Searched the docs\
  \ for a scope or permissions reference page; none exists beyond the single\n  scope named in the token example.'\nscope_count: 1\ngranularity: all-or-nothing\nleast_privilege_supported: false\nauthorization_model: Estate-based rather than scope-based. Each API client is provisioned against specific\n  facilities; operations on a facility, doctor or address outside that estate return 403.\nresponse_extensions_are_not_scopes:\n  note: The `with` query parameter values in this API are named like scopes — booking.patient, doctor.addresses,\n    address_service.public_insurance_flow — and the OpenAPI even calls their enum schemas *Scopes. They\n    are NOT OAuth scopes. They widen the response payload; they do not grant permission, and they are\n    not presented at the token endpoint. Recorded here so the naming does not later get mistaken for a\n    scope catalog.\n  documented_in: conventions/znanylekarz-conventions.yml (field_expansion)\n  docs: https://integrations.docplanner.com/guide/fundamentals/extensions.html\n\
  \  values:\n  - facility.doctors\n  - doctor.profile_url\n  - doctor.specializations\n  - doctor.addresses\n  - doctor.license_numbers\n  - address.booking_extra_fields\n  - address.online_only\n  - address.visit_payment\n  - address.commercial_type\n  - address.insurance_support\n  - address_service.allowed_patients\n  - address_service.custom_name\n  - address_service.public_insurance_flow\n  - booking.patient\n  - booking.address_service\n  - booking.presence\n  - booking.moving\n  - services.only_diagnostics\n  - slot.services\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/scopes/znanylekarz-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Healthcare
- Health Tech
- Appointments
- Booking
- Medical
- Marketplace
- Doctors
- Scheduling
- Poland
- Practice Management
- Telemedicine
token_urls:
- https://www.{domain}/oauth/v2/token
---
