---
authorization_urls:
- https://auth.ambiencehealthcare.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Ambience Healthcare Scopes
name_suffix: OAuth Scopes
note: Scopes are taken verbatim from the `scopes_supported` array of the provider's live OpenID Connect discovery document. These are the standard OIDC scopes and claim-scopes the Ambience identity tenant advertises anonymously; Ambience publishes no product or resource scope reference (the Integration API is access-gated), so no application-level scopes such as read:encounters or write:notes are recorded here. Absence is the honest result, not an omission.
overview: 'Ambience Healthcare publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ambience Healthcare API on a user''s behalf.


  Tokens are issued from https://auth.ambiencehealthcare.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ambience Healthcare
provider_slug: ambience-healthcare
schemes:
- flows:
  - authorizationUrl: https://auth.ambiencehealthcare.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token
  - deviceAuthorizationUrl: https://auth.ambiencehealthcare.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token
  issuer: https://auth.ambiencehealthcare.com/
  name: OpenIDConnect
  source: well-known/ambience-healthcare-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- name
- given_name
- family_name
- nickname
- email
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Request an OpenID Connect ID token for the authenticating subject.
  flows: []
  scope: openid
- description: Basic profile claims for the authenticating subject.
  flows: []
  scope: profile
- description: Issue a refresh token so the client can obtain new access tokens without user interaction.
  flows: []
  scope: offline_access
- description: The subject's full name claim.
  flows: []
  scope: name
- description: The subject's given name claim.
  flows: []
  scope: given_name
- description: The subject's family name claim.
  flows: []
  scope: family_name
- description: The subject's nickname claim.
  flows: []
  scope: nickname
- description: The subject's email address claim.
  flows: []
  scope: email
- description: Whether the subject's email address has been verified.
  flows: []
  scope: email_verified
- description: The subject's profile picture URL claim.
  flows: []
  scope: picture
- description: The timestamp the subject's identity record was created.
  flows: []
  scope: created_at
- description: The linked identity providers associated with the subject.
  flows: []
  scope: identities
- description: The subject's phone number claim.
  flows: []
  scope: phone
- description: The subject's address claim.
  flows: []
  scope: address
slug: ambience-healthcare-scopes
source_filename: ambience-healthcare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://auth.ambiencehealthcare.com/.well-known/openid-configuration\ndocs: null\nnote: 'Scopes are taken verbatim from the `scopes_supported` array of the provider''s\n  live OpenID Connect discovery document. These are the standard OIDC scopes and claim-scopes\n  the Ambience identity tenant advertises anonymously; Ambience publishes no product\n  or resource scope reference (the Integration API is access-gated), so no application-level\n  scopes such as read:encounters or write:notes are recorded here. Absence is the honest\n  result, not an omission.'\nschemes:\n- name: OpenIDConnect\n  source: well-known/ambience-healthcare-openid-configuration.json\n  issuer: https://auth.ambiencehealthcare.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.ambiencehealthcare.com/authorize\n    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token\n\
  \  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.ambiencehealthcare.com/oauth/device/code\n    tokenUrl: https://auth.ambiencehealthcare.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an OpenID Connect ID token for the authenticating subject.\n  kind: protocol\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims for the authenticating subject.\n  kind: profile\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can obtain new access tokens without\n    user interaction.\n  kind: protocol\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: name\n  description: The subject's full name claim.\n  kind: profile\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: given_name\n  description: The subject's given name claim.\n  kind: profile\n\
  \  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: family_name\n  description: The subject's family name claim.\n  kind: profile\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: nickname\n  description: The subject's nickname claim.\n  kind: profile\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: email\n  description: The subject's email address claim.\n  kind: profile\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: email_verified\n  description: Whether the subject's email address has been verified.\n  kind: profile\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: picture\n  description: The subject's profile picture URL claim.\n  kind: profile\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: created_at\n  description: The timestamp the subject's identity record was created.\n  kind: profile\n  sources:\
  \ [well-known/ambience-healthcare-openid-configuration.json]\n- scope: identities\n  description: The linked identity providers associated with the subject.\n  kind: profile\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: phone\n  description: The subject's phone number claim.\n  kind: profile\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\n- scope: address\n  description: The subject's address claim.\n  kind: profile\n  sources: [well-known/ambience-healthcare-openid-configuration.json]\ncoverage:\n  scopes_total: 14\n  product_scopes: 0\n  protocol_or_profile_scopes: 14\nx-evidence:\n  fetched: '2026-07-31'\n  url: https://auth.ambiencehealthcare.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambience-healthcare/refs/heads/main/scopes/ambience-healthcare-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Healthcare
- Artificial Intelligence
- Clinical Documentation
- Ambient AI
- Medical Coding
- Electronic Health Records
- FHIR
- Health IT
- Speech Recognition
token_urls:
- https://auth.ambiencehealthcare.com/oauth/token
---
