---
api_specs:
- filename: fasten-health-bridge-api-openapi.yml
  format: yaml
  label: Fasten Health Bridge API
  slug: fasten-health-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fasten-health/refs/heads/main/openapi/fasten-health-bridge-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.connect.fastenhealth.com/identity-proofing/bring-your-own-identity
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fasten Health Scopes
name_suffix: OAuth Scopes
note: 'The Fasten Connect REST API itself is NOT OAuth-protected — it uses HTTP Basic auth with public/private key pairs, and derive-oauth-scopes.py correctly found zero oauth2 security schemes in the published OpenAPI. Two genuine OAuth scope surfaces exist alongside it, and both are documented rather than specified: the OAuth 2.0 Pushed Authorization Request flow on Fasten''s identity service, and the SMART on FHIR scopes that the patient''s own EHR grants and that Fasten reports back on connection events. Neither appears in any machine-readable artifact.'
overview: 'Fasten Health publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fasten Health API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fasten Health
provider_slug: fasten-health
schemes:
- applies_to: Bring Your Own Identity (BYOI) TEFCA IAS flow
  client_authentication: HTTP Basic with the Fasten public ID and private key
  endpoint: POST https://identity.fastenhealth.com/oauth2/par
  jwks: https://identity.fastenhealth.com/jwks.json
  name: Fasten Identity (Pushed Authorization Request)
  parameters:
  - name: scope
    note: Documented as a fixed value — must be exactly this.
    required: true
    value: openid profile email
  - name: response_type
    required: true
    value: code
  - name: prompt
    required: true
    value: consent
  - name: redirect_uri
    note: must exactly match a redirect URI registered for your Fasten client
    required: true
  - name: patient_id
    note: your stable
    opaque patient identifier: null
    required: true
  probe:
    checked: '2026-08-14'
    result: identity.fastenhealth.com does not resolve in public DNS (NXDOMAIN); no anonymous discovery document could be fetched from it. Scopes below are taken from the documentation, not from a live authorization-server metadata document.
  request_content_type: application/x-www-form-urlencoded
  response:
    fields:
      expires_in: 90
      request_uri: urn:ietf:params:oauth:request_uri:<uuid>
    note: The request_uri is single-use and expires after 90 seconds.
    status: 201
  source: docs
  standards:
  - RFC 9126 Pushed Authorization Requests
  - RFC 8693 Token Exchange
  - RFC 7523
  - OpenID Connect Core 1.0
  status: documented-host-unreachable
  type: oauth2
- applies_to: The downstream authorization between the patient and their healthcare provider's EHR, brokered by Fasten. Reported back to the integrator on the patient.connection_success webhook `scope` field.
  name: SMART on FHIR (granted by the patient's EHR)
  note: Only some EHRs report the granted scope; for those that do not, the field is omitted. In TEFCA mode the scope is always present and always `patient/*.read`.
  source: docs
  spec: https://hl7.org/fhir/smart-app-launch/scopes-and-launch-context.html
  type: oauth2
scope_count: 5
scope_names:
- openid
- profile
- email
- patient/*.read
- patient/Patient.read
scopes:
- description: Required OIDC scope for the Fasten Identity PAR request.
  flows: []
  scope: openid
- description: Required in the fixed `openid profile email` scope string for the PAR request.
  flows: []
  scope: profile
- description: Required in the fixed `openid profile email` scope string for the PAR request.
  flows: []
  scope: email
- description: SMART on FHIR patient-level read scope. Always granted in TEFCA mode; required for a successful EHI export.
  flows: []
  scope: patient/*.read
- description: SMART on FHIR demographics read scope. Named in the `scope_patient_missing` failure reason as an acceptable alternative to patient/*.read; its absence (patient unchecked "Demographics" during consent) causes EHI export to fail.
  flows: []
  scope: patient/Patient.read
slug: fasten-health-scopes
source_filename: fasten-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://docs.connect.fastenhealth.com/identity-proofing/bring-your-own-identity,\n  https://docs.connect.fastenhealth.com/webhooks/events\ndocs: https://docs.connect.fastenhealth.com/identity-proofing/bring-your-own-identity\nnote: >-\n  The Fasten Connect REST API itself is NOT OAuth-protected — it uses HTTP Basic auth with\n  public/private key pairs, and derive-oauth-scopes.py correctly found zero oauth2 security schemes\n  in the published OpenAPI. Two genuine OAuth scope surfaces exist alongside it, and both are\n  documented rather than specified: the OAuth 2.0 Pushed Authorization Request flow on Fasten's\n  identity service, and the SMART on FHIR scopes that the patient's own EHR grants and that Fasten\n  reports back on connection events. Neither appears in any machine-readable artifact.\nspec_derived: false\nspec_derived_note: >-\n  derive-oauth-scopes.py over openapi/fasten-health-connect-openapi-original.yml\
  \ returned\n  \"providers with oauth2: 0\" — there is no oauth2 securityScheme to derive from.\n\nschemes:\n  - name: Fasten Identity (Pushed Authorization Request)\n    type: oauth2\n    source: docs\n    status: documented-host-unreachable\n    endpoint: POST https://identity.fastenhealth.com/oauth2/par\n    client_authentication: HTTP Basic with the Fasten public ID and private key\n    request_content_type: application/x-www-form-urlencoded\n    applies_to: Bring Your Own Identity (BYOI) TEFCA IAS flow\n    standards: [RFC 9126 Pushed Authorization Requests, RFC 8693 Token Exchange, RFC 7523, OpenID Connect Core 1.0]\n    parameters:\n      - {name: scope, required: true, value: \"openid profile email\", note: \"Documented as a fixed value — must be exactly this.\"}\n      - {name: response_type, required: true, value: code}\n      - {name: prompt, required: true, value: consent}\n      - {name: redirect_uri, required: true, note: must exactly match a redirect URI registered for your\
  \ Fasten client}\n      - {name: patient_id, required: true, note: your stable, opaque patient identifier}\n    response:\n      status: 201\n      fields: {request_uri: \"urn:ietf:params:oauth:request_uri:<uuid>\", expires_in: 90}\n      note: The request_uri is single-use and expires after 90 seconds.\n    jwks: https://identity.fastenhealth.com/jwks.json\n    probe:\n      checked: '2026-08-14'\n      result: >-\n        identity.fastenhealth.com does not resolve in public DNS (NXDOMAIN); no anonymous discovery\n        document could be fetched from it. Scopes below are taken from the documentation, not from\n        a live authorization-server metadata document.\n\n  - name: SMART on FHIR (granted by the patient's EHR)\n    type: oauth2\n    source: docs\n    applies_to: >-\n      The downstream authorization between the patient and their healthcare provider's EHR, brokered\n      by Fasten. Reported back to the integrator on the patient.connection_success webhook `scope`\n      field.\n\
  \    spec: https://hl7.org/fhir/smart-app-launch/scopes-and-launch-context.html\n    note: >-\n      Only some EHRs report the granted scope; for those that do not, the field is omitted. In TEFCA\n      mode the scope is always present and always `patient/*.read`.\n\nscopes:\n  - scope: openid\n    description: Required OIDC scope for the Fasten Identity PAR request.\n    scheme: Fasten Identity (Pushed Authorization Request)\n    required: true\n    sources: [https://docs.connect.fastenhealth.com/identity-proofing/bring-your-own-identity]\n  - scope: profile\n    description: Required in the fixed `openid profile email` scope string for the PAR request.\n    scheme: Fasten Identity (Pushed Authorization Request)\n    required: true\n    sources: [https://docs.connect.fastenhealth.com/identity-proofing/bring-your-own-identity]\n  - scope: email\n    description: Required in the fixed `openid profile email` scope string for the PAR request.\n    scheme: Fasten Identity (Pushed Authorization\
  \ Request)\n    required: true\n    sources: [https://docs.connect.fastenhealth.com/identity-proofing/bring-your-own-identity]\n  - scope: patient/*.read\n    description: >-\n      SMART on FHIR patient-level read scope. Always granted in TEFCA mode; required for a\n      successful EHI export.\n    scheme: SMART on FHIR (granted by the patient's EHR)\n    sources: [https://docs.connect.fastenhealth.com/webhooks/events]\n  - scope: patient/Patient.read\n    description: >-\n      SMART on FHIR demographics read scope. Named in the `scope_patient_missing` failure reason as\n      an acceptable alternative to patient/*.read; its absence (patient unchecked \"Demographics\"\n      during consent) causes EHI export to fail.\n    scheme: SMART on FHIR (granted by the patient's EHR)\n    sources: [https://docs.connect.fastenhealth.com/webhooks/events]\n\ngaps:\n  - No OAuth authorization-server metadata document is reachable (identity host does not resolve).\n  - No scopes or permissions reference\
  \ page exists; scopes are scattered across guides.\n  - The Fasten Connect REST API has no per-scope authorization model — a private key is all-or-nothing.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fasten-health/refs/heads/main/scopes/fasten-health-scopes.yml
summary_line: 5 scopes
tags:
- Healthcare
- FHIR
- Personal Health Record
- Electronic Medical Record
- Health Data Interoperability
- TEFCA
- EHI Export
- Patient Consent
- Self-Hosted
- Open-Source
- HL7
- Healthcare Connectivity
token_urls: []
---
