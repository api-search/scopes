---
api_specs:
- filename: textmaster-abilities-api-openapi.yml
  format: yaml
  label: TextMaster Abilities API
  slug: textmaster-abilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-abilities-api-openapi.yml
- filename: textmaster-api-templates-api-openapi.yml
  format: yaml
  label: TextMaster API Templates API
  slug: textmaster-api-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-api-templates-api-openapi.yml
- filename: textmaster-authors-api-openapi.yml
  format: yaml
  label: TextMaster Authors API
  slug: textmaster-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-authors-api-openapi.yml
- filename: textmaster-categories-api-openapi.yml
  format: yaml
  label: TextMaster Categories API
  slug: textmaster-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-categories-api-openapi.yml
- filename: textmaster-countries-api-openapi.yml
  format: yaml
  label: TextMaster Countries API
  slug: textmaster-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-countries-api-openapi.yml
- filename: textmaster-documents-api-openapi.yml
  format: yaml
  label: TextMaster Documents API
  slug: textmaster-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-documents-api-openapi.yml
- filename: textmaster-expertises-api-openapi.yml
  format: yaml
  label: TextMaster Expertises API
  slug: textmaster-expertises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-expertises-api-openapi.yml
- filename: textmaster-glossaries-api-openapi.yml
  format: yaml
  label: TextMaster Glossaries API
  slug: textmaster-glossaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-glossaries-api-openapi.yml
- filename: textmaster-invoices-api-openapi.yml
  format: yaml
  label: TextMaster Invoices API
  slug: textmaster-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-invoices-api-openapi.yml
- filename: textmaster-languages-api-openapi.yml
  format: yaml
  label: TextMaster Languages API
  slug: textmaster-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-languages-api-openapi.yml
- filename: textmaster-locales-api-openapi.yml
  format: yaml
  label: TextMaster Locales API
  slug: textmaster-locales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-locales-api-openapi.yml
- filename: textmaster-my-authors-api-openapi.yml
  format: yaml
  label: TextMaster My Authors API
  slug: textmaster-my-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-my-authors-api-openapi.yml
- filename: textmaster-negotiated-contracts-api-openapi.yml
  format: yaml
  label: TextMaster Negotiated Contracts API
  slug: textmaster-negotiated-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-negotiated-contracts-api-openapi.yml
- filename: textmaster-projects-api-openapi.yml
  format: yaml
  label: TextMaster Projects API
  slug: textmaster-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-projects-api-openapi.yml
- filename: textmaster-receipts-api-openapi.yml
  format: yaml
  label: TextMaster Receipts API
  slug: textmaster-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-receipts-api-openapi.yml
- filename: textmaster-support-messages-api-openapi.yml
  format: yaml
  label: TextMaster Support Messages API
  slug: textmaster-support-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-support-messages-api-openapi.yml
- filename: textmaster-transactions-api-openapi.yml
  format: yaml
  label: TextMaster Transactions API
  slug: textmaster-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-transactions-api-openapi.yml
- filename: textmaster-uploadproperties-api-openapi.yml
  format: yaml
  label: TextMaster Upload Properties API
  slug: textmaster-uploadproperties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-uploadproperties-api-openapi.yml
- filename: textmaster-users-api-openapi.yml
  format: yaml
  label: TextMaster Users API
  slug: textmaster-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-users-api-openapi.yml
- filename: textmaster-work-templates-api-openapi.yml
  format: yaml
  label: TextMaster Work Templates API
  slug: textmaster-work-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/openapi/textmaster-work-templates-api-openapi.yml
authorization_urls:
- https://api.textmaster.com/oauth/authorize
description: ''
docs: https://developer.textmaster.com/apps/building-oauth-apps/scopes-for-oauth-apps
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Textmaster Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TextMaster publishes 22 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TextMaster API on a user''s behalf.


  Tokens are issued from https://api.textmaster.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TextMaster
provider_slug: textmaster
schemes:
- description: OAuth2 Bearer token authentication
  flows:
  - authorizationUrl: https://api.textmaster.com/oauth/authorize
    authorizationUrl_docs: https://app.textmaster.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://api.textmaster.com/oauth/token
    tokenUrl: https://api.textmaster.com/oauth/token
  name: oauth2
  scope_delimiter: space (URL-encoded as %20 in the authorize redirect)
  source: openapi/textmaster-api-v1-openapi.yml
scope_count: 22
scope_names:
- public
- user:manage
- user:read
- user:write
- user:email
- glossary:manage
- glossary:read
- glossary:write
- project:manage
- project:read
- project:write
- project:launch
- project:quote
- discussion:manage
- discussion:read
- discussion:write
- transaction:read
- transaction:manage
- transaction:write
- preferred_author:manage
- preferred_author:read
- preferred_author:write
scopes:
- description: Grants read-only access to public information (such as, but not limited to, available languages, options, pricing, expertises). This is the default scope if none is provided.
  flows: []
  scope: public
- description: Grants full access to user's profile info only (includes `user:email`).
  flows: []
  scope: user:manage
- description: Grants read-only access to user's profile info.
  flows: []
  scope: user:read
- description: Grants read/write access to user's profile info.
  flows: []
  scope: user:write
- description: Grants read-only access to user's private email address.
  flows: []
  scope: user:email
- description: Grants full access to glossaries (includes the ones shared from organization).
  flows: []
  scope: glossary:manage
- description: Grants read-only access to glossaries (includes the ones shared from organization).
  flows: []
  scope: glossary:read
- description: Grants read/write access to glossaries (includes the ones shared from organization).
  flows: []
  scope: glossary:write
- description: Grants full access to projects, documents and templates (includes `project:launch` and `project:quote`).
  flows: []
  scope: project:manage
- description: Grants read-only access to projects, documents and templates.
  flows: []
  scope: project:read
- description: Grants read/write access to projects, documents and templates.
  flows: []
  scope: project:write
- description: Grants access to launch projects and debit the client's account.
  flows: []
  scope: project:launch
- description: Grants access to request project quotations.
  flows: []
  scope: project:quote
- description: Grants full access to team discussions.
  flows: []
  scope: discussion:manage
- description: Grants read-only access to team discussions.
  flows: []
  scope: discussion:read
- description: Grants read/write access to team discussions.
  flows: []
  scope: discussion:write
- description: Grants read-only access to financial transactions.
  flows: []
  scope: transaction:read
- description: Full access to financial transactions. Referenced by the transactions, invoices and receipts operations and requested by TextMaster's own Postman collection, but ABSENT from the published scopes table.
  flows: []
  scope: transaction:manage
- description: Write access to financial transactions. Referenced by operation `security[]` and the Postman collection, but ABSENT from the published scopes table.
  flows: []
  scope: transaction:write
- description: Grants full access to client's preferred authors.
  flows:
  - authorizationCode
  scope: preferred_author:manage
- description: Grants read-only access to client's preferred authors.
  flows:
  - authorizationCode
  scope: preferred_author:read
- description: Grants write access to client's preferred authors.
  flows:
  - authorizationCode
  scope: preferred_author:write
slug: textmaster-scopes
source_filename: textmaster-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/textmaster-api-v1-openapi.yml\ndocs: https://developer.textmaster.com/apps/building-oauth-apps/scopes-for-oauth-apps\ncorroboration: collections/textmaster-api-v1-postman-collection.json\nchecked: '2026-08-17'\nsummary: >-\n  22 OAuth scopes in the union of three provider sources. The spec's securityScheme flow map\n  declares only 3 (the preferred_author family); operation `security[]` requirements reference 21;\n  the published scopes documentation tables 20 with descriptions — adding `public`, which no\n  operation names because it is the default scope granted when none is requested. TextMaster's own\n  Postman collection requests all 22 in one string, which is the authoritative full list.\nscope_count: 22\nnaming_convention: >-\n  resource:verb, where verb is one of read / write / manage / plus two resource-specific\n  capability scopes on projects (launch, quote). `resource:manage` is a shorthand granting every\n\
  \  permission on that resource.\nschemes:\n- name: oauth2\n  source: openapi/textmaster-api-v1-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.textmaster.com/oauth/authorize\n    authorizationUrl_docs: https://app.textmaster.com/oauth/authorize\n    tokenUrl: https://api.textmaster.com/oauth/token\n    refreshUrl: https://api.textmaster.com/oauth/token\n  description: OAuth2 Bearer token authentication\n  scope_delimiter: space (URL-encoded as %20 in the authorize redirect)\nscopes:\n- scope: public\n  description: >-\n    Grants read-only access to public information (such as, but not limited to, available\n    languages, options, pricing, expertises). This is the default scope if none is provided.\n  spec_declared: false\n  docs_declared: true\n  operation_count: 0\n  operation_note: >-\n    No operation names it in `security[]`; the /v1/public/* endpoints carry no security\n    requirement at all. Documented as the implicit default.\n  sources:\n\
  \  - https://developer.textmaster.com/apps/building-oauth-apps/scopes-for-oauth-apps\n  - collections/textmaster-api-v1-postman-collection.json\n- scope: user:manage\n  description: Grants full access to user's profile info only (includes `user:email`).\n  includes: [user:email]\n  operation_count: 2\n- scope: user:read\n  description: Grants read-only access to user's profile info.\n  operation_count: 1\n- scope: user:write\n  description: Grants read/write access to user's profile info.\n  operation_count: 2\n- scope: user:email\n  description: Grants read-only access to user's private email address.\n  operation_count: 1\n- scope: glossary:manage\n  description: Grants full access to glossaries (includes the ones shared from organization).\n  operation_count: 1\n- scope: glossary:read\n  description: Grants read-only access to glossaries (includes the ones shared from organization).\n  operation_count: 1\n- scope: glossary:write\n  description: Grants read/write access to glossaries\
  \ (includes the ones shared from organization).\n  operation_count: 1\n- scope: project:manage\n  description: >-\n    Grants full access to projects, documents and templates (includes `project:launch` and\n    `project:quote`).\n  includes: [project:launch, project:quote]\n  operation_count: 28\n- scope: project:read\n  description: Grants read-only access to projects, documents and templates.\n  operation_count: 9\n- scope: project:write\n  description: Grants read/write access to projects, documents and templates.\n  operation_count: 25\n- scope: project:launch\n  description: Grants access to launch projects and debit the client's account.\n  operation_count: 3\n  spend_authority: true\n  spend_note: >-\n    The one scope that moves money. It authorizes launch/finalize/async_launch, which debit the\n    client's prepaid credit wallet. An agent granted project:launch can spend the account balance.\n- scope: project:quote\n  description: Grants access to request project quotations.\n\
  \  operation_count: 1\n- scope: discussion:manage\n  description: Grants full access to team discussions.\n  operation_count: 2\n- scope: discussion:read\n  description: Grants read-only access to team discussions.\n  operation_count: 1\n- scope: discussion:write\n  description: Grants read/write access to team discussions.\n  operation_count: 2\n- scope: transaction:read\n  description: Grants read-only access to financial transactions.\n  operation_count: 3\n- scope: transaction:manage\n  description: >-\n    Full access to financial transactions. Referenced by the transactions, invoices and receipts\n    operations and requested by TextMaster's own Postman collection, but ABSENT from the published\n    scopes table.\n  docs_declared: false\n  operation_count: 3\n- scope: transaction:write\n  description: >-\n    Write access to financial transactions. Referenced by operation `security[]` and the Postman\n    collection, but ABSENT from the published scopes table.\n  docs_declared: false\n\
  \  operation_count: 3\n- scope: preferred_author:manage\n  description: Grants full access to client's preferred authors.\n  spec_description: Allow read & write access to My Authors\n  flows: [authorizationCode]\n  operation_count: 5\n- scope: preferred_author:read\n  description: Grants read-only access to client's preferred authors.\n  spec_description: Allow read access to My Authors\n  flows: [authorizationCode]\n  operation_count: 3\n- scope: preferred_author:write\n  description: Grants write access to client's preferred authors.\n  spec_description: Allow write access to My Authors\n  flows: [authorizationCode]\n  operation_count: 5\ngaps:\n  spec_omits:\n  - public\n  docs_omits:\n  - transaction:manage\n  - transaction:write\n  note: >-\n    Neither the spec nor the docs is complete on its own. Three scopes are recoverable only from\n    the union, which is why this artifact is searched rather than derived.\nconsent_model: >-\n  Requested scopes are shown to the user on the authorization\
  \ form. Users can grant less than was\n  requested and can edit token scopes after the flow completes, so applications must read the\n  granted `scope` attribute on the token and degrade gracefully. Applications may re-run the flow\n  to request additional permissions, which the user may deny.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textmaster/refs/heads/main/scopes/textmaster-scopes.yml
summary_line: 22 scopes · authorizationCode
tags:
- Company
- Translation
- Localization
- Language Services
- Copywriting
- Proofreading
- Machine Translation
- Content Production
- Translation Memory
- Glossary
- Ecommerce Localization
- Product Information Management
- Webhook
- Authentication
- Software-as-a-Service
token_urls:
- https://api.textmaster.com/oauth/token
---
