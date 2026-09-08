---
authorization_urls: []
description: ''
docs: https://developers.welcomekit.co/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Welcome To The Jungle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Welcome to the Jungle uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Welcome to the Jungle
provider_slug: welcome-to-the-jungle
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: welcome-to-the-jungle-scopes
source_filename: welcome-to-the-jungle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://developers.welcomekit.co/scopes\ndocs: https://developers.welcomekit.co/scopes\napi: Welcome to the Jungle Solutions API\nsummary: 'Welcome to the Jungle Solutions publishes a complete OAuth scope reference — 20 standard\n  scopes plus 10 partnership-gated su_* / cms_* scopes. Scopes follow a resource_access naming\n  convention where the suffix is _r (read), _w (write) or _rw (read and write). Scopes are not\n  self-selected: you tell the vendor your use case through the help form and they open the matching\n  set. Transcribed verbatim from the published table; no scope here was inferred.'\nconvention:\n  pattern: <resource>_<access>\n  access_suffixes:\n    _r: read\n    _w: write\n    _rw: read and write\n  privileged_prefix: 'su_ — company-wide (super-user) read access across organizations, granted only under a dedicated partnership'\nscope_count: 29\nscopes:\n- name: me_r\n  access: read\n  partnership_required:\
  \ false\n  description: Read access on your personal information.\n- name: organizations_rw\n  access: read-write\n  partnership_required: false\n  description: Read and write access on your organization(s).\n- name: organizations_r\n  access: read\n  partnership_required: false\n  description: Read access on your organization(s).\n- name: jobs_rw\n  access: read-write\n  partnership_required: false\n  description: Read and write access on your job offers.\n- name: jobs_r\n  access: read\n  partnership_required: false\n  description: Read access on your job offers.\n- name: offices_rw\n  access: read-write\n  partnership_required: false\n  description: Read and write access on your offices.\n- name: offices_r\n  access: read\n  partnership_required: false\n  description: Read access on your offices.\n- name: departments_rw\n  access: read-write\n  partnership_required: false\n  description: Read and write access on your departments.\n- name: departments_r\n  access: read\n  partnership_required:\
  \ false\n  description: Read access on your departments.\n- name: candidates_rw\n  access: read-write\n  partnership_required: false\n  description: Read and write access on all candidates (limited to the user's role).\n- name: candidates_r\n  access: read\n  partnership_required: false\n  description: Read access on all candidates (limited to the user's role).\n- name: my_candidates_rw\n  access: read-write\n  partnership_required: false\n  description: 'Read and write access limited to candidates this user created through the API — the\n    least-privilege scope for synchronising an external service without exposing the whole candidate base.'\n- name: documents_rw\n  access: read-write\n  partnership_required: false\n  description: Read and write access on your candidate files.\n- name: documents_r\n  access: read\n  partnership_required: false\n  description: Read access on your candidate files.\n- name: emails_rw\n  access: read-write\n  partnership_required: false\n  description:\
  \ Read and write access on your candidate emails.\n- name: emails_r\n  access: read\n  partnership_required: false\n  description: Read access on your candidate emails.\n- name: comments_w\n  access: write\n  partnership_required: false\n  description: Write access on your candidate comments.\n- name: images_r\n  access: read\n  partnership_required: false\n  description: Read access to your images.\n- name: moves_r\n  access: read\n  partnership_required: false\n  description: Read access on candidate moves (pipeline stage transitions).\n- name: videos_r\n  access: read\n  partnership_required: false\n  description: Read access on your video files.\n- name: su_offices_r\n  access: read\n  partnership_required: true\n  description: Read access on offices of a company.\n- name: su_jobs_r\n  access: read\n  partnership_required: true\n  description: Read access on jobs of a company. Required by GET /jobs/all.\n- name: su_departments_r\n  access: read\n  partnership_required: true\n  description:\
  \ Read access on departments of a company.\n- name: su_organizations_r\n  access: read\n  partnership_required: true\n  description: Read access on organization information of a company. Required by GET /organizations.\n- name: su_images_r\n  access: read\n  partnership_required: true\n  description: Read access to images of a company.\n- name: su_videos_r\n  access: read\n  partnership_required: true\n  description: Read access to videos of a company.\n- name: cms_articles_r\n  access: read\n  partnership_required: true\n  description: Read access to WTTJ articles. Required by GET /cms/articles/all.\n- name: cms_collections_r\n  access: read\n  partnership_required: true\n  description: Read access to WTTJ collections.\n- name: cms_collection_categories_r\n  access: read\n  partnership_required: true\n  description: Read access to WTTJ collection categories.\nnotes:\n- 'The published table lists su_offices_r twice; it is recorded once here. That is the only discrepancy\n  between the\
  \ source table and this transcription.'\n- 'The docs cite the OAuth 2.0 scope definition (draft-ietf-oauth-v2-31 §3.3) but publish no\n  authorization endpoint, token endpoint or discovery document — scopes are granted administratively.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/welcome-to-the-jungle/refs/heads/main/scopes/welcome-to-the-jungle-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Human Resources
- Recruiting
- Applicant Tracking
- Jobs
- Employer Branding
- Talent Acquisition
- HR Tech
- France
token_urls: []
---
