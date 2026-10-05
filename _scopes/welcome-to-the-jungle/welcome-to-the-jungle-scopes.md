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
overview: 'Welcome to the Jungle publishes 29 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Welcome to the Jungle API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Welcome to the Jungle
provider_slug: welcome-to-the-jungle
schemes: []
scope_count: 29
scope_names:
- me_r
- organizations_rw
- organizations_r
- jobs_rw
- jobs_r
- offices_rw
- offices_r
- departments_rw
- departments_r
- candidates_rw
- candidates_r
- my_candidates_rw
- documents_rw
- documents_r
- emails_rw
- emails_r
- comments_w
- images_r
- moves_r
- videos_r
- su_offices_r
- su_jobs_r
- su_departments_r
- su_organizations_r
- su_images_r
- su_videos_r
- cms_articles_r
- cms_collections_r
- cms_collection_categories_r
scopes:
- description: Read access on your personal information.
  flows: []
  scope: me_r
- description: Read and write access on your organization(s).
  flows: []
  scope: organizations_rw
- description: Read access on your organization(s).
  flows: []
  scope: organizations_r
- description: Read and write access on your job offers.
  flows: []
  scope: jobs_rw
- description: Read access on your job offers.
  flows: []
  scope: jobs_r
- description: Read and write access on your offices.
  flows: []
  scope: offices_rw
- description: Read access on your offices.
  flows: []
  scope: offices_r
- description: Read and write access on your departments.
  flows: []
  scope: departments_rw
- description: Read access on your departments.
  flows: []
  scope: departments_r
- description: Read and write access on all candidates (limited to the user's role).
  flows: []
  scope: candidates_rw
- description: Read access on all candidates (limited to the user's role).
  flows: []
  scope: candidates_r
- description: Read and write access limited to candidates this user created through the API — the least-privilege scope for synchronising an external service without exposing the whole candidate base.
  flows: []
  scope: my_candidates_rw
- description: Read and write access on your candidate files.
  flows: []
  scope: documents_rw
- description: Read access on your candidate files.
  flows: []
  scope: documents_r
- description: Read and write access on your candidate emails.
  flows: []
  scope: emails_rw
- description: Read access on your candidate emails.
  flows: []
  scope: emails_r
- description: Write access on your candidate comments.
  flows: []
  scope: comments_w
- description: Read access to your images.
  flows: []
  scope: images_r
- description: Read access on candidate moves (pipeline stage transitions).
  flows: []
  scope: moves_r
- description: Read access on your video files.
  flows: []
  scope: videos_r
- description: Read access on offices of a company.
  flows: []
  scope: su_offices_r
- description: Read access on jobs of a company. Required by GET /jobs/all.
  flows: []
  scope: su_jobs_r
- description: Read access on departments of a company.
  flows: []
  scope: su_departments_r
- description: Read access on organization information of a company. Required by GET /organizations.
  flows: []
  scope: su_organizations_r
- description: Read access to images of a company.
  flows: []
  scope: su_images_r
- description: Read access to videos of a company.
  flows: []
  scope: su_videos_r
- description: Read access to WTTJ articles. Required by GET /cms/articles/all.
  flows: []
  scope: cms_articles_r
- description: Read access to WTTJ collections.
  flows: []
  scope: cms_collections_r
- description: Read access to WTTJ collection categories.
  flows: []
  scope: cms_collection_categories_r
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
summary_line: 29 scopes
tags:
- Company
- Human Resources
- Recruiting
- Applicant Tracking
- Job
- Employer Branding
- Talent Acquisition
- France
token_bound: false
token_urls: []
---
