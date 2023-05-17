# aspace-config
Our ArchivesSpace configuration choices, including plugins and their versions.

We install any new plugins, version updates, or config changes on dev for testing before making the corresponding change on prod.

**Prod status:**

- Prod is behind by one version on user_defined_in_basic.
- Prod is lacking as_marcao
- Prod is behind on en.yml (label in resource/user_defined/boolean_1)

**Dev status:**

These are the plugins we currently have installed on dev. 

- name: as_marcao

  branch: v0.3
  
  url: https://github.com/hudmol/as_marcao/releases/tag/v0.3
  
  added: 5/15/2023

- name: as_princeton_shim

  branch: v1.0
  
  url: https://github.com/hudmol/as_princeton_shim.git
  
- name: as_spreadsheet_bulk_updater

  branch: main
  
  url: https://github.com/hudmol/as_spreadsheet_bulk_updater.git
  
- name: aspace-oauth

  branch: v3.2.0
  
  url: https://github.com/lyrasis/aspace-oauth.git
  
- name: digitization_work_order

  branch: master
  
  url: https://github.com/duke-libraries/digitization_work_order.git
  
- name: editable_external_ids

  branch: master
  
  url: https://github.com/hudmol/editable_external_ids.git
  
- name: next_accession

  branch: master
  
  url: https://github.com/duspeccoll/next_accession.git
  
- name: princeton_ead_exporter

  branch: main
  
  url: https://github.com/pulibrary/princeton_ead_exporter.git
  
- name: refid_rules

  branch: master
  
  url: https://github.com/archivesspace-plugins/refid_rules.git
  
- name: user_defined_in_basic

  branch: release 1.0
  
  url: https://github.com/hudmol/user_defined_in_basic.git
  
  updated: 4/20/2023
  

