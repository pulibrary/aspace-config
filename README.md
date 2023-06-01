# aspace-config
Our ArchivesSpace configuration choices, including plugins and their versions.

We install any new plugins, version updates, or config changes on dev for testing before making the corresponding change on prod.

**We are on v3.3.1**

| plugin | staging | prod |
| ------ | ------- | ---- |
| aspace-oauth | branch: v3.2.0 <br/> url: https://github.com/lyrasis/aspace-oauth.git | branch: v3.2.0 <br/> url: https://github.com/lyrasis/aspace-oauth.git |
| as_marcao | [removed to avoid conflict writing to sftp staging] | branch: v0.5 <br/> url: https://github.com/hudmol/as_marcao.git <br/> added: 5/30/2023 |
| as_princeton_shim | branch: v1.0 <br/> url: https://github.com/hudmol/as_princeton_shim.git <br/> **NB this plugin is specific to v3.2. It was upgraded but may at this point be creating problems** | branch: v1.0 <br/> url: https://github.com/hudmol/as_princeton_shim.git |
| as_spreadsheet_bulk_updater | branch: main <br/> url: https://github.com/hudmol/as_spreadsheet_bulk_updater.git | branch: main <br/> url: https://github.com/hudmol/as_spreadsheet_bulk_updater.git |
| digitization_workorder | branch: master <br/> url: https://github.com/duke-libraries/digitization_work_order.git | branch: master <br/> url: https://github.com/duke-libraries/digitization_work_order.git |
| editable_external_ids | branch: master <br/> url: https://github.com/hudmol/editable_external_ids.git | n/a |
| newrelic | n/a | url: https://github.com/archivesspace-plugins/newrelic.git <br/> branch: master <br/> restricted: true |
| next_accession | branch: master <br/> url: https://github.com/duspeccoll/next_accession.git| branch: master </br> url: https://github.com/duspeccoll/next_accession.git |
| princeton_ead_exporter | branch: main <br/> url: https://github.com/pulibrary/princeton_ead_exporter.git | branch: main <br/> url: https://github.com/pulibrary/princeton_ead_exporter.git |
| refid_rules | branch: master <br/> url: https://github.com/archivesspace-plugins/refid_rules.git | branch: master <br/> url: https://github.com/archivesspace-plugins/refid_rules.git
| timewalk | n/a | branch: master <br/> url: https://github.com/alexduryee/timewalk.git
| user_defined_in_basic | branch: release 1.0<br/> url: https://github.com/hudmol/user_defined_in_basic.git <br/> updated: 4/20/2023 | branch: '1.0' <br/> url: https://github.com/hudmol/user_defined_in_basic.git <br/> updated: 5/30/2023
