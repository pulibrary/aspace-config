# aspace-config
Our ArchivesSpace configuration choices, including plugins and their versions.

We install any new plugins, version updates, or config changes on dev for testing before making the corresponding change on prod.

**Prod status:**

Prod is behind by one version on user_defined_in_basic.

**Dev status:**

These are the plugins we currently have installed on dev. 

```
plugins:
     - name: as_princeton_shim
       branch: v1.0
       url: https://github.com/hudmol/as_princeton_shim.git
     - name: editable_external_ids
       branch: master
       url: https://github.com/hudmol/editable_external_ids.git
     - name: aspace-oauth
       branch: v3.2.0
       url: https://github.com/lyrasis/aspace-oauth.git
     - name: princeton_ead_exporter
       branch: main
       url: https://github.com/pulibrary/princeton_ead_exporter.git
     - name: user_defined_in_basic
       branch: release 1.0
       url: https://github.com/hudmol/user_defined_in_basic.git
     - name: refid_rules
       branch: master
       url: https://github.com/archivesspace-plugins/refid_rules.git
     - name: next_accession
       branch: master
       url: https://github.com/duspeccoll/next_accession.git
     - name: digitization_work_order
       branch: master
       url: https://github.com/duke-libraries/digitization_work_order.git
     - name: as_spreadsheet_bulk_updater
       branch: main
       url: https://github.com/hudmol/as_spreadsheet_bulk_updater.git
```
