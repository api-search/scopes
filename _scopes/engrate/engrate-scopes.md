---
api_specs:
- filename: engrate-audit-logs-api-openapi.yml
  format: yaml
  label: Engrate Audit Logs API
  slug: engrate-audit-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-audit-logs-api-openapi.yml
- filename: engrate-benachrichtigung-api-openapi.yml
  format: yaml
  label: Engrate Benachrichtigung API
  slug: engrate-benachrichtigung-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-benachrichtigung-api-openapi.yml
- filename: engrate-betrieb-api-openapi.yml
  format: yaml
  label: Engrate Betrieb API
  slug: engrate-betrieb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-betrieb-api-openapi.yml
- filename: engrate-clearing-api-openapi.yml
  format: yaml
  label: Engrate Clearing API
  slug: engrate-clearing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-clearing-api-openapi.yml
- filename: engrate-core-api-openapi.yml
  format: yaml
  label: Engrate Core API
  slug: engrate-core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-core-api-openapi.yml
- filename: engrate-cost-of-energy-api-openapi.yml
  format: yaml
  label: Engrate Cost Of Energy API
  slug: engrate-cost-of-energy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-cost-of-energy-api-openapi.yml
- filename: engrate-geo-api-openapi.yml
  format: yaml
  label: Engrate Geo API
  slug: engrate-geo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-geo-api-openapi.yml
- filename: engrate-holidays-api-openapi.yml
  format: yaml
  label: Engrate Holidays API
  slug: engrate-holidays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-holidays-api-openapi.yml
- filename: engrate-lokationen-api-openapi.yml
  format: yaml
  label: Engrate Lokationen API
  slug: engrate-lokationen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-lokationen-api-openapi.yml
- filename: engrate-lokationsb-ndel-api-openapi.yml
  format: yaml
  label: Engrate Lokationsbündel API
  slug: engrate-lokationsb-ndel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-lokationsb-ndel-api-openapi.yml
- filename: engrate-mabis-api-openapi.yml
  format: yaml
  label: Engrate Mabis API
  slug: engrate-mabis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-mabis-api-openapi.yml
- filename: engrate-netzbetreiberwechsel-api-openapi.yml
  format: yaml
  label: Engrate Netzbetreiberwechsel API
  slug: engrate-netzbetreiberwechsel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-netzbetreiberwechsel-api-openapi.yml
- filename: engrate-nl-settlement-api-openapi.yml
  format: yaml
  label: Engrate Nl Settlement API
  slug: engrate-nl-settlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-nl-settlement-api-openapi.yml
- filename: engrate-profiles-api-openapi.yml
  format: yaml
  label: Engrate Profiles API
  slug: engrate-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-profiles-api-openapi.yml
- filename: engrate-reference-api-openapi.yml
  format: yaml
  label: Engrate Reference API
  slug: engrate-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-reference-api-openapi.yml
- filename: engrate-schedules-api-openapi.yml
  format: yaml
  label: Engrate Schedules API
  slug: engrate-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-schedules-api-openapi.yml
- filename: engrate-status-request-api-openapi.yml
  format: yaml
  label: Engrate Status Request API
  slug: engrate-status-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-status-request-api-openapi.yml
- filename: engrate-time-series-api-openapi.yml
  format: yaml
  label: Engrate Time Series API
  slug: engrate-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/engrate/openapi/engrate-time-series-api-openapi.yml
authorization_urls:
- https://authz.example-netzbetreiber.de/oauth2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Engrate Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Engrate publishes 5 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Engrate API on a user''s behalf.


  Tokens are issued from https://authz.example-netzbetreiber.de/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Engrate
provider_slug: engrate
schemes:
- description: 'OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der

    Ausbaustufe 1 über das Signaturzertifikat der Smart-Metering-PKI; die Architektur

    ist so angelegt, dass sie später um OpenID Connect und föderierte Identitäten

    (etwa europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu

    ändern.


    Damit werden drei Anforderungen adressiert, die eine ausschließlich

    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:

    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen

    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  - authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  name: oauth2
  source: openapi/engrate-benachrichtigung-api-openapi.yml
- description: 'OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der

    Ausbaustufe 1 über das Signaturzertifikat der Smart-Metering-PKI; die Architektur

    ist so angelegt, dass sie später um OpenID Connect und föderierte Identitäten

    (etwa europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu

    ändern.


    Damit werden drei Anforderungen adressiert, die eine ausschließlich

    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:

    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen

    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  - authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  name: oauth2
  source: openapi/engrate-betrieb-api-openapi.yml
- description: 'OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der

    Ausbaustufe 1 über das Signaturzertifikat der Smart-Metering-PKI; die Architektur

    ist so angelegt, dass sie später um OpenID Connect und föderierte Identitäten

    (etwa europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu

    ändern.


    Damit werden drei Anforderungen adressiert, die eine ausschließlich

    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:

    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen

    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  - authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  name: oauth2
  source: openapi/engrate-clearing-api-openapi.yml
- description: 'OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der

    Ausbaustufe 1 über das Signaturzertifikat der Smart-Metering-PKI; die Architektur

    ist so angelegt, dass sie später um OpenID Connect und föderierte Identitäten

    (etwa europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu

    ändern.


    Damit werden drei Anforderungen adressiert, die eine ausschließlich

    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:

    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen

    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  - authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  name: oauth2
  source: openapi/engrate-lokationen-api-openapi.yml
- description: 'OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der

    Ausbaustufe 1 über das Signaturzertifikat der Smart-Metering-PKI; die Architektur

    ist so angelegt, dass sie später um OpenID Connect und föderierte Identitäten

    (etwa europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu

    ändern.


    Damit werden drei Anforderungen adressiert, die eine ausschließlich

    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:

    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen

    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  - authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  name: oauth2
  source: openapi/engrate-lokationsb-ndel-api-openapi.yml
- description: 'OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der

    Ausbaustufe 1 über das Signaturzertifikat der Smart-Metering-PKI; die Architektur

    ist so angelegt, dass sie später um OpenID Connect und föderierte Identitäten

    (etwa europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu

    ändern.


    Damit werden drei Anforderungen adressiert, die eine ausschließlich

    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:

    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen

    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  - authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token
  name: oauth2
  source: openapi/engrate-netzbetreiberwechsel-api-openapi.yml
scope_count: 5
scope_names:
- benachrichtigung:schreiben
- clearing:schreiben
- lokationsbuendel:lesen
- lokationsbuendel:schreiben
- netzbetreiberwechsel:schreiben
scopes:
- description: Abonnements verwalten
  flows:
  - clientCredentials
  scope: benachrichtigung:schreiben
- description: Clearing-Fälle eröffnen und fortschreiben
  flows:
  - clientCredentials
  scope: clearing:schreiben
- description: Lokationsbündel und Lokationen lesen
  flows:
  - authorizationCode
  - clientCredentials
  scope: lokationsbuendel:lesen
- description: Lokationsbündel ändern (nur verantwortlicher Netzbetreiber)
  flows:
  - clientCredentials
  scope: lokationsbuendel:schreiben
- description: Übergabepakete anfordern
  flows:
  - clientCredentials
  scope: netzbetreiberwechsel:schreiben
slug: engrate-scopes
source_filename: engrate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/engrate-benachrichtigung-api-openapi.yml, openapi/engrate-betrieb-api-openapi.yml,\n  openapi/engrate-clearing-api-openapi.yml, openapi/engrate-lokationen-api-openapi.yml, openapi/engrate-lokationsb-ndel-api-openapi.yml,\n  openapi/engrate-netzbetreiberwechsel-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/engrate-benachrichtigung-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  description: |-\n    OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der\n    Ausbaustufe 1 über das Signaturzertifikat der Smart-Metering-PKI; die Architektur\n    ist so angelegt, dass sie später um OpenID Connect und föderierte Identitäten\n    (etwa\
  \ europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu\n    ändern.\n\n    Damit werden drei Anforderungen adressiert, die eine ausschließlich\n    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:\n    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen\n    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.\n- name: oauth2\n  source: openapi/engrate-betrieb-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  description: |-\n    OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der\n    Ausbaustufe 1 über das Signaturzertifikat der Smart-Metering-PKI; die Architektur\n    ist so angelegt, dass sie später um OpenID Connect und föderierte\
  \ Identitäten\n    (etwa europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu\n    ändern.\n\n    Damit werden drei Anforderungen adressiert, die eine ausschließlich\n    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:\n    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen\n    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.\n- name: oauth2\n  source: openapi/engrate-clearing-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  description: |-\n    OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der\n    Ausbaustufe 1 über das Signaturzertifikat der Smart-Metering-PKI; die Architektur\n    ist so angelegt, dass sie später um\
  \ OpenID Connect und föderierte Identitäten\n    (etwa europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu\n    ändern.\n\n    Damit werden drei Anforderungen adressiert, die eine ausschließlich\n    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:\n    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen\n    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.\n- name: oauth2\n  source: openapi/engrate-lokationen-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  description: |-\n    OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der\n    Ausbaustufe 1 über das Signaturzertifikat der Smart-Metering-PKI; die Architektur\n    ist\
  \ so angelegt, dass sie später um OpenID Connect und föderierte Identitäten\n    (etwa europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu\n    ändern.\n\n    Damit werden drei Anforderungen adressiert, die eine ausschließlich\n    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:\n    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen\n    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.\n- name: oauth2\n  source: openapi/engrate-lokationsb-ndel-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  description: |-\n    OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der\n    Ausbaustufe 1 über das Signaturzertifikat der Smart-Metering-PKI;\
  \ die Architektur\n    ist so angelegt, dass sie später um OpenID Connect und föderierte Identitäten\n    (etwa europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu\n    ändern.\n\n    Damit werden drei Anforderungen adressiert, die eine ausschließlich\n    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:\n    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen\n    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.\n- name: oauth2\n  source: openapi/engrate-netzbetreiberwechsel-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://authz.example-netzbetreiber.de/oauth2/authorize\n    tokenUrl: https://authz.example-netzbetreiber.de/oauth2/token\n  description: |-\n    OAuth 2.0. Die Authentisierung des Clients am Authorization Server erfolgt in der\n    Ausbaustufe 1 über das Signaturzertifikat\
  \ der Smart-Metering-PKI; die Architektur\n    ist so angelegt, dass sie später um OpenID Connect und föderierte Identitäten\n    (etwa europäische ID-Wallets) erweitert werden kann, ohne die Ressourcen-APIs zu\n    ändern.\n\n    Damit werden drei Anforderungen adressiert, die eine ausschließlich\n    zertifikatsbasierte Marktpartner-Authentisierung nicht abbilden kann:\n    Zugriff von Letztverbrauchern auf ihre eigenen Daten, übertragbare Berechtigungen\n    an Dritte und Anschlussfähigkeit an übergreifende Datenräume.\nscopes:\n- scope: benachrichtigung:schreiben\n  description: Abonnements verwalten\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/engrate-benachrichtigung-api-openapi.yml\n  - openapi/engrate-betrieb-api-openapi.yml\n  - openapi/engrate-clearing-api-openapi.yml\n  - openapi/engrate-lokationen-api-openapi.yml\n  - openapi/engrate-lokationsb-ndel-api-openapi.yml\n  - openapi/engrate-netzbetreiberwechsel-api-openapi.yml\n- scope: clearing:schreiben\n  description:\
  \ Clearing-Fälle eröffnen und fortschreiben\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/engrate-benachrichtigung-api-openapi.yml\n  - openapi/engrate-betrieb-api-openapi.yml\n  - openapi/engrate-clearing-api-openapi.yml\n  - openapi/engrate-lokationen-api-openapi.yml\n  - openapi/engrate-lokationsb-ndel-api-openapi.yml\n  - openapi/engrate-netzbetreiberwechsel-api-openapi.yml\n- scope: lokationsbuendel:lesen\n  description: Lokationsbündel und Lokationen lesen\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/engrate-benachrichtigung-api-openapi.yml\n  - openapi/engrate-betrieb-api-openapi.yml\n  - openapi/engrate-clearing-api-openapi.yml\n  - openapi/engrate-lokationen-api-openapi.yml\n  - openapi/engrate-lokationsb-ndel-api-openapi.yml\n  - openapi/engrate-netzbetreiberwechsel-api-openapi.yml\n- scope: lokationsbuendel:schreiben\n  description: Lokationsbündel ändern (nur verantwortlicher Netzbetreiber)\n  flows:\n  - clientCredentials\n \
  \ sources:\n  - openapi/engrate-benachrichtigung-api-openapi.yml\n  - openapi/engrate-betrieb-api-openapi.yml\n  - openapi/engrate-clearing-api-openapi.yml\n  - openapi/engrate-lokationen-api-openapi.yml\n  - openapi/engrate-lokationsb-ndel-api-openapi.yml\n  - openapi/engrate-netzbetreiberwechsel-api-openapi.yml\n- scope: netzbetreiberwechsel:schreiben\n  description: Übergabepakete anfordern\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/engrate-benachrichtigung-api-openapi.yml\n  - openapi/engrate-betrieb-api-openapi.yml\n  - openapi/engrate-clearing-api-openapi.yml\n  - openapi/engrate-lokationen-api-openapi.yml\n  - openapi/engrate-lokationsb-ndel-api-openapi.yml\n  - openapi/engrate-netzbetreiberwechsel-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/engrate/scopes/engrate-scopes.yml
summary_line: 5 scopes · clientCredentials/authorizationCode
tags:
- Company
- Energy
- Platform
- Integration
- Markets
token_bound: false
token_urls:
- https://authz.example-netzbetreiber.de/oauth2/token
---
