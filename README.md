# aspace-config
Our ArchivesSpace configuration choices, including plugins and their versions.

We install any new plugins, version updates, or config changes on dev for testing before making the corresponding change on prod.

**We are on v3.3.1**

**Prod status:**

These are the plugins we currently have installed on prod.


  - name: aspace-oauth
    
    branch: v3.2.0
    
    url: https://github.com/lyrasis/aspace-oauth.git
    
 - name: as_marcao
 
    branch: v0.5
    
    url: https://github.com/hudmol/as_marcao.git
    
    added: 5/30/2023
    
  - name: as_princeton_shim
    
    branch: v1.0
    
    url: https://github.com/hudmol/as_princeton_shim.git  
    
 - name: as_spreadsheet_bulk_updater
    
    branch: main
    
    url: https://github.com/hudmol/as_spreadsheet_bulk_updater.git
    
   - name: digitization_work_order
    
    branch: master
    
    url: https://github.com/duke-libraries/digitization_work_order.git
    
  - name: newrelic
    
    url: https://github.com/archivesspace-plugins/newrelic.git
    
    branch: master
    
    restricted: true
    
 - name: next_accession
    
    branch: master
    
    url: https://github.com/duspeccoll/next_accession.git

  - name: princeton_ead_exporter
    
    branch: main
    
    url: https://github.com/pulibrary/princeton_ead_exporter.git
    
  - name: refid_rules
    
    branch: master
    
    url: https://github.com/archivesspace-plugins/refid_rules.git
    
  - name: timewalk
    
    branch: master
    
    url: https://github.com/alexduryee/timewalk.git
    
  - name: user_defined_in_basic
    
    branch: '1.0'
    
    url: https://github.com/hudmol/user_defined_in_basic.git
    
    updated: 5/30/2023
  
**Dev status:**

These are the plugins we currently have installed on dev. 

- name: as_princeton_shim

  branch: v1.0
  
  url: https://github.com/hudmol/as_princeton_shim.git
  
  **NB this plugin is specific to v3.2. It was upgraded but may at this point be creating problems**
  
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
  

