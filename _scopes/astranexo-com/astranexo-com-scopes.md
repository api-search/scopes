---
api_specs:
- filename: astranexo-com-archivo-api-openapi.yml
  format: yaml
  label: Astranexo Archivo API
  slug: astranexo-com-archivo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-archivo-api-openapi.yml
- filename: astranexo-com-cat-logos-api-openapi.yml
  format: yaml
  label: Astranexo Catálogos API
  slug: astranexo-com-cat-logos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-cat-logos-api-openapi.yml
- filename: astranexo-com-claves-api-api-openapi.yml
  format: yaml
  label: Astranexo Claves API
  slug: astranexo-com-claves-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-claves-api-api-openapi.yml
- filename: astranexo-com-cuenta-y-uso-api-openapi.yml
  format: yaml
  label: Astranexo Cuenta y uso API
  slug: astranexo-com-cuenta-y-uso-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-cuenta-y-uso-api-openapi.yml
- filename: astranexo-com-documentos-api-openapi.yml
  format: yaml
  label: Astranexo Documentos API
  slug: astranexo-com-documentos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-documentos-api-openapi.yml
- filename: astranexo-com-estado-api-openapi.yml
  format: yaml
  label: Astranexo Estado API
  slug: astranexo-com-estado-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-estado-api-openapi.yml
- filename: astranexo-com-hacienda-api-openapi.yml
  format: yaml
  label: Astranexo Hacienda API
  slug: astranexo-com-hacienda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-hacienda-api-openapi.yml
- filename: astranexo-com-mensajes-receptor-api-openapi.yml
  format: yaml
  label: Astranexo Mensajes receptor API
  slug: astranexo-com-mensajes-receptor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-mensajes-receptor-api-openapi.yml
- filename: astranexo-com-organizaciones-api-openapi.yml
  format: yaml
  label: Astranexo Organizaciones API
  slug: astranexo-com-organizaciones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-organizaciones-api-openapi.yml
- filename: astranexo-com-receptores-api-openapi.yml
  format: yaml
  label: Astranexo Receptores API
  slug: astranexo-com-receptores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-receptores-api-openapi.yml
- filename: astranexo-com-tipo-de-cambio-api-openapi.yml
  format: yaml
  label: Astranexo Tipo de cambio API
  slug: astranexo-com-tipo-de-cambio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-tipo-de-cambio-api-openapi.yml
- filename: astranexo-com-webhooks-api-openapi.yml
  format: yaml
  label: Astranexo Webhooks API
  slug: astranexo-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astranexo-com/openapi/astranexo-com-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Astranexo Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Astranexo publishes 25 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Astranexo API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Astranexo
provider_slug: astranexo-com
schemes: []
scope_count: 25
scope_names:
- invoices:read
- invoices:write
- invoices:sign
- invoices:void
- credit-notes:read
- credit-notes:write
- credit-notes:sign
- debit-notes:read
- debit-notes:write
- debit-notes:sign
- tickets:read
- tickets:write
- tickets:sign
- recipients:read
- recipients:write
- hacienda:query
- hacienda:validate
- settings:read
- settings:manage
- webhooks:read
- webhooks:write
- webhooks:manage
- reference:read
- documents:export
- account:manage
scopes:
- description: Consultar comprobantes y facturas
  flows: []
  scope: invoices:read
- description: Crear y actualizar facturas
  flows: []
  scope: invoices:write
- description: Firmar y enviar comprobantes a Hacienda, y enviar Mensajes Receptor
  flows: []
  scope: invoices:sign
- description: Anular comprobantes
  flows: []
  scope: invoices:void
- description: Consultar notas de crédito
  flows: []
  scope: credit-notes:read
- description: Crear y actualizar notas de crédito
  flows: []
  scope: credit-notes:write
- description: Firmar y enviar notas de crédito
  flows: []
  scope: credit-notes:sign
- description: Consultar notas de débito
  flows: []
  scope: debit-notes:read
- description: Crear y actualizar notas de débito
  flows: []
  scope: debit-notes:write
- description: Firmar y enviar notas de débito
  flows: []
  scope: debit-notes:sign
- description: Consultar tiquetes
  flows: []
  scope: tickets:read
- description: Crear y actualizar tiquetes
  flows: []
  scope: tickets:write
- description: Firmar y enviar tiquetes
  flows: []
  scope: tickets:sign
- description: Consultar receptores guardados
  flows: []
  scope: recipients:read
- description: Crear y actualizar receptores
  flows: []
  scope: recipients:write
- description: Consultar el estado de Hacienda y de un comprobante en Hacienda
  flows: []
  scope: hacienda:query
- description: Validar un comprobante sin enviarlo
  flows: []
  scope: hacienda:validate
- description: Ver los datos de la organización y el estado del certificado
  flows: []
  scope: settings:read
- description: Cambiar los datos de la organización y subir certificados
  flows: []
  scope: settings:manage
- description: Ver webhooks
  flows: []
  scope: webhooks:read
- description: Crear webhooks
  flows: []
  scope: webhooks:write
- description: Modificar, probar y eliminar webhooks
  flows: []
  scope: webhooks:manage
- description: Consultar tipos de cambio
  flows: []
  scope: reference:read
- description: Descargar los XML en un ZIP
  flows: []
  scope: documents:export
- description: Administrar organizaciones y llaves (solo llaves de cuenta)
  flows: []
  scope: account:manage
slug: astranexo-com-scopes
source_filename: astranexo-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://aster.astranexo.com/docs/autenticacion/\nscopes:\n  - scope: invoices:read\n    description: Consultar comprobantes y facturas\n  - scope: invoices:write\n    description: Crear y actualizar facturas\n  - scope: invoices:sign\n    description: Firmar y enviar comprobantes a Hacienda, y enviar Mensajes Receptor\n  - scope: invoices:void\n    description: Anular comprobantes\n  - scope: credit-notes:read\n    description: Consultar notas de crédito\n  - scope: credit-notes:write\n    description: Crear y actualizar notas de crédito\n  - scope: credit-notes:sign\n    description: Firmar y enviar notas de crédito\n  - scope: debit-notes:read\n    description: Consultar notas de débito\n  - scope: debit-notes:write\n    description: Crear y actualizar notas de débito\n  - scope: debit-notes:sign\n    description: Firmar y enviar notas de débito\n  - scope: tickets:read\n    description: Consultar tiquetes\n  - scope: tickets:write\n\
  \    description: Crear y actualizar tiquetes\n  - scope: tickets:sign\n    description: Firmar y enviar tiquetes\n  - scope: recipients:read\n    description: Consultar receptores guardados\n  - scope: recipients:write\n    description: Crear y actualizar receptores\n  - scope: hacienda:query\n    description: Consultar el estado de Hacienda y de un comprobante en Hacienda\n  - scope: hacienda:validate\n    description: Validar un comprobante sin enviarlo\n  - scope: settings:read\n    description: Ver los datos de la organización y el estado del certificado\n  - scope: settings:manage\n    description: Cambiar los datos de la organización y subir certificados\n  - scope: webhooks:read\n    description: Ver webhooks\n  - scope: webhooks:write\n    description: Crear webhooks\n  - scope: webhooks:manage\n    description: Modificar, probar y eliminar webhooks\n  - scope: reference:read\n    description: Consultar tipos de cambio\n  - scope: documents:export\n    description: Descargar los\
  \ XML en un ZIP\n  - scope: account:manage\n    description: Administrar organizaciones y llaves (solo llaves de cuenta)\n"
source_yaml_url: https://artifacts.apis.io/astranexo-com/scopes/astranexo-com-scopes.yml
summary_line: 25 scopes
tags:
- Software
- Business
- Software-as-a-Service
- Spanish
- CRM
token_bound: false
token_urls: []
---
