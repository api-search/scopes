---
authorization_urls: []
description: ''
docs: https://developer.factset.com/learn/authentication-oauth2-scopes
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Factset Scopes
name_suffix: OAuth Scopes
note: FactSet documents an OAuth 2.0 scopes model (URL-style scope names, optional on Client Credentials and Authorization Code flows) at developer.factset.com/learn/authentication-oauth2-scopes, but the portal page is JavaScript-rendered and FactSet publishes no complete per-API scope catalog; the scopes below are the concrete scope names documented in FactSet's official OAuth 2.0 guidelines (github.com/factset/oauth2-guidelines), which provide no per-scope descriptions.
overview: 'Factset publishes 9 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Factset API on a user''s behalf.


  Tokens are issued from https://auth.factset.com/as/token.oauth2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Factset
provider_slug: factset
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/conversational-api-powered-by-mercury-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/direct-streaming-of-transaction-messages-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/documents-distributor-callstreet-events-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/esg-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/event-calendar-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-documents-distributor-callstreet-events-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-esg-api-openapi.yml
- description: OAuth 2.0 Client Credentials flow. Obtain an access token from the FactSet token endpoint using your client ID and client secret.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-fundamentals-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-global-filings-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-irn-notes-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-pa-engine-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-portfolio-metadata-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-portfolio-reporting-batcher-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-quant-engine-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-real-time-news-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-real-time-price-alerting-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-real-time-quotes-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-real-time-time-series-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-spar-engine-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-streetaccount-news-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-tick-history-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-vault-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/factset-vermilion-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/fixed-income-calculation-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/fundamentals-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/global-filings-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/investment-banking-office-refresh-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/irn-notes-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/issue-tracker-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/natural-language-processing-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/ofdb-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/open-partners-documents-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/open-risk-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/overview-report-builder-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/pa-engine-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/portfolio-metadata-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/portfolio-reporting-batcher-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/quant-engine-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/real-time-news-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/real-time-price-alerting-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/real-time-quotes-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/real-time-time-series-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/s-p-global-fixed-income-evaluated-prices-and-analytics-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/spar-engine-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/streetaccount-news-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/tick-history-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/trading-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/vault-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.factset.com/as/token.oauth2
  name: FactSetOAuth2
  source: openapi/vermilion-openapi-original.yml
scope_count: 9
scope_names:
- https://api.factset.com/analytics/accounts.fullcontrol
- https://api.factset.com/analytics/engines.fullcontrol
- https://api.factset.com/analytics/engines.pub.fullcontrol
- https://api.factset.com/analytics/engines.readonly
- https://api.factset.com/analytics/engines.vault.fullcontrol
- https://api.factset.com/analytics/lookups.readonly
- https://api.factset.com/analytics/lookups.pa.readonly
- https://api.factset.com/analytics/lookups.spar.readonly
- https://api.factset.com/analytics/lookups.vault.readonly
scopes:
- description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines; FactSet does not publish a per-scope description.
  flows: []
  scope: https://api.factset.com/analytics/accounts.fullcontrol
- description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines; FactSet does not publish a per-scope description.
  flows: []
  scope: https://api.factset.com/analytics/engines.fullcontrol
- description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines; FactSet does not publish a per-scope description.
  flows: []
  scope: https://api.factset.com/analytics/engines.pub.fullcontrol
- description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines; FactSet does not publish a per-scope description.
  flows: []
  scope: https://api.factset.com/analytics/engines.readonly
- description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines; FactSet does not publish a per-scope description.
  flows: []
  scope: https://api.factset.com/analytics/engines.vault.fullcontrol
- description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines; FactSet does not publish a per-scope description.
  flows: []
  scope: https://api.factset.com/analytics/lookups.readonly
- description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines; FactSet does not publish a per-scope description.
  flows: []
  scope: https://api.factset.com/analytics/lookups.pa.readonly
- description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines; FactSet does not publish a per-scope description.
  flows: []
  scope: https://api.factset.com/analytics/lookups.spar.readonly
- description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines; FactSet does not publish a per-scope description.
  flows: []
  scope: https://api.factset.com/analytics/lookups.vault.readonly
slug: factset-scopes
source_filename: factset-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\ndocs: https://developer.factset.com/learn/authentication-oauth2-scopes\nnote: FactSet documents an OAuth 2.0 scopes model (URL-style scope names, optional\n  on Client Credentials and Authorization Code flows) at developer.factset.com/learn/authentication-oauth2-scopes,\n  but the portal page is JavaScript-rendered and FactSet publishes no complete per-API\n  scope catalog; the scopes below are the concrete scope names documented in FactSet's\n  official OAuth 2.0 guidelines (github.com/factset/oauth2-guidelines), which provide\n  no per-scope descriptions.\nsource: openapi/conversational-api-powered-by-mercury-openapi-original.yml, openapi/direct-streaming-of-transaction-messages-openapi-original.yml,\n  openapi/documents-distributor-callstreet-events-openapi-original.yml, openapi/esg-openapi-original.yml,\n  openapi/event-calendar-openapi-original.yml, openapi/factset-documents-distributor-callstreet-events-openapi.yml,\n  openapi/factset-esg-api-openapi.yml,\
  \ openapi/factset-fundamentals-api-openapi.yml, openapi/factset-global-filings-api-openapi.yml,\n  openapi/factset-irn-notes-api-openapi.yml, openapi/factset-pa-engine-api-openapi.yml, openapi/factset-portfolio-metadata-api-openapi.yml,\n  openapi/factset-portfolio-reporting-batcher-api-openapi.yml, openapi/factset-quant-engine-api-openapi.yml,\n  openapi/factset-real-time-news-api-openapi.yml, openapi/factset-real-time-price-alerting-api-openapi.yml,\n  openapi/factset-real-time-quotes-api-openapi.yml, openapi/factset-real-time-time-series-api-openapi.yml,\n  openapi/factset-spar-engine-api-openapi.yml, openapi/factset-streetaccount-news-api-openapi.yml,\n  openapi/factset-tick-history-api-openapi.yml, openapi/factset-vault-api-openapi.yml, openapi/factset-vermilion-api-openapi.yml,\n  openapi/fixed-income-calculation-openapi-original.yml, openapi/fundamentals-openapi-original.yml,\n  openapi/global-filings-openapi-original.yml, openapi/investment-banking-office-refresh-openapi-original.yml,\n\
  \  openapi/irn-notes-openapi-original.yml, openapi/issue-tracker-openapi-original.yml, openapi/natural-language-processing-openapi-original.yml,\n  openapi/ofdb-openapi-original.yml, openapi/open-partners-documents-openapi-original.yml, openapi/open-risk-openapi-original.yml,\n  openapi/overview-report-builder-openapi-original.yml, openapi/pa-engine-openapi-original.yml,\n  openapi/portfolio-metadata-openapi-original.yml, openapi/portfolio-reporting-batcher-openapi-original.yml,\n  openapi/quant-engine-openapi-original.yml, openapi/real-time-news-openapi-original.yml, openapi/real-time-price-alerting-openapi-original.yml,\n  openapi/real-time-quotes-openapi-original.yml, openapi/real-time-time-series-openapi-original.yml,\n  openapi/s-p-global-fixed-income-evaluated-prices-and-analytics-openapi-original.yml, openapi/spar-engine-openapi-original.yml,\n  openapi/streetaccount-news-openapi-original.yml, openapi/tick-history-openapi-original.yml,\n  openapi/trading-openapi-original.yml, openapi/vault-openapi-original.yml,\
  \ openapi/vermilion-openapi-original.yml\nschemes:\n- name: FactSetOAuth2\n  source: openapi/conversational-api-powered-by-mercury-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/direct-streaming-of-transaction-messages-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/documents-distributor-callstreet-events-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/esg-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/event-calendar-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n\
  \  source: openapi/factset-documents-distributor-callstreet-events-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-esg-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-fundamentals-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n  description: OAuth 2.0 Client Credentials flow. Obtain an access token from the FactSet token\n    endpoint using your client ID and client secret.\n- name: FactSetOAuth2\n  source: openapi/factset-global-filings-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-irn-notes-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n\
  - name: FactSetOAuth2\n  source: openapi/factset-pa-engine-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-portfolio-metadata-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-portfolio-reporting-batcher-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-quant-engine-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-real-time-news-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-real-time-price-alerting-api-openapi.yml\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-real-time-quotes-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-real-time-time-series-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-spar-engine-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-streetaccount-news-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-tick-history-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-vault-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/factset-vermilion-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/fixed-income-calculation-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/fundamentals-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/global-filings-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/investment-banking-office-refresh-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n\
  \  source: openapi/irn-notes-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/issue-tracker-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/natural-language-processing-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/ofdb-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/open-partners-documents-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/open-risk-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n\
  - name: FactSetOAuth2\n  source: openapi/overview-report-builder-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/pa-engine-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/portfolio-metadata-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/portfolio-reporting-batcher-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/quant-engine-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/real-time-news-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/real-time-price-alerting-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/real-time-quotes-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/real-time-time-series-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/s-p-global-fixed-income-evaluated-prices-and-analytics-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/spar-engine-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n\
  \  source: openapi/streetaccount-news-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/tick-history-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/trading-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/vault-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\n- name: FactSetOAuth2\n  source: openapi/vermilion-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.factset.com/as/token.oauth2\nscopes:\n- scope: https://api.factset.com/analytics/accounts.fullcontrol\n  description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines;\n    FactSet does\
  \ not publish a per-scope description.\n  sources:\n  - https://github.com/factset/oauth2-guidelines\n- scope: https://api.factset.com/analytics/engines.fullcontrol\n  description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines;\n    FactSet does not publish a per-scope description.\n  sources:\n  - https://github.com/factset/oauth2-guidelines\n- scope: https://api.factset.com/analytics/engines.pub.fullcontrol\n  description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines;\n    FactSet does not publish a per-scope description.\n  sources:\n  - https://github.com/factset/oauth2-guidelines\n- scope: https://api.factset.com/analytics/engines.readonly\n  description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines;\n    FactSet does not publish a per-scope description.\n  sources:\n  - https://github.com/factset/oauth2-guidelines\n- scope: https://api.factset.com/analytics/engines.vault.fullcontrol\n  description: Analytics API\
  \ scope named in FactSet's official OAuth 2.0 guidelines;\n    FactSet does not publish a per-scope description.\n  sources:\n  - https://github.com/factset/oauth2-guidelines\n- scope: https://api.factset.com/analytics/lookups.readonly\n  description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines;\n    FactSet does not publish a per-scope description.\n  sources:\n  - https://github.com/factset/oauth2-guidelines\n- scope: https://api.factset.com/analytics/lookups.pa.readonly\n  description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines;\n    FactSet does not publish a per-scope description.\n  sources:\n  - https://github.com/factset/oauth2-guidelines\n- scope: https://api.factset.com/analytics/lookups.spar.readonly\n  description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines;\n    FactSet does not publish a per-scope description.\n  sources:\n  - https://github.com/factset/oauth2-guidelines\n- scope: https://api.factset.com/analytics/lookups.vault.readonly\n\
  \  description: Analytics API scope named in FactSet's official OAuth 2.0 guidelines;\n    FactSet does not publish a per-scope description.\n  sources:\n  - https://github.com/factset/oauth2-guidelines\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/scopes/factset-scopes.yml
summary_line: 9 scopes · clientCredentials
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
token_urls:
- https://auth.factset.com/as/token.oauth2
---
