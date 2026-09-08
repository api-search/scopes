---
api_specs:
- filename: cms-energy-authorizations-api-openapi.yml
  format: yaml
  label: CMS Energy Authorizations API
  slug: cms-energy-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-authorizations-api-openapi.yml
- filename: cms-energy-bills-api-openapi.yml
  format: yaml
  label: CMS Energy Bills API
  slug: cms-energy-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-bills-api-openapi.yml
- filename: cms-energy-greenbutton-api-openapi.yml
  format: yaml
  label: CMS Energy GreenButton API
  slug: cms-energy-greenbutton-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-greenbutton-api-openapi.yml
- filename: cms-energy-intervals-api-openapi.yml
  format: yaml
  label: CMS Energy Intervals API
  slug: cms-energy-intervals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-intervals-api-openapi.yml
- filename: cms-energy-meters-api-openapi.yml
  format: yaml
  label: CMS Energy Meters API
  slug: cms-energy-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-meters-api-openapi.yml
- filename: cms-energy-outage-map-api-openapi.yml
  format: yaml
  label: Consumers Energy Outage Map ArcGIS REST API
  slug: cms-energy-outage-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/openapi/cms-energy-outage-map-api-openapi.yml
authorization_urls: []
description: Authorization scope reference for the Consumers Energy Green Button Connect My Data program. Green Button does not use OAuth scope as a flat list of strings — the scope value is a semicolon-separated parameter string whose required `FB` member is an underscore-joined list of ESPI Function Blocks. Recorded here as the provider documents it, not flattened into pseudo-scopes.
docs: https://utilityapi.com/docs/greenbutton/scope
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cms Energy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CMS Energy publishes 10 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CMS Energy API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CMS Energy
provider_slug: cms-energy
schemes: []
scope_count: 10
scope_names:
- FB=4
- FB=16
- FB=39
- FB=51
- HistoryLength
- PreferredAuthEndDate
- SubscriptionFrequency
- AdditionalScope
- AdditionalScope=auth-sso
- AdditionalScope=auth-test-{scenario}
scopes:
- description: Access to the customer's anonymous interval usage data.
  flows: []
  scope: FB=4
- description: Access to the customer's bill data.
  flows: []
  scope: FB=16
- description: Push notifications of new data to a configured notify_url. Frequency is set with SubscriptionFrequency.
  flows: []
  scope: FB=39
- description: Access to account details — account number, service address and similar.
  flows: []
  scope: FB=51
- description: Seconds of history requested. 0 requests no history.
  flows: []
  scope: HistoryLength
- description: Unix timestamp at which the authorization auto-revokes. 0 means run until the customer revokes.
  flows: []
  scope: PreferredAuthEndDate
- description: How often bulk-download notifications are sent when FB 39 is in scope. Integer days or a named frequency.
  flows: []
  scope: SubscriptionFrequency
- description: Underscore-joined list of universal and utility-specific options.
  flows: []
  scope: AdditionalScope
- description: Authenticate the customer through Consumers Energy SSO (described in the docs as OpenIDConnect). This is the default for CONSUMERSENERGY.
  flows: []
  scope: AdditionalScope=auth-sso
- description: Bypass Consumers Energy SSO and authenticate as a published test scenario — test_residential, test_commercial or test_empty.
  flows: []
  scope: AdditionalScope=auth-test-{scenario}
slug: cms-energy-scopes
source_filename: cms-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://utilityapi.com/docs/greenbutton/scope\ndocs: https://utilityapi.com/docs/greenbutton/scope\ndescription: >-\n  Authorization scope reference for the Consumers Energy Green Button Connect My Data program.\n  Green Button does not use OAuth scope as a flat list of strings — the scope value is a\n  semicolon-separated parameter string whose required `FB` member is an underscore-joined list of\n  ESPI Function Blocks. Recorded here as the provider documents it, not flattened into\n  pseudo-scopes.\nsupersedes: >-\n  The prior derived artifact carried a single scope, `auth-sso`, read from the OpenAPI in this\n  repo. That is an authentication OPTION, not a data scope; it is retained below under\n  additional_scope.\noauth:\n  flows:\n    - flow: authorizationCode\n      grant_type: authorization_code\n      authorization_endpoint_pattern: https://utilityapi.com/DataCustodian/{utility}/oauth/authorize\n      token_endpoint_pattern:\
  \ https://utilityapi.com/DataCustodian/{utility}/oauth/token\n      note: >-\n        The exact authorize and token URLs for CONSUMERSENERGY are issued per third party and are\n        shown in the third party's own settings after Consumers Energy approves the registration.\n        They are therefore not publicly enumerable. The `demo` utility variant is the documented\n        example (https://utilityapi.com/DataCustodian/demo/oauth/authorize, probed 401 — exists,\n        gated).\n      token_auth: HTTP Basic with client_id and client_secret\n      token_response: [token_type, access_token, refresh_token, expires_in, scope, resourceURI, customerResourceURI, authorizationURI]\n      access_token_lifetime_seconds: 3600\n    - flow: refreshToken\n      grant_type: refresh_token\n      note: Same token endpoint; POST grant_type=refresh_token with the stored refresh_token.\n    - flow: clientCredentials\n      grant_type: client_credentials\n      note: Issues the client_access_token used\
  \ for Green Button Authorization and Bulk endpoints.\n      source: https://utilityapi.com/docs/greenbutton/api\n  probed:\n    - url: https://utilityapi.com/authorize\n      status: 200\n      note: The customer-facing \"Authorize Access to Utility Data\" page. Live.\n    - url: https://utilityapi.com/api/v2/oauth/token\n      status: 404\n      note: >-\n        DEFECT FOUND. This tokenUrl is carried in the OpenAPI securitySchemes in this repo and\n        does not exist — it returns the platform's own not_found envelope. It was authored into\n        the scaffolded spec, not harvested. The real token endpoint is the per-utility\n        DataCustodian path above. Recorded rather than silently corrected, because the spec's\n        securityScheme is what downstream artifacts were derived from.\n    - url: https://utilityapi.com/DataCustodian/espi/1_1/resource/ReadServiceStatus\n      status: 401\n      note: Live and auth-gated, confirming the ESPI resource tree is real.\nscope_string:\n\
  \  grammar: 'FB=<FUNCTION_BLOCK_LIST>;<OPTION_NAME>=<OPTION_VALUE>;...'\n  separator: ';'\n  fb_separator: '_'\n  required: [FB]\n  example_request: FB=4_16_51;HistoryLength=34128000\n  example_final: FB=1_3_4_5_8_13_14_18_19_34_35_39_51;IntervalDuration=900_3600;BlockDuration=daily;HistoryLength=34128000;SubscriptionFrequency=daily;AccountCollection=2\n  warning: >-\n    The scope in the authorization URL only PREFILLS the consent form. The customer can edit it,\n    and the platform may add parameters. Always read the final `scope` returned with the access\n    token — it is authoritative, and it may be narrower than what was asked for.\nscopes:\n  - scope: FB=4\n    name: Interval Metering\n    description: Access to the customer's anonymous interval usage data.\n    type: function-block\n    requestable: true\n  - scope: FB=16\n    name: Usage Summary with Costs\n    description: Access to the customer's bill data.\n    type: function-block\n    requestable: true\n  - scope: FB=39\n\
  \    name: PUSH Model\n    description: >-\n      Push notifications of new data to a configured notify_url. Frequency is set with\n      SubscriptionFrequency.\n    type: function-block\n    requestable: true\n  - scope: FB=51\n    name: Core Retail Customer\n    description: Access to account details — account number, service address and similar.\n    type: function-block\n    requestable: true\n  - scope: HistoryLength\n    name: Historical window\n    description: Seconds of history requested. 0 requests no history.\n    type: option\n    default: 63072000\n    default_human: 2 years\n    requestable: true\n  - scope: PreferredAuthEndDate\n    name: Automatic revocation date\n    description: Unix timestamp at which the authorization auto-revokes. 0 means run until the customer revokes.\n    type: option\n    default: three years from the time of authorization\n    requestable: true\n  - scope: SubscriptionFrequency\n    name: Notification frequency\n    description: How often bulk-download\
  \ notifications are sent when FB 39 is in scope. Integer days or a named frequency.\n    type: option\n    default: billingPeriod\n    requestable: true\n  - scope: AdditionalScope\n    name: Additional scope options\n    description: Underscore-joined list of universal and utility-specific options.\n    type: option\n    default: ''\n    requestable: true\n  - scope: AdditionalScope=auth-sso\n    name: Consumers Energy single sign-on\n    description: >-\n      Authenticate the customer through Consumers Energy SSO (described in the docs as\n      OpenIDConnect). This is the default for CONSUMERSENERGY.\n    type: additional-scope\n    utility_specific: true\n    source: https://utilityapi.com/docs/utilities/consumersenergy\n  - scope: AdditionalScope=auth-test-{scenario}\n    name: Test-account authentication\n    description: >-\n      Bypass Consumers Energy SSO and authenticate as a published test scenario —\n      test_residential, test_commercial or test_empty.\n    type: additional-scope\n\
  \    utility_specific: true\n    source: https://utilityapi.com/docs/utilities/consumersenergy\ninformational_only:\n  note: Returned in the final scope string; cannot be requested in the authorization URL.\n  parameters:\n  - name: AccountCollection\n    description: How many UsagePoints the authorization covers.\n  - name: BR\n    description: The Bulk ID for the Bulk API.\n  - name: IntervalDuration\n    description: Interval length in seconds (900 = 15 minutes).\n  - name: BlockDuration\n    description: Interval chunk size in seconds, or a named frequency.\nfunction_block_reference:\n  note: >-\n    Only 4, 16, 39 and 51 are honoured in an authorization URL. The full ESPI table is returned in\n    the final scope string.\n  blocks:\n    1: Common\n    2: Download My Data\n    3: Connect My Data\n    4: Interval Metering\n    5: Interval Electricity Metering\n    6: Demand Electricity Metering\n    7: Net Metering\n    8: Forward and Reverse Metering\n    9: Register Values\n    10:\
  \ Gas\n    11: Water\n    12: Cost of Interval Data\n    13: Security and Privacy Classes\n    14: Authorization and Authentication (replaced by FB 31)\n    15: Usage Summary\n    16: Usage Summary with Cost\n    17: Power Quality Summary\n    39: PUSH Model\n    51: Core Retail Customer\ntoken_classes:\n  source: https://utilityapi.com/docs/greenbutton/api\n  classes:\n  - name: registration_access_token\n    grants: Registration endpoints (third-party ApplicationInformation)\n    lifetime: Does not expire unless rotated\n  - name: client_access_token\n    grants: Authorization endpoints and Bulk endpoints\n    issued_by: grant_type=client_credentials\n  - name: access_token\n    grants: Resource endpoints and Batch endpoints, scoped to one authorization\n    issued_by: grant_type=authorization_code\n    lifetime_seconds: 3600\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/scopes/cms-energy-scopes.yml
summary_line: 10 scopes
tags:
- Electric
- Energy
- Green Button
- Michigan
- Natural Gas
- Utility
- Fortune 500
token_urls: []
---
