---
api_specs:
- filename: postman.yaml
  format: yaml
  label: MoMo All-in-One Payment Gateway (AIO v2)
  slug: aio-payment-gateway
  spec_type: Postman
  url: https://developers.momo.vn/v3/docs/payment/api/other/postman/
authorization_urls: []
description: ''
docs: https://developers.momo.vn/v3/docs/app-center/development-guideline/open-capabilities/permissions/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Momo Scopes
name_suffix: OAuth Scopes
note: 'MoMo''s Mini App Open Platform is described in its own documentation as "based on the industry standard OAuth2.0 authorization mechanism", but it does NOT publish RFC 6749 scope strings. What it publishes instead is a consent-role vocabulary: a Mini App calls MiniApi.requestUserConsents with an array of permission roles, MoMo renders a bottom sheet, and the user grants or denies each role individually. The resulting authCode/accessToken carries whatever the user granted. These roles are the closest thing MoMo has to scopes and are recorded here verbatim from the Consents Request page. The dedicated "Permissions" page on the same site is published but EMPTY — its entire body reads "( to be updated )" — so there is no authoritative permission reference beyond this list.'
overview: 'MoMo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MoMo
provider_slug: momo
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: momo-scopes
source_filename: momo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://developers.momo.vn/v3/docs/app-center/development-guideline/open-capabilities/consents-request/consentsRequest/\ndocs: https://developers.momo.vn/v3/docs/app-center/development-guideline/open-capabilities/permissions/\napi: momo:mini-app-open-api\nmodel: consent-roles\nnote: >-\n  MoMo's Mini App Open Platform is described in its own documentation as\n  \"based on the industry standard OAuth2.0 authorization mechanism\", but it does\n  NOT publish RFC 6749 scope strings. What it publishes instead is a consent-role\n  vocabulary: a Mini App calls MiniApi.requestUserConsents with an array of\n  permission roles, MoMo renders a bottom sheet, and the user grants or denies\n  each role individually. The resulting authCode/accessToken carries whatever the\n  user granted. These roles are the closest thing MoMo has to scopes and are\n  recorded here verbatim from the Consents Request page.\n  The dedicated \"Permissions\"\
  \ page on the same site is published but EMPTY — its\n  entire body reads \"( to be updated )\" — so there is no authoritative permission\n  reference beyond this list.\nscope_count: 6\nscopes:\n- name: phone\n  label: Phone Number\n  description: The end user's MoMo-registered phone number.\n- name: name\n  label: Full Name\n  description: The end user's full name.\n- name: email\n  label: Email Address\n  description: The end user's email address.\n- name: gender\n  label: User's Gender\n  description: The end user's gender.\n- name: dateOfBirth\n  label: User's date of birth\n  description: The end user's date of birth.\n- name: identity\n  label: User's MoMo KYC status\n  description: >-\n    The end user's KYC verification status (documented response values include\n    UNCONFIRM). Requested via the role key `identity`; MoMo's own example code\n    on the same page passes `identify`, an inconsistency in the published docs\n    that is recorded here rather than silently corrected.\n\
  request_shape:\n  function: MiniApi.requestUserConsents\n  parameter: 'permissions: Array<{ role: String, require?: boolean }>'\n  required_flag: >-\n    Setting require:true on a role prevents the user turning that role off in the\n    consent sheet — the Mini App can force a field to be all-or-nothing.\nresponse_shape:\n  since_platform: 3.1.10\n  fields:\n    data: The granted values, keyed by role\n    status: Per-role grant status (granted) or a top-level \"cancelled\"\n  note: >-\n    Before MoMo Platform 3.1.10 the granted values were returned flat and a\n    cancelled consent returned an empty object, indistinguishable from a denial.\n    The 3.1.10 change split data from status specifically to make cancel, deny and\n    accept distinguishable — MoMo documents the compatibility shim\n    (response?.name || response?.data?.name) in its own changelog.\nother_apis:\n  aio-payment-gateway: >-\n    No scopes. Authentication is a partnerCode/accessKey/secretKey triple with an\n    HMAC-SHA256\
  \ request signature; capability is governed by which payment\n    solutions the merchant is approved for in the M4B portal, not by a token scope.\n  business-page-openapi: >-\n    No scope strings, but a real permission-group model: the X-API-KEY is bound to\n    the groups granted in the MoMo for Business portal — page management and\n    setup, content (posts, ratings, reviews), messaging (templates, segmentation,\n    automated notifications), reporting and customer care.\n  voucher-distribution: >-\n    No scopes. clientId/clientSecret exchanged for a 24-hour bearer token with no\n    scope parameter documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/momo/refs/heads/main/scopes/momo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Payments
- Mobile Payments
- FinTech
- Digital Wallet
- Payment Gateway
- QR Payments
- Disbursement
- Buy Now Pay Later
- E-commerce
- Vietnam
token_urls: []
---
